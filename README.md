# Matrix-operation-using-array
To implement matrix operation using array
m=int(input("Enter no. of rows of matrix : "))
n=int(input("Enter no. of columns of matrix : "))
print("Enter the values into matrix1::")
matrix1=[[int(input())for i in range(m)]for j in range (n)]
print("Matrix 1 is")
for i in range(m):
	for j in range(n):
		print(matrix1[i][j],end=" ")
	print()

print("Enter the values into matrix2::")
matrix2=[[int(input())for i in range(m)]for j in range (n)]
print("Matrix 2 is")
for i in range(m):
	for j in range(n):
		print(matrix2[i][j],end=" ")
	print()

#<********************************************************************>

result1=[[0 for i in range(m)]for j in range (n)]
print("Addition Result ")
for i in range(m):
	for j in range(n):
		result1[i][j]=matrix1[i][j]+matrix2[i][j]
for i in range (m):
	for j in range (n):
		print(result1[i][j],end=" ")
	print()

#<********************************************************************>

result2=[[0 for i in range(m)]for j in range (n)]
print("Substraction Result ")
for i in range(m):
	for j in range(n):
		result2[i][j]=matrix1[i][j]-matrix2[i][j]
for i in range (m):
	for j in range (n):
		print(result2[i][j],end=" ")
	print()
	
#<********************************************************************>

result3=[[0 for i in range(m)]for j in range (n)]
print("Transpose Matrix Result ")
for i in range(m):
	for j in range(n):
		result3[j][i]=matrix1[i][j]
for i in range (m):
	for j in range (n):
		print(result3[i][j],end=" ")
	print()

#<********************************************************************>
	
result4=[[0 for i in range(m)]for j in range (n)]
print("Multiplication is ")
for i in range(m):
	for j in range(n):
		for k in range(m):
			result4[i][j]=result4[i][j]+matrix1[i][k]*matrix2[k][j]
for i in range (m):
	for j in range (n):
		print(result4[i][j],end=" ")
	print()

#<*****************************END OF PROGRAM**************************************>


