# 
🔥 Essential Programming Math/Logic Concepts


---

1. Prime Number

👉 A number divisible only by 1 and itself.

Example: 2, 3, 5, 7 (prime), but 4, 6, 9 are not.


n = 7
prime = True
for i in range(2, n):
    if n % i == 0:
        prime = False
        break
print("Prime" if prime else "Not Prime")


---

2. Fibonacci Series

👉 Each number is sum of the previous two.

Example: 0, 1, 1, 2, 3, 5, 8, 13


a, b = 0, 1
for _ in range(10):
    print(a, end=" ")
    a, b = b, a + b


---

3. Factorial

👉 Multiply a number by all numbers below it.

Example: 5! = 5 × 4 × 3 × 2 × 1 = 120


n = 5
fact = 1
for i in range(1, n+1):
    fact *= i
print(fact)


---

4. Palindrome Number / String

👉 Reads same forward & backward.

Example: 121, madam, radar.


s = "121"
print("Palindrome" if s == s[::-1] else "Not Palindrome")


---

5. Armstrong Number

👉 Sum of digits^power = number itself.

Example: 153 = 1³ + 5³ + 3³ = 153


n = 153
s = sum(int(d)**len(str(n)) for d in str(n))
print("Armstrong" if s == n else "Not Armstrong")


---

6. Reverse Number / String

👉 Reverse the order.

Example: 123 → 321, hello → olleh


n = "12345"
print(n[::-1])


---

7. Sum of Digits

👉 Add all digits.

Example: 123 → 1+2+3 = 6


n = 123
print(sum(int(d) for d in str(n)))


---

8. Greatest Common Divisor (GCD)

👉 Largest number that divides two numbers.

Example: GCD(12, 18) = 6


import math
print(math.gcd(12, 18))


---

9. Least Common Multiple (LCM)

👉 Smallest number divisible by both.

Example: LCM(4, 5) = 20


import math
print(math.lcm(4, 5))


---

10. Prime Factorization

👉 Break number into prime factors.

Example: 28 = 2 × 2 × 7


n = 28
i = 2
factors = []
while n > 1:
    if n % i == 0:
        factors.append(i)
        n //= i
    else:
        i += 1
print(factors)


---

11. Perfect Number

👉 Sum of divisors (excluding itself) = number.

Example: 6 → 1+2+3 = 6


n = 6
s = sum(i for i in range(1, n) if n % i == 0)
print("Perfect" if s == n else "Not Perfect")


---

12. Strong Number

👉 Sum of factorials of digits = number.

Example: 145 → 1! + 4! + 5! = 145


import math
n = 145
s = sum(math.factorial(int(d)) for d in str(n))
print("Strong" if s == n else "Not Strong")


---

13. Leap Year

👉 Divisible by 4 (except century years unless divisible by 400).

Example: 2000 ✅, 1900 ❌, 2024 ✅.


year = 2024
if (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0):
    print("Leap Year")
else:
    print("Not Leap Year")


---

14. Swap Numbers

👉 Exchange two values without a third variable.


a, b = 5, 10
a, b = b, a
print(a, b)  # 10 5


---

15. Patterns (Stars & Numbers)

👉 Used to test loops + logic.

Example:

*
**
***
****

n = 5
for i in range(1, n+1):
    print("*" * i)


---

🎯 Interview Tip

These cover 90% of beginner coding interview questions.

Learn:

1. Concept (definition + example)


2. Code logic (don’t just memorize)


3. Edge cases (e.g., 0, 1, negative numbers)





---
