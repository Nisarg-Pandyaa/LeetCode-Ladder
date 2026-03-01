```java
class Solution {
    public String trimTrailingVowels(String s) {
        int i = 0;
        int tv = 0;
        StringBuilder sb = new StringBuilder();
        int n = s.length()-1;
        char lastChar = ' ';
        while(n>=0 && (s.charAt(n)=='a' || s.charAt(n)=='e' || s.charAt(n)=='i' || s.charAt(n)=='o' || s.charAt(n)=='u')){
            n--;
        }
        if(n==-1) return "";
        sb.append(s.substring(0,n+1));
        return sb.toString();
    }
}
