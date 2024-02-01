# test  

<p>Find the group using Group model with the name of the group, then add the user to the user_set</p>

<p>For that reason, the count needs to fit in the platform C   <code class="language-python">ssize_t</code> 
  type, which is generally at most  <code class="language-python">2**31 - 1</code>   on a 32-bit box, and here on a 64-bit box:</p>

<code class="language-python">from django.contrib.auth.models import Group
my_group = Group.objects.get(name='my_group_name') 
my_group.user_set.add(your_user)
</code>
