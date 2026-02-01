# program-to-print-butterfly-pattern-made-of-stars-up-to-n-number-of-lines-given-by-user.
row = int(input(&quot;Enter number of rows (even): &quot;))

n = row//2

print(&quot;Generated butterfly pattern is:\n&quot;)
# Upper part
for i in range(1,n+1):
for j in range(1, 2*n+1):
if j&gt;i and j&lt; 2*n+1-i:
print(&quot; &quot;, end=&quot;&quot;)
else:
print(&quot;* &quot;, end=&quot;&quot;)
print()

# Lower part
for i in range(n,0,-1):
for j in range(2*n,0,-1):
if j&gt;i and j&lt; 2*n+1-i:
print(&quot; &quot;, end=&quot;&quot;)
else:
print(&quot;* &quot;, end=&quot;&quot;)
print()
