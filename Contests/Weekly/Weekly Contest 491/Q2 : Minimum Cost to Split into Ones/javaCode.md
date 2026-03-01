```java
class Solution {
    public int minCost(int x,int[] ans){
        if(x==0 || x==1) return 0;

        int a = x/2;
        int b = x-a;

        ans[0] += a*b;
        return minCost(a,ans) + minCost(b,ans);
    }
    
    public int minCost(int n) {
        // int[] ans = new int[1];
        // minCost(n,ans);
        // return ans[0];
        int cost = n*(n-1)/2;
        return cost;
    }
}
