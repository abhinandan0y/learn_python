# test  

<p>Find the group using Group model with the name of the group, then add the user to the user_set</p>

<p>For that reason, the count needs to fit in the platform C   <code class="language-python">ssize_t</code> 
  type, which is generally at most  <code class="language-python">2**31 - 1</code>   on a 32-bit box, and here on a 64-bit box:</p>

<code class="language-python">from django.contrib.auth.models import Group
my_group = Group.objects.get(name='my_group_name') 
my_group.user_set.add(your_user)
</code>

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
access-uri-parameters-via-webapp2.txt

    
<code class="language-python">class User(webapp2.RequestHandler):
  def get(self):
    un = self.request.get('un')
    pw = self.request.get('pw')
    self.response.headers['Content-Type'] = 'text/plain'
    self.response.write('Yey!' + un + ' ' + pw)
</code>
adding-a-user-to-a-group-in-django.txt
    
<p>Find the group using Group model with the name of the group, then add the user to the user_set</p>

<code class="language-python">from django.contrib.auth.models import Group
my_group = Group.objects.get(name='my_group_name') 
my_group.user_set.add(your_user)
</code>


adding-days-to-a-date-in-python.txt
    
<p>The previous answers are correct but it's generally a better practice to do:</p>

<code class="language-python">import datetime
</code>

<p>Then you'll have, using <a href="https://docs.python.org/2/library/datetime.html#datetime.timedelta" rel="noreferrer"><code class="language-python">datetime.timedelta</code></a>:</p>

<code class="language-python">date_1 = datetime.datetime.strptime(start_date, "%m/%d/%y")

end_date = date_1 + datetime.timedelta(days=10)
</code>
