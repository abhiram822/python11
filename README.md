#niven number
num = int(input("Enter a number: "))
original_num = num  
sum_digits = 0
while num > 0:
    d = num % 10
    sum_digits += d
    num //= 10
if original_num % sum_digits == 0:
    print(f"{original_num} is a Niven number.")
else:
    print(f"{original_num} is not a Niven number.")
