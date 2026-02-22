```java
class Solution {
    public String maximumXor(String s, String t) {
        long ones = 0;
        long zeros = 0;
        
        for(int i=0;i<t.length();i++){

            if(t.charAt(i)=='0') zeros++;
            else ones++;
        }

        StringBuilder sb = new StringBuilder();

        for(int i=0;i<s.length();i++){
            if(s.charAt(i)=='0'){
                if(ones>0){
                    sb.append('1');
                    ones--;
                }
                else{
                    sb.append('0');
                    zeros--;
                    
                }
            }
            else{
                if(zeros>0){
                    sb.append('1');
                    zeros--;
                }
                else{
                    sb.append('0');
                    ones--;
                }
            }
        }
        

        return sb.toString();
    }
}
