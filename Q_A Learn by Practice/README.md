# test  

<p>Using</p>

<code class="language-python">for _ in itertools.repeat(None, count)
    do something
</code>

<p>is the non-obvious way of getting the best of all worlds: tiny constant space requirement, and no new objects created per iteration. Under the covers, the C code for <code class="language-python">repeat</code> uses a native C integer type (not a Python integer ob
ject!) to keep track of the count remaining.</p>

<p>For that reason, the count needs to fit in the platform C <code class="language-python">ssize_t</code> type, which is generally at most <code class="language-python">2**31 - 1</code> on a 32-bit box, and here on a 64-bit box:</p>

<code class="language-python">&gt;&gt;&gt; itertools.repeat(None, 2**63)
Traceback (most recent call last):
    ...
OverflowError: Python int too large to convert to C ssize_t

&gt;&gt;&gt; itertools.repeat(None, 2**63-1)
repeat(None, 9223372036854775807)
</code>

<p>Which is plenty big for my loops ;-)</p>

