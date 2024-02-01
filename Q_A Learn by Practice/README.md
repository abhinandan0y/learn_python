# test  
```
<div>
<pre><code class="language-python">
from django.contrib.auth.models import Group
my_group = Group.objects.get(name='my_group_name') 
my_group.user_set.add(your_user)
</code></pre>
    </div>

<div>
    <pre><code class="language-python">
    def hello_world():
        print("Hello, world!")
    </code></pre>
</div>
