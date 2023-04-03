# SISTEMAS-LINEARES
USANDO PYTHON PARA RESOLUCAO DOS SISTEMAS LINEARES
A = [[2, -1], [1, 5]]
# Constantes
B = [7, -2]
n = len(B)
for i in range(n):
       div = A[i][i]
    A[i] = [a/div for a in A[i]]
    B[i] /= div
    
    for j in range(i+1, n):
        mult = A[j][i]
        A[j] = [a - mult*b for a, b in zip(A[j], A[i])]
        B[j] -= mult*B[i]
for i in range(n-1, -1, -1):
       for j in range(i-1, -1, -1):
        mult = A[j][i]
        A[j] = [a - mult*b for a, b in zip(A[j], A[i])]
        B[j] -= mult*B[i]
x = B
print("x =", x[0])
print("y =", x[1])








# x + 2y - z = 0
# 3x - 4y + 5z = 10
# x - y + 9z = 1

A = [[1, 2, -1], [3, -4, 5], [1, -1, 9]]
B = [0, 10, 1]
n = len(B)

for i in range(n):
        div = A[i][i]
    A[i] = [a/div for a in A[i]]
    B[i] /= div
    
        for j in range(i+1, n):
        mult = A[j][i]
        A[j] = [a - mult*b for a, b in zip(A[j], A[i])]
        B[j] -= mult*B[i]

for i in range(n-1, -1, -1):
    for j in range(i-1, -1, -1):
        mult = A[j][i]
        A[j] = [a - mult*b for a, b in zip(A[j], A[i])]
        B[j] -= mult*B[i]
x = B
print("x =", x[0])
print("y =", x[1])
print("z =", x[2])





A = [[1, 2], [2, -3]]
B = [5, -4]
n = len(B)

for i in range(n):
        div = A[i][i]
    A[i] = [a/div for a in A[i]]
    B[i] /= div
    
    for j in range(i+1, n):
        mult = A[j][i]
        A[j] = [a - mult*b for a, b in zip(A[j], A[i])]
        B[j] -= mult*B[i]

for i in range(n-1, -1, -1):
    for j in range(i-1, -1, -1):
        mult = A[j][i]
        A[j] = [a - mult*b for a, b in zip(A[j], A[i])]
        B[j] -= mult*B[i]

x = B
print("x =", x[0])
print("y =", x[1])



# x + y = 5
# 2x + 2y = 10

A = [[1, 1], [2, 2]]
B = [5, 10]
n = len(B)
for i in range(n):
    div = A[i][i]
    A[i] = [a/div for a in A[i]]
    B[i] /= div
    
    for j in range(i+1, n):
        mult = A[j][i]
        A[j] = [a - mult*b for a, b in zip(A[j], A[i])]
        B[j] -= mult*B[i]

for i in range(n-1, -1, -1):
    for j in range(i-1, -1, -1):
        mult = A[j][i]
        A[j] = [a - mult*b for a, b in zip(A[j], A[i])]
        B[j] -= mult*B[i]

x = B
print("x =", x[0])
print("y =", x[1])


