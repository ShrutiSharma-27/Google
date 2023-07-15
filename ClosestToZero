import java.io.*;
import java.util.*;


public class TestClass {
    public static void main(String[] args) throws IOException {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        PrintWriter wr = new PrintWriter(System.out);
        int N = Integer.parseInt(br.readLine().trim());
        int[] A = new int[N];
        String[] arr_A = br.readLine().split(" ");
        for(int i_A = 0; i_A < N; i_A++) {
        	A[i_A] = Integer.parseInt(arr_A[i_A]);
        }
        int out_ = Solve(N, A);
        System.out.println(out_);

         wr.close();
         br.close();
    }
    static int Solve(int N, int[] A){
        // Write your code here
        int prev_min = A[0];
        int min = A[0];
        int prev_diff = Math.abs(A[0]-0);
        for (int i=1 ; i<N ; i++){
            int diff = Math.abs(A[i]-0);
            if (diff < prev_diff){
                min = A[i];
            }
            else if (diff==prev_diff) {
                if(prev_min > A[i]) {
                    min=prev_min;
                }
                else{
                    min=A[i];
                }
            }
            prev_min = min;
            prev_diff = Math.abs(A[i]-0);
        }
        return min;
    }
}
