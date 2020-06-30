//matrixaddn
//Program to add  two matrices

package matrixaddn;

public class matrixaddn {
    
    public static void main(String[] args) {
    
        int rows = 3, columns = 3;
        
        // Declaring the two matrices as multi-dimensional arrays
        int [][] a = { {1,3,4},{2,4,3},{3,4,5} };
        int [][] b = { {1,3,4},{2,4,3},{1,2,4} };
        
        
        int[][] sum = new int[rows][columns];
        for(int i = 0; i < rows; i++) {
            for (int j = 0; j < columns; j++) {
                sum[i][j] = a[i][j] + b[i][j];
            }
        }
        
        for(int i = 0; i < rows; i++) {
            for (int j = 0; j < columns; j++) {
                System.out.print(sum[i][j] + " ");
            }
            System.out.println();
        }
    }
}

OUTPUT=>

2 6 8 
4 8 6 
4 6 9 
