```java
class Solution {
    public boolean isPermutation(long sum, int[] freq, int len){
        if(sum<=0) return false;

        int[] sumCount = new int[10];
        int sumLength = 0;
        long temp = sum;

        while(temp>0){
            sumCount[(int)temp%10]++;
            sumLength++;
            temp /= 10;
        }

        if(sumLength!=len) return false;

        for(int i=0;i<10;i++){
            if(sumCount[i]!=freq[i]) return false;
        }
        return true;
    }
    public int factorial(int n){
        int[] facto = {1,1,2,6,24,120,720,5040,40320,362880};
        return facto[n];
    }
    public boolean isDigitorialPermutation(int n) {
        long digitFactoSum = 0;
        int og = n;
        int[] digitFreq = new int[10];
        int len = 0;
        while(og>0){
            digitFreq[og%10]++;
            digitFactoSum += factorial(og%10);
            
            og /= 10;
            len++;
        }
        
        
        return isPermutation(digitFactoSum,digitFreq,len);
    }
}


// We only deals with digits<10 (iykyk)
