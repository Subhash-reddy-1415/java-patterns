# Letter Q Pattern in Java



`Q.java`

---

## 💻 Code

```java
public class Q {
    public static void main(String[] args) {
        int n = 10; // size of the letter

        for (int i = 0; i <= n; i++) { // rows
            for (int j = 0; j <= n; j++) { // columns
                if ((i == 0 && j > 0 && j < n) ||           // top border
                    (i == n && j > 0 && j < n) ||           // bottom border
                    (j == 0 && i > 0 && i < n) ||           // left border
                    (j == n && i > 0 && i < n) ||           // right border
                    (i == j && i > n/2)) {                  // diagonal tail
                    System.out.print("* ");
                } else {
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}
```

---

## ✅ Sample Output (n = 10)

```
  * * * * * * * * *  
*                 * 
*                 * 
*                 * 
*                 * 
*                 * 
*                 * 
*                 * 
*                 * 
  * * * * * * * * *  
                    * 
                      * 
```

---

## ⚙️ Explanation

* **`i == 0` and `i == n`** → draw top and bottom borders.
* **`j == 0` and `j == n`** → draw left and right borders.
* **`i == j && i > n/2`** → adds the diagonal line that forms the **Q tail**.

This creates the letter **Q**.

---

## 🎯 Usage

1. Save the file as `Q.java`.
2. Compile with:

   ```bash
   javac Q.java
   ```
3. Run with:

   ```bash
   java Q
   ```

The output will display the **letter Q** pattern in the console.
