# sumOfDigitsFrom1ToN
def sumOfDigitsFrom1ToN(n) : 
  
    result = 0   
 
    for x in range(1**2, (n+1)**2) : 
        result = result + sumOfDigits(x) 
   
    return result 

def sumOfDigits(x) : 
    sum = 0
    while (x != 0) : 
        sum = sum + x % 10
        x  = x // 10
      
    return sum


def multi(n):
    for y in range(n, n+1, 2*n+1) :
        result = n*(n+1)*(2*n+1)
        result = result / 6
   
    return result   


n = int(input("Enter a number: "))

print("Sum of digits in numbers from 1 to", n, "is", sumOfDigitsFrom1ToN(n)) 
  
print("multi", n, "is", multi(n))
