# Matrix Operations Implemented in C
## Why I Built This
I wanted to deepen my understanding of mathematics while also preparing for my **C programming final**. Additionally, this tool allows me to create practice sheets for myself and my classmates, making it easier for all of us to get ready for exams. Some functions also let the user generate an answer key or directly compute the answer.
## Functions (Planned)
- Summation  
- Difference  
- Multiplication (matrix × matrix, matrix × scalar)  
- Determinant  
- Determining if a matrix is singular or regular  
- Inverse of a matrix  
- Gauss–Jordan elimination  
- Solving systems of equations with matrices  
## Matrix Generation Options
Generated files are usable with the web application [Typst](https://typst.app). Users can directly insert the output into a Typst file.  
**Supported types:**  
- Regular n×n random matrix  
- Upper/lower triangular matrix  
- Identity (I) matrix  
- Row/column matrix  
## How to Use
### Input Format
The user needs to provide matrices in the following formats (for both console and files):  
`.typ` files are exceptions – leave them as written.  
**Example for an n×n matrix:**
```c
[[a,b,c],[d,e,f],[g,h,i]]
Example for a row matrix:

c
Kód másolása
l [a,b,c]
Example for a column matrix:

c
Kód másolása
r [a,b,c]
Operations (Console and .txt)
Note: Invalid input will result in a single error message.

Sum
c
Kód másolása
[[a,b,c],[d,e,f]] + [[g,h,i],[j,k,l]] 
# Output: Either the sum or an error message
Difference
c
Kód másolása
[[a,b,c],[d,e,f]] - [[g,h,i],[j,k,l]] 
# Output: Either the difference or an error message
Singular or Regular
c
Kód másolása
isSingOrReg([[a,b,c],[d,e,f]]) 
# Output: "singular" or "regular"
Determinant
c
Kód másolása
det([[a,b,c],[d,e,f]]) 
# Output: A number
Inverse
c
Kód másolása
inv([[a,b,c],[d,e,f]]) 
# Output: Matrix in the same format, e.g., [[a,b,c],[d,e,f]]
Gauss–Jordan Elimination
c
Kód másolása
rref([[a,b,c],[d,e,f]]) 
# Output: Reduced Row Echelon Form
# Example:
rref([[1,2,3],[4,5,6],[7,8,9]]) -> [[1,0,-1],[0,1,2],[0,0,0]]
Solving Systems of Equations
Use augmented matrix (last column is constants):

c
Kód másolása
solve([[1,1,1,6],[2,3,7,20],[1,-1,1,2]]) 
# Output (console): [x=1, y=2, z=3]
# Output (Typst): [[1],[2],[3]]
Notes
The project is designed to reinforce mathematical understanding and C programming fundamentals.

Outputs are Typst-compatible, making it easy to generate clean and structured documents.

Future Improvements
Add file I/O error handling

Extend Typst output templates

Optimize computation for larger matrices

Add color-coded console output for readability

Tech Stack
Language: C

Output Integration: Typst
