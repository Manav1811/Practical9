# Practical9
package part1;
import java.util.*;
public class Practical9 {
	
    public static void main(String[] args) {
        int[][] arr1={{5,3,4,6,7,8,9,1,2},
                      {6,7,2,1,9,5,3,4,8},
                      {1,9,8,3,4,2,5,6,7},
                      {8,5,9,7,6,1,4,2,3},
                      {4,2,6,8,5,3,7,9,1},
                      {7,1,3,9,2,4,8,5,6},
                      {9,6,1,5,3,7,2,8,4},
                      {2,8,7,4,1,9,6,3,5},
                      {3,4,5,2,8,6,1,7,9}};
        for(int k=0;k<9;k++)
        {
            for(int l=0;l<9;l++)
            {
                System.out.print(arr1[k][l]+ " ");
            }
            System.out.println('\n');
        }
        int row=0,col=0;
        int sum = 0;
        int ans = 0;
       for( row=0;row<9;row++) {
           sum=0;
           ans=0;
           for( col=0;col<9;col++) {

               sum=sum+arr1[row][col];
               ans=ans+arr1[col][row];

           }
           if(sum!=45 || ans != 45)
           {
               System.out.println("Incorrect answer");
               break;
           }

       }
       if(row==9 && col ==9){
           System.out.println("Correct answer ");
       }

   	//Created by Manav_21CE063.
       
    }
}


