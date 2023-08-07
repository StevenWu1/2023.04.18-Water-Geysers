import java.io.*;
import java.util.*;

public class Solution {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int geyser[] = new int[n];
        for (int i = 0; i < n; i++){
            geyser[i] = sc.nextInt();
        }
        int ans = 0;
        for (int i = 0; i < (geyser.length - 1); i++){
            boolean increase = (geyser[i] < geyser[i+1]);
            for (int j = i + 1; j < geyser.length; j++){
                if (increase){
                    if (geyser[j] <= geyser[j-1]){
                        int maybeAns = Math.abs(geyser[j-1] - geyser[i]);
                        if (maybeAns > ans){
                            ans = maybeAns;
                            i = j-1;
                        }
                        break;
                    }
                    if (j == (geyser.length - 1)){
                        int maybeAns = Math.abs(geyser[j] - geyser[i]);
                        if (maybeAns > ans){
                            ans = maybeAns;
                        }
                        break;
                    }
                } else {
                    if (geyser[j] >= geyser[j-1]){
                        int maybeAns = Math.abs(geyser[j-1] - geyser[i]);
                        if (maybeAns > ans){
                            ans = maybeAns;
                            i = j-1;
                        }
                        break;
                    }
                    if (j == (geyser.length - 1)){
                        int maybeAns = Math.abs(geyser[j] - geyser[i]);
                        if (maybeAns > ans){
                            ans = maybeAns;
                        }
                        break;
                    }
                }
            }
        }
        System.out.println(ans);
    }
}
