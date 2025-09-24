🖥️ README File for Hollow Diamond
Hollow Diamond Pattern in Java
📌 Description

This program prints a hollow diamond (rhombus) pattern using asterisks (*).
It uses nested loops to handle spaces, borders, and symmetry between the top and bottom halves.

🖥️ Code Example
public class Pp {
    public static void main(String[] args) {
        // Upper triangle
        for(int i = 1; i <= 5; i++) {
            for(int j = 5 ;j >= i;j--) {
                System.out.print(" ");
            }  
            for(int j = 1;j<=i;j++) {
                if(i == 1 || i == j || j == 1 || j == 5) {
                    System.out.print("* ");
                } else {
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
        
        // Lower triangle
        for(int i = 2; i <= 5; i++) {
            for(int j = 1 ;j <=  i;j++) {
                System.out.print(" ");
            }  
            for(int j = 5;j >= i;j--) {
                if( i == j || j == 1 || j == 5) {
                    System.out.print("* ");
                } else {
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

🎯 Output
     * 
    * * 
   *   * 
  *     * 
 *       * 
  *     * 
   *   * 
    * * 
     * 

⚙️ How It Works

The first loop prints the upper hollow triangle.

The second loop prints the lower hollow inverted triangle.

Borders (j == 1, i == j, or j == max) print *, while the inside is left as spaces.
🔍 Explanation of Code
First Half → Top Pyramid
for(int i = 1; i <= 5; i++) {
    // leading spaces
    for(int j = 5 ;j >= i;j--) {
        System.out.print(" ");
    }  
    // stars and hollow
    for(int j = 1;j<=i;j++) {
        if(i == 1 || i == j || j == 1 || j == 5) {
            System.out.print("* ");
        } else {
            System.out.print("  ");
        }
    }
    System.out.println();
}


Prints the upper hollow triangle.

Spaces align the stars.

Stars are placed at borders (first column, last column, diagonal edges).

Second Half → Inverted Pyramid
for(int i = 2; i <= 5; i++) {
    // leading spaces
    for(int j = 1 ;j <=  i;j++) {
        System.out.print(" ");
    }  
    // stars and hollow
    for(int j = 5;j >= i;j--) {
        if( i == j || j == 1 || j == 5) {
            System.out.print("* ");
        } else {
            System.out.print("  ");
        }
    }
    System.out.println();
}


Prints the lower hollow triangle.

Starts from row 2 (to avoid repeating the middle row).

Again prints stars only on borders.

✅ Output
     * 
    * * 
   *   * 
  *     * 
 *       * 
  *     * 
   *   * 
    * * 
     * 


That’s a hollow diamond pattern.
