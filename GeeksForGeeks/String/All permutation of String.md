```
/* package whatever; // don't place package name! */

import java.util.*;
import java.lang.*;
import java.io.*;

/* Name of the class has to be "Main" only if the class is public. */
class Test
{
	public static void main (String[] args) throws java.lang.Exception
	{
		// your code goes here
		String str = "abc";
		permutation(str,0,2);
	}
	public static void permutation(String str,int l,int r){
		if(l==r){
			System.out.println(str);
		}else{
			for (int i = l; i <= r; i++)  
        	{
        	
				str=swap(l,i,str);
				permutation(str,l+1,r);
				str=swap(l,i,str);
    	  }
		}
	}
	public static String swap(int i,int j,String a){
		char temp; 
        char[] charArray = a.toCharArray(); 
        temp = charArray[i] ; 
        charArray[i] = charArray[j]; 
        charArray[j] = temp; 
        return String.valueOf(charArray); 
	}
}
```
