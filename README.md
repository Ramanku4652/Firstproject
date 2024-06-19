def r(X, Y, Z, target):
    result = []
    for x in X:
        for y in Y:
            for z in Z:
                if x + y + z == target:
                    result.append((x, y, z))
    return result
input_data = input("")
data = list(map(int, input_data.split()))
X = data[:4]
Y = data[5:9]
Z = data[10:14]
target = data[-1]
combinations = r(X, Y, Z, target)
print(combinations)
