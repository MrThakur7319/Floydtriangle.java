# Floydtriangle.java
public class FloydTriangle{
  
  /**
   * Main method - entry point of the program
   * @param args command line arguments (not used)
   */
  public static void main(String [] args){
    
   // Number of rows in Floyd's triangle
    int n = 5;
    
   // Counter for consecutive numbers starting from 1
    int num = 1;
    
   // Outer loop: controls the number of rows (1 to n)
    // Each iteration represents one row of the triangle
    for(int i = 1; i <= n; i++) {
      
  // Inner loop: prints numbers for current row
      // Row number determines how many numbers to print
      // Row 1: 1 number, Row 2: 2 numbers, Row 3: 3 numbers, etc.
      for(int j = 1; j <= i; j++){
        System.out.print(num + " "); // Print current number followed by space
        num++; // Increment to next consecutive number
      }
      
   // Move to next line after completing current row
      System.out.println();
    }
  }
}
