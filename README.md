# Finahub PlayGround
Repository for some coding experiments, assessment and hiring
class ABC{
static String censor(String text,String word)
{
String[] word_list=text.split("\\s+");
String result="";
String hash="";
for(int i=0;i<word.length();i++)
hash='#';
int index=0;
for(String i:word_list)
{
if(i.compareTo(word)==0)
word_list[index]=hash;
index++;
}
for(String i: word_list)
result+=i+'';
return result;
}
public static void main(string[] args)
{
String extract="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum";
String cen="consectetur adipiscing elit";
system.out.println(censor(extract, cen));
}
}
