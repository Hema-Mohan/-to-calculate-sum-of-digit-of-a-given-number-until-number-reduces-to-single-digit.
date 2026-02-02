# -to-calculate-sum-of-digit-of-a-given-number-until-number-reduces-to-single-digit.
number = int(input("Enter number: "))
total_sum = 0
step = 1

condition = True

while condition:
    
    while number:
        total_sum += number%10
        number //= 10
    
    print("Step-%d Sum: %d" %(step, total_sum))
    number = total_sum
    total_sum = 0
    step += 1
    condition = number > 9
OUTPUT:
Enter number: 999999999
Step-1 Sum: 81
Step-2 Sum: 9
