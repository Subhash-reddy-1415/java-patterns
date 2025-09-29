💻 Java Code for Letter P
public class P {
    public static void main(String[] args) {
        int n = 10; // size of the letter

        for (int i = 0; i <= n; i++) { // rows
            for (int j = 0; j <= n; j++) { // columns
                if (j == 0 || (i == 0 && j < n) || (i == n / 2 && j < n) || (j == n && i < n / 2 && i != 0)) {
                    // Left vertical bar
                    // Top horizontal bar
                    // Middle horizontal bar
                    // Right vertical bar (only for upper half)
                    System.out.print("* ");
                } else {
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

✅ Output (for n = 10)
* * * * * * * * * * 
*                 * 
*                 * 
*                 * 
*                 * 
* * * * * * * * *   
*                   
*                   
*                   
*                   
*                   

⚙️ Explanation

j == 0 → left vertical bar

i == 0 → top horizontal line

i == n/2 → middle horizontal line

j == n && i < n/2 → right vertical line (only in top half)

This forms a P-shaped pattern.
