# PYTHON MODULE - 2
# (E) Loops in Python: Palindrome Number Checker

## 🎯 Aim:
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm:
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program:

    num = int(input("ENTER A NUMBER :"))
    temp = num
    rev = 0
    while temp > 0:
        rev = (10 * rev) + temp % 10
        temp = temp // 10
    if rev == num :
        print(f"The given number {num} is Palindrome")
    else:
        print(f"The given number {num} is not Palindrome")

## Output:

<img width="615" height="316" alt="Screenshot 2025-10-20 173230" src="https://github.com/user-attachments/assets/1b54da96-abb3-49a7-97da-98de6bc55b46" />
<img width="630" height="59" alt="Screenshot 2025-10-20 173216" src="https://github.com/user-attachments/assets/8d402f1f-d5fa-4459-aabd-f3b3572d4552" />


## Result:
Thus, The Python program that checks whether a given number is a **palindrome** using loops is verified.
