# GoogleFoobar
my attempts at the Foobar challenge questions

#1 
public class Answer {
    public static String answer(String s) {
        char[] charArray = s.toCharArray();
        StringBuilder sb = new StringBuilder(s.length());
        for (int i = 0; i < s.length(); ++i) {
            char temp = charArray[i];
            if (Character.isLowerCase(temp)) {
                int numValue = 123 - ((int)temp - 96);
                sb.append((char)numValue) ;
            }
            else { sb.append(temp); }
        }
        return sb.toString();
    }
