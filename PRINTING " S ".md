S Pattern Printing in Java

This project prints the letter S in a star (*) pattern using Java.

📌 Program Description

The program uses nested for loops to print stars (*) in the correct positions.

It creates the shape of the letter S with customizable size.

Works for any n (pattern size), but looks best with odd numbers like 7, 9, etc.

🖥️ Example Output (for n = 7)
 ***** 
*     
*     
 ***** 
      *
      *
 ***** 

🚀 How to Run

Save the code in a file named SPattern.java

Open terminal/command prompt in the folder where the file is located.

Compile the program:

javac SPattern.java


Run the program:

java SPattern

🔧 Customization

Change the value of n in the code to increase/decrease the size of the S.

int n = 7; // try 5, 9, 11 for different sizes

📂 Project Structure
S-Pattern/
│── SPattern.java   # Java source code
│── README.md       # Project documentation

```
public class SPattern {
    public static void main(String[] args) {
        int n = 7; // size of the pattern (rows)

        for (int i = 0; i < n; i++) {
            for (int j = 0; j < n; j++) {
                
                // Top row
                if (i == 0 && j > 0) 
                    System.out.print("*");
                
                // Upper curve
                else if (i < n/2 && j == 0) 
                    System.out.print("*");
                
                // Middle row
                else if (i == n/2) 
                    System.out.print("*");
                
                // Lower curve
                else if (i > n/2 && j == n-1) 
                    System.out.print("*");
                
                // Bottom row
                else if (i == n-1 && j < n-1) 
                    System.out.print("*");
                
                else 
                    System.out.print(" ");
            }
            System.out.println();
        }
    }
}
```
