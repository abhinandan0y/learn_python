# test  
<code class="language-python">    def hello_world():
        print("Hello, world!")
<p>Find the group using Group model with the name of the group, then add the user to the user_set</p>

<pre><code class="language-python"> from django.contrib.auth.models import Group
my_group = Group.objects.get(name='my_group_name') 
my_group.user_set.add(your_user)
</code></pre>
