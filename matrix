class Matrix:
    def __init__(self, data):
        self.data = data

    def __add__(self, other):
        result = []
        for i in range(len(self.data)):
            row = []
            for j in range(len(self.data[0])):
                row.append(self.data[i][j] + other.data[i][j])
            result.append(row)
        return Matrix(result)

    def __sub__(self, other):
        result = []
        for i in range(len(self.data)):
            row = []
            for j in range(len(self.data[0])):
                row.append(self.data[i][j] - other.data[i][j])
            result.append(row)
        return Matrix(result)

    def __mul__(self, other):
        result = []
        for i in range(len(self.data)):
            row = []
            for j in range(len(other.data[0])):
                s = 0
                for k in range(len(other.data)):
                    s += self.data[i][k] * other.data[k][j]
                row.append(s)
            result.append(row)
        return Matrix(result)

    def __str__(self):
        return str(self.data)


m1 = Matrix([[1, 2], [3, 4]])
m2 = Matrix([[5, 6], [7, 8]])

print("Addition:", m1 + m2)
print("Subtraction:", m1 - m2)
print("Multiplication:", m1 * m2)
