---
layout: post
title: Elliptic Curve Cryptography - Part 1 Introduction
categories: blog
permalink: blog/ecc1
---

As part of my work, I have been reading about cryptography and how randomness plays a role in make our data secure. The latest thing I've read was on elliptic curve cryptography, and it's quite fascinating. So I want to write about it. This helps me clarify my thoughts, and scratches this "teaching" itch that I often have. 

<!--more-->

Cryptography is the study of secrets. It is the science behind protecting information so that someone cannot listen in and learn your secret data. It typically involves encoding your secret information in some form, sending it over an insecure channel, like the internet, and having your intended recipient decode it. Let's just jump right into it. 

Let's look at two people, Alice and Bob, that live in two different cities. Alice wants to send Bob her ATM pin, which is the 4 digit number $1854$. However, she's worried about her enemy Eve listening in and stealing her pin number. To be absolutely sure that Eve cannot steal this information, Alice needs to be very clever about how to send this information to Bob. 

If we assume that Eve is very powerful, she might have access to Alice's internet data. If Alice emails the PIN to Bob, Eve would be able to steal the information. The "level of security" of the method Alice uses typically depends on how powerful you assume the eavesdropper Eve is. To be absolutely sure that an arbitarily powerful Eve could not steal the data, Alice and Bob use a protocol called the <b>One-Time Pad</b>, or OTP.

The most important assumption of the OTP protocol is that, ahead of time, Alice and Bob met in person and shared some secret numbers called the OTP. The PIN number she wants to send is called the message $m$. In this case, let's assume that the secret they shared was $0111\ 1010\ 0011\ 1011\ 0001\ 0111\ 1000$. This OTP is mixed in with the message in a specific way that makes her message uncrackable.

The first thing that Alice needs to do is to convert her message into ones and zeros, called binary notation. There is an easy method to do this, but for ease of explanation, I'm just going to write down the recipe that she uses

$$
    \begin{align}
        0 &\rightarrow 0000 \\
        1 &\rightarrow 0001 \\
        2 &\rightarrow 0010 \\
        3 &\rightarrow 0011 \\
        4 &\rightarrow 0100 \\
        5 &\rightarrow 0101 \\
        6 &\rightarrow 0110 \\
        7 &\rightarrow 0111 \\
        8 &\rightarrow 1000 \\
        9 &\rightarrow 1001 \\
    \end{align}
$$

So, the message $1854$ becomes $0001\ 1000\ 0101\ 0100$. This 16-bit binary number is now mixed with the first 16 bits of the shared secret, which is $0111\ 1010\ 0011\ 1011$. This mixing procedure is mathematically called bitwise addition modulo $2$. How does this work? It works like regular addition, expect instead of adding the entire 16-bit number as a whole, we just add each bit individually. In addition, we made a special rule that $1 \oplus 1 = 0$ and not $2$ (this is what addition modulo 2 means).

So for our case, Alice wants to mix $0001\ 1000\ 0101\ 0100$ and $0111\ 1010\ 0011\ 1011$. As an example, the first four bits become

$$
    \begin{align}
        0 \oplus 0 &= 0 \\
        0 \oplus 1 &= 1 \\
        0 \oplus 1 &= 1 \\
        1 \oplus 1 &= 0.
    \end{align}
$$

Thus, $0001\ 1000\ 0101\ 0100 \oplus 0111\ 1010\ 0011\ 1011 = 0110\ 0010\ 0110\ 1111$. Now, Alice sends this over any communication channel, like an email. 

But this new 16-bit string is clearly not the PIN, so what is Bob supposed to do with this? The beauty of the OTP protocol lies in its simplicity. Bob has to just do the same operation again! In other words, Bob mixes the encoded message he gets from Alice with the secret again, to get the real message. Mathematically if $m \oplus s = e$, then $e \oplus s$ is equal to $m$! Let's see this in action. $0110\ 0010\ 0110\ 1111 \oplus 0111\ 1010\ 0011\ 1011 = 0001\ 1000\ 0101\ 0100$, which is $m$. 

The real interesting part is that, as long as the secret $s$ is truly secret, the only thing Eve sees is the encoded $e$, from which Eve cannot get the message. The word 'cannot' is a strong word here -- Eve literally cannot do anything to find the message! It is independent of how powerful Eve is, how strong a computer she has, etc. This type of security is known as <b>information-theoretic security</b>.

So did we solve cryptography? Are we done? Far from it. The imporant caveat of the above construction is that, to send a message of length $n$, we need a shared secret of length $n$. This is a strong requirement. Alice cannot arbitrarily decide to send a large file to Bob, unless they have a large amount of preshared secret bits that they keep secret. Still, OTPs are used in scenarios like state-secrets, where security is paramount. A suitcase,with the secret key locked in it, is handcuffed to a courier and its flown to the intended recepient. Then, the OTP protocol is used to send previous secrets.

But can be we something better? Something that doesn't need preshared secret bits, so information can be sent at any time. Turns out the answer is yes, with a loss in the security level. While the security of the OTP is unconditional, there are methods to create protocols that do not need preshared secret keys, but which are secure only if some conditions are met. These conditions typically look like an assumption on the computational power of an adversary. Let's look at one of the most important and prevelant examples -- the RSA cryptosystem.

