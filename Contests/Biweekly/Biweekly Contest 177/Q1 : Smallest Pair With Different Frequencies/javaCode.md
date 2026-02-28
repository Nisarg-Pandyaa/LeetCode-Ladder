```java
class Solution {
    public int[] minDistinctFreqPair(int[] nums) {

        int[] freq = new int[101];

        for(int n : nums) freq[n]++;

        int[] pair = {-1,-1};

        for(int i=1;i<101;i++){
            if(freq[i]!=0){
                if(pair[0]!=-1){
                    if(freq[i]==freq[pair[0]]){
                        continue;
                    }else{
                        pair[1] = i;
                        return pair;
                    }
                }
                else{
                    pair[0]=i;
                }
            }
        }
        if(pair[1]==-1) pair[0]=-1;
        return pair;        
    }
}
