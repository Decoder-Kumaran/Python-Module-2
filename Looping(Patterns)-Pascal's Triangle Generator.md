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

def print_pascals_triangle(num_rows):
    
    triangle = []
    
    for i in range(num_rows):
    
        row = [1] * (i + 1)
        
        if i > 1:
        
            prev_row = triangle[-1]
            
            for j in range(1, i):
                row[j] = prev_row[j-1] + prev_row[j]
        
        triangle.append(row)
        
    
    # Print the formatted triangle
    
    max_width = len(" ".join(map(str, triangle[-1])))
    
    for row in triangle:
    
        row_str = " ".join(map(str, row))
        
        print(row_str.center(max_width))


n = int(input("Enter the number of rows for Pascal's Triangle: "))

print_pascals_triangle(n)


## Output:



## Result:

Thus, The Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user is verified.
