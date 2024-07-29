import random
random.seed()   #Prepare random number generator

print("Find the element that appears most often in the array")
print("Enter the number of elements of the array")
print("Enter n")
n = int(input())
a = [0] * (n)
b = [0] * (1000)

for i in range(0, n - 1 + 1, 1):
    b[i] = 0
print("The random elements are")
for i in range(0, n - 1 + 1, 1):
    a[i] = int(random.random() * 10)
    print(a[i])
    b[a[i]] = b[a[i]] + 1
max = 0
maxt = 0
for i in range(0, n - 1 + 1, 1):
    if max < b[a[i]]:
        max = b[a[i]]
for i in range(0, n - 1 + 1, 1):
    if max == b[a[i]]:
        maxt = a[i]
print("Element that repeats the most times is " + maxt)
print("The number of repetitions is " + max)

![Screenshot 2024-07-29 215347](https://github.com/user-attachments/assets/46e2a359-fc84-4679-9494-c581e75d8190)

