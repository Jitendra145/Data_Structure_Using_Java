```
import java.util.*;
import java.lang.*;
import java.io.*;
 
/* Name of the class has to be "Main" only if the class is public. */
class Ideone
{
	public static void main (String[] args) throws java.lang.Exception
	{
		// your code goes here
		int ar [] = new int[]{2,5,10,9,3};
		for(int i=0;i<5;i++){
			for(int j=0;j<i;j++){
				if(ar[j]>ar[i]){
					for(int k=i;k>j;k--){
					int tmp = ar[k];
					ar[k] = ar[k-1];
					ar[k-1] = tmp;
					}
				}
			}
		}
		for(int i=0;i<5;i++){
			System.out.println(ar[i]);
		}
	}
}
```
