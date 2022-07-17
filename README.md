# PYTHON-CODE-Smallest-Positive-Number-From-an-Array
# Program that Returns Smallest Positive Number From an Array

def solution(A):
    A.sort()
    if A[0] >= 1:
        for item in range(A[0], A[-1]):
                if item not in A:
                    print(item)
                    break

        else:
            if A[0] != 1:
                print(A[0] - 1)
            else:
                print(A[-1] + 1)
    else:
        print(1)


A = [1, 3, 6, 4, 1, 2]
check = solution(A)
check
