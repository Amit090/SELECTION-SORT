# SELECTION-SORT

/******************************************************************************

                            Online Java Compiler.
                Code, Compile, Run and Debug java program online.
Write your code in this editor and press "Run" button to execute it.

*******************************************************************************/

public class Main
{


	public static void main(String[] args) {
		System.out.println("Hello World");
		
		int a[]= {10, 9, 7, 101, 23, 44, 12, 78, 34, 23};  
		int pos,temp=0;
		for(int i=0;i<10;i++)
		{
		    pos=smallest(a,10,i);
		    temp = a[i];  
            a[i]=a[pos];  
            a[pos] = temp; 
		}
		for(int i=0;i<10;i++)
		{
		    System.out.println(a[i]);
		}
	}
    public static int smallest(int a[],int n,int i)
      {
        int pos=i;
        int small=a[i];
        for(int j=i+1;j<n;j++)
        {
          if(small>a[j])
          {
              small=a[j];
              pos=j;
          }
         }
    return pos;
}

    
}

