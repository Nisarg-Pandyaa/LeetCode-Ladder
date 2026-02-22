```java
class Solution {
    public int scoreDifference(int[] nums) {
        int n = nums.length;
        int p1 = 0; boolean flag = true;
        int p2 = 0;
        int sixGame =5;
        
        for(int i = 0;i<n;i++){
            if(nums[i]%2!=0){
                flag = !flag;
            }

            if(i==sixGame){
                flag = !flag;
                sixGame += 6;
            }

            if(flag) p1+=nums[i];
            else p2 += nums[i];
        }
        return p1-p2;
    }
}
