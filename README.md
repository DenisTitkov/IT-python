a = []
while x != -1:
    x = int(input("Enter the number"))
    a.append(x)
n = len(a)
s = 0
m = a[0]
if n == 0:
    m = -1
    a = -1
for i in range(n-1):
    s = s + a[i]
    if a[i] < m:
        m = a[i]
if n != 0:
    a = s/n

print(s)
print(a)
print(m)
