🖥️ README File (for this program)
Hollow Triangle Pattern in Java
📌 Description

This program prints a hollow right-angled triangle using asterisks (*).
It uses nested loops to align spaces and draw borders while leaving the inside hollow.

🖥️ Code
class Main {
    public static void main(String[] args) {
        for (int i = 1; i <= 5; i++) {
            // spaces
            for (int j = 5; j > i; j--) {
                System.out.print(" ");
            }

            // stars and spaces
            for (int j = 1; j <= i; j++) {
                if (i == 1 || i == 5 || j == 1 || j == i) {
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
* * * * * 

⚙️ How It Works

First inner loop → prints leading spaces.

Second inner loop → decides where to print stars.

Top & bottom rows → fully filled.

First & last positions in row → stars.

Inside → spaces.
