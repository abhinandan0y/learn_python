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

adding-days-to-a-date-in-python.txt
    
<p>The previous answers are correct but it's generally a better practice to do:</p>

<code class="language-python">import datetime
</code>

<p>Then you'll have, using <a href="https://docs.python.org/2/library/datetime.html#datetime.timedelta" rel="noreferrer"><code class="language-python">datetime.timedelta</code></a>:</p>

<code class="language-python">date_1 = datetime.datetime.strptime(start_date, "%m/%d/%y")

end_date = date_1 + datetime.timedelta(days=10)
</code>
