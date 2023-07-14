# Assignment-6-placement-JPR

# 1. Print the following hill pattern , Input 5 Output
1
12
123
1234
12345
def hillpattern(n):
    for i in range(1,n+1):
        for j in range(1,i+1):
            print(j,end=" ")
        print()
n=int(input("enter the number of rows"))
print(hillpattern(n))


# 2. Print the following hill pattern ,When n=5
1
22
333
4444
55555

def hillpattern(n):
    for i in range(1,n+1):
        for j in range(1,i+1):
            print(i,end=" ")
        print()
n=int(input("enter the number of rows"))
print(hillpattern(n))


# 3. Print the following hill pattern ,When n=4
1
23
456
78910

def hillpattern(n):
    num=1
    for i in range(0,n):
        for j in range(0,i+1):
            print(num,end=" ")
            num+=1
        print()
n=int(input("enter the number of rows"))
print(hillpattern(n))

# 4. Print the following hill pattern ,When n=5
1
24
135
2468
13579

# 5. Print the following hill pattern , Each line contains n characters = space+number When n=5
      1
    1 2
  1 2 3
1 2 3 4

def hillpattern(n):
    for i in range(1,n+1):
        num=1
        for j in range(n,0,-1):
            if j>i:
                print(" ", end="")
            else:
                print(num, end="")
                num+=1
        print("\n")
n=int(input("enter the number of rows"))
print(hillpattern(n))


# 6. Count the prime number between X and y In put X= 5 , Y = 20 Output: 6 (5,7,11,13,17,19)
if __name__ == '__main__':
    a, b, i, j, flag = 0, 0, 0, 0, 0
    print("Enter lower bound of the interval:",
          end="")
    a = int(input())
    print(a)
    print("Enter upper bound of the interval:",
          end="")
    b = int(input())  
    print(b)
    print("Prime numbers between", a, "and",
          b, "are:", end="")
    for i in range(a, b + 1):
        if (i == 1):
            continue
        flag = 1
        for j in range(2, i // 2 + 1):
            if (i % j == 0):
                flag = 0
                break
        if (flag == 1):
            print(i, end=" ")



# 7. Find the Nth Prime number (first prime is 2) I/O: 3 5 I/O: 20 71
