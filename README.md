# Reverse-each-word-of-a-string in python
str = input()
len = len(str)
i = j = startIndex = 0
endIndex = len - 1
for i in range(len - 1, -1, -1):
    if str[i] == ' ' or i == 0:
        if i == 0:
            startIndex = 0
        else:
            startIndex = i + 1
        for j in range(startIndex, endIndex + 1):
            print(str[j], end='')
        endIndex = i - 1
        print(" ", end='')
