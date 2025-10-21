# PYTHON MODULE -2
# (D)🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

-------------

## 🎯 Aim:

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

## 🧠 Algorithm:

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

## 🧪 Program:

  
    def print_pascals_triangle_formula(num_rows):
   
        for n in range(num_rows):
            val = 1
            row_list = []
            for k in range(n + 1):
                 row_list.append(str(val))
                 val = val * (n - k) // (k + 1)
        
             row_str = " ".join(row_list)
             max_width = len(" ".join(map(str, [1] * num_rows)))
             print(row_str.center(max_width))

    n = int(input())
    print_pascals_triangle_formula(n)

## Output:

<img width="790" height="537" alt="Screenshot 2025-10-20 170612" src="https://github.com/user-attachments/assets/5a21a82f-fd70-4aac-95f7-43b4dbf16fa7" />


## Result:

Thus, The Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user was executed successfully.
