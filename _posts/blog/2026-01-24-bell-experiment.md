---
layout: post
title: Bell's Experiment with (Local) Reality - Classical Bound
categories: blog
permalink: blog/bell_test_classical
---

Bell's experiment was the final nail in the coffin for the prevalent intuition of the world -- local realism. The test gave a 'simple' way to test quantum physics and either disprove/prove Einstein, Podolsky, and Rosen's argument (EPR) that quantum mechanics was an incomplete picture of the world.

<!--more-->

Local realism is the intuitive idea that physical properties of objects exist objectively and independently of measurement (realism) and that influences can't travel faster than light (locality), meaning distant events can't instantaneously affect each other. Both seem reasonable to assume. Einstein certainly thought so, especially with this wildly successful theory, Relativity, was build on the postulate that no information travels faster than the speed of light. Around the same time as relativity, there was a new kid on the block, quantum mechanics, which Einstein helped develop as well. Quantum mechanics was proving to be incredibly successful in prredicting different phenomena at the atomic/nuclear scale, and helped patch several holes with classical theory as well. But Einstein was really happy with this new 'weird' theory. After years of debate between Neils Bohr and Einstein, the EPR paper have a relatively simple argument that quantum mechanics predicted that local realism was not possible. Atleast one, locality or realism, needed to be forgotten.  

Enter John Bell, thirty years later. He devised an experiment (or a game) that predicted that a player using only local real resources can only win 75% of the time, whereas a player using quantum resources could win around 85% of the time! And many years later, as people devised ways to actually control quantum systems, they played this game and showed that quantum mechanics is just that good at this game. Let's try to take a look at the simplified version of the game, and see why a player with local real resources can only win 75% of the time -- an upper bound on the winning probability.

They game is played by two players Alice and Bob, who are on one team, against a referee. The referee send one bit each -- $x$ and $y$ to Alice and Bob, respectively. Alice and Bob then individually need to send a single bit as a response -- $a$ from Alive, and $b$ from Bob. Alice and Bob win the game when 

$$
x \cdot y = a \oplus b,
$$

where the left hand size is the AND operation, and the right hand size is the XOR operation. 
<div style="display: flex; gap: 40px; justify-content: center; margin: 1.5em 0;">

  <div>
    <div style="font-weight: 600; text-transform: none; margin-bottom: 0.3em;">
      AND ($x \cdot y$)
    </div>
    <table style="border-collapse: collapse; table-layout: fixed; width: 270px;">
      <tr>
        <th style="border: 1px solid black; padding: 4px; width: 90px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible; box-sizing: border-box;">
          $x$
        </th>
        <th style="border: 1px solid black; padding: 4px; width: 90px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible; box-sizing: border-box;">
          $y$
        </th>
        <th style="border: 1px solid black; padding: 4px; width: 90px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible; box-sizing: border-box;">
          $x \cdot y$
        </th>
      </tr>
      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$0$</td>
      </tr>
      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$0$</td>
      </tr>
      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$0$</td>
      </tr>
      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$1$</td>
      </tr>
    </table>
  </div>

  <div>
    <div style="font-weight: 600; text-transform: none; margin-bottom: 0.3em;">
      XOR ($a \oplus b$)
    </div>
    <table style="border-collapse: collapse; table-layout: fixed; width: 270px;">
      <tr>
        <th style="border: 1px solid black; padding: 4px; width: 90px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible; box-sizing: border-box;">
          $a$
        </th>
        <th style="border: 1px solid black; padding: 4px; width: 90px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible; box-sizing: border-box;">
          $b$
        </th>
        <th style="border: 1px solid black; padding: 4px; width: 90px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible; box-sizing: border-box;">
          $a \oplus b$
        </th>
      </tr>
      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$0$</td>
      </tr>
      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$1$</td>
      </tr>
      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$1$</td>
      </tr>
      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;
                   text-transform: none; overflow: visible;">$0$</td>
      </tr>
    </table>
  </div>

</div>

Alice and Bob can meet up beforehand and come up the strategies. But once they begin the game, they cannot communicate in any way. The way to enforce this usually is to have Alice and Bob be in far away rooms. We're about to delve in some slightly heavy. If you're not interested, you can skip down to the example section. 

Here we go. How do we model the winning probability? Define a function $\mathcal{I}$ that is $1$ if $x \cdot y = a \oplus b$ and $0$ otherwise. So the winning probability is given by

$$
\begin{align}
    p_{\text{win}} &=  \sum_{a, b, x, y} p(a, b, x, y) \mathcal{I}(a, b, x, y), \\
    &= \sum_{a, b, x, y} p(a, b \vert x, y) p(x, y) \mathcal{I}(a, b, x, y), \\
    &= \frac{1}{4} \sum_{a, b, x, y} p(a, b \vert x, y) \mathcal{I}(a, b, x, y).
\end{align}
$$

Okay let's break down what happened there. The winning probability is the average of the function $\mathcal{I}$. The probability distribution $p(a, b, x, y)$ encodes the strategy that Alice and Bob use. Since $a, b$ depend on $x, y$ in our game, we can write $p(a, b, x, y) = p(a, b \vert x, y) p(x, y)$. $p(\text{event }A \vert \text{event } B)$ is called the conditional probability and is defined as the probability that event $A$ occurs given that event $B$ has already occured. We also make the assumption that $p(x, y) = \frac{1}{4}$, since the referee has no reason to preferentially pick any $x$ or $y$. So the strategy that Alice and Bob is encoded in the conditional distribution $p(a, b \vert x, y). Now, we need to <i>impose</i> the two conditions -- that they could have met beforehand and shared some results, and they cannot communicate after the referee bits have been sent out. 

The way to impose the first constraint is that they could have shared some random bits between themselves. This type of shared randomness has been shown to boost winning probabilities and is considered the most general (local real) resource they can share beforehand. Let's call the random string of bits they share $r$. So we replace the conditional distribution with

$$
    p(a, b \vert x, y) = \sum_{r} p(r) p(a, b \vert x, y, r).
$$

The conditional probability depends on $r$ and how likely a particular string $r$ is. So we average over all possible $r$ values ($\sum_r p(r) f(r)$ is the definitiion of the average of some function $f(r)$)! Next, we need to encode that they cannot communicate. This leads to the conditional probability to factor into two indepedent terms!

$$
    p(a, b \vert x, y, r) = p(a \vert x, r) p(b \vert y, r).
$$

Putting it all together, we see that the winning probability is then

$$
    \begin{align}
        p_{\text{win}} &= \frac{1}{4} \sum_{a, b, x, y} p(a, b \vert x, y) \mathcal{I}(a, b, x, y), \\
        &= \frac{1}{4} \sum_{a, b, x, y, r} p(r) p(a \vert x, r) p(b \vert y, r) \mathcal{I}(a, b, x, y).
    \end{align}
$$

Here is the step that might the hardest to understand without some intuition. The final equation can be grouped simply as 

$$
\begin{align}
\frac{1}{4} \sum_{a, b, x, y, r} p(r) p(a \vert x, r) p(b \vert y, r) \mathcal{I}(a, b, x, y) &= \sum_{r} p(r) \left[ \frac{1}{4} \sum_{a, b, x, y} p(a \vert x, r) p(b \vert y, r) \mathcal{I}(a, b, x, y) \right], \\
&\leq \frac{1}{4} \sum_{a, b, x, y} p(a \vert x, r^*) p(b \vert y, r^*) \mathcal{I}(a, b, x, y).
\end{align}
$$

What did we do in the above equation? Since the winning probability is clearly an average over the possible values of $r$, there must be some optimal string $r^* $. For any distribution, the average is always less than or equal to the maximum. (Think about a simple game where you roll a weighted dice and depending on the face that lands up, you win some cash. If you play multiple times, you will get the average reward, but there must be a best outcome.) We might not know what the optimal string is, but for the proof, we can replace the average with the maximum $r^* $.

Okay that was a lot of math. The tl;dr of the entire math above is that the classical winning probability is bounded from above by a funky looking quantity that depends on the way Alice and Bob respond to their bits, and they optimal shared bitstring. Let's finally look at some examples.

## Examples!

<ol>
  <li>
    <p><strong>Alice and Bob always return whatever bit they are sent in.</strong></p>

<div style="display: flex; justify-content: center; margin: 1.5em 0;">
  <div>
    <div style="font-weight: 600; text-transform: none; margin-bottom: 0.3em;">
      Strategy: $a = x,\; b = y$
    </div>

    <table style="border-collapse: collapse; table-layout: fixed; width: 450px;">
      <tr>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$x$</th>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$y$</th>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$a$</th>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$b$</th>
        <th style="border: 1px solid black; padding: 4px; width: 150px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">
          $x \cdot y = a \oplus b$
        </th>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\checkmark$</td>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\checkmark$</td>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\checkmark$</td>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\times$</td>
      </tr>
    </table>
</div>
</div>

    <p>
      The winning probability in this case is $\frac{3}{4}$ or $75\%$.
    </p>
  </li>

<li>
<p><strong>Alice always return $0$, and Bob always returns $1$.</strong></p>

<div style="display: flex; justify-content: center; margin: 1.5em 0;">
  <div>
    <div style="font-weight: 600; text-transform: none; margin-bottom: 0.3em;">
      Strategy: $a = 0,\; b = 1$
    </div>

    <table style="border-collapse: collapse; table-layout: fixed; width: 450px;">
      <tr>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$x$</th>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$y$</th>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$a$</th>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$b$</th>
        <th style="border: 1px solid black; padding: 4px; width: 150px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">
          $x \cdot y = a \oplus b$
        </th>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\times$</td>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\times$</td>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\times$</td>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\checkmark$</td>
      </tr>
    </table>
  </div>
</div>

<p>
      The winning probability in this case is $\frac{1}{4}$ or $25\%$.
    </p>
  </li>

<li>
<p><strong>Shared Randomness</strong></p>

Alice and Bob met beforehand and share a secret string $r = 101101$. For round $i$, Alice returns $a = x \oplus r_i$ and Bob returns $b = y \cdot r_i$. For example, round $1$ with $r_1 = 1$ leads to

<div style="display: flex; justify-content: center; margin: 1.5em 0;">
  <div>
    <div style="font-weight: 600; text-transform: none; margin-bottom: 0.3em;">
      Strategy: $a = x \oplus 1\; b = y \cdot 1$
    </div>

    <table style="border-collapse: collapse; table-layout: fixed; width: 450px;">
      <tr>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$x$</th>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$y$</th>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$a$</th>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$b$</th>
        <th style="border: 1px solid black; padding: 4px; width: 150px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">
          $x \cdot y = a \oplus b$
        </th>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\times$</td>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\checkmark$</td>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\checkmark$</td>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\times$</td>
      </tr>
    </table>
  </div>
</div>

The winning probability in this case is $\frac{1}{2}$ or $50\%$. Round $2$ with $r_1 = 0$ leads to

<div style="display: flex; justify-content: center; margin: 1.5em 0;">
  <div>
    <div style="font-weight: 600; text-transform: none; margin-bottom: 0.3em;">
      Strategy: $a = x \oplus 0\; b = y \cdot 0$
    </div>

    <table style="border-collapse: collapse; table-layout: fixed; width: 450px;">
      <tr>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$x$</th>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$y$</th>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$a$</th>
        <th style="border: 1px solid black; padding: 4px; width: 75px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">$b$</th>
        <th style="border: 1px solid black; padding: 4px; width: 150px; text-align: center;
                   text-transform: none; white-space: nowrap; overflow: visible;">
          $x \cdot y = a \oplus b$
        </th>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\checkmark$</td>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\checkmark$</td>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\times$</td>
      </tr>

      <tr>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$1$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$0$</td>
        <td style="border: 1px solid black; padding: 4px; text-align: center;">$\checkmark$</td>
      </tr>
    </table>
  </div>
</div>

<p>
      The winning probability in this case is $\frac{3}{4}$ or $75\%$. Turns out, if the string they share is perfectly random, they win with probability $62.5\%$.
    </p>
  </li>
</ol>

Long story short, it turns out, using the equation we derived, we can show that using classical resources only, Alice and Bob can only with a maximum of $75\%$. There is no strategy, or no preshared resources they can use to win with anything above this. In the next [part](/blog/bell_experiments_quantum), we're going to look at a relatively simple quantum system that helps Alice and Bob beat this.
