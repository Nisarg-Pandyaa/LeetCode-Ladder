```java
class Solution {
    public String mergeCharacters(String s, int k) {
        StringBuilder sb = new StringBuilder();
        int i =0;
        HashMap<Character,Integer> hm = new HashMap<>();
        int n = s.length();
        
        while(i<n){
            char ch = s.charAt(i);
            if(hm.containsKey(ch)){
                int idx = hm.get(ch);
                if(sb.length()-idx<=k){
                    i++;
                    continue;
                }
            }

            sb.append(ch);
            hm.put(ch,sb.length()-1);
            i++;
        }
        
        return sb.toString();
    }
}
