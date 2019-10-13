package sample;
​
import java.util.Scanner;
​
public class MatrixTranspose {
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        System.out.print("Please enter number of rows: ");
        int row = scan.nextInt();
        System.out.print("Please enter number of columns: ");
        int column = scan.nextInt();
​
        int matrix[][] = new int[row][column];
        System.out.println("Enter the matrix elements: ");
        for(int i = 0; i < row; i++){
            for(int j = 0; j < column; j++){
                matrix[i][j] = scan.nextInt();
            }
        }
        System.out.println("Original matrix: ");
        for(int i = 0; i < row; i++){
            for(int j = 0; j < column; j++){
                System.out.print(matrix[i][j] + " ");
            }
            System.out.println(" ");
        }
        System.out.println("Matrix transpose: ");
        for(int i = 0; i < column; i++){
            for(int j = 0; j < row; j++){
                System.out.print(matrix[j][i] + " ");
            }
            System.out.println(" ");
        }
    }
}
