# Minimum-Number
public class Minimum{  
public static int getMinimum(int[] a, int total){  
int temp;  
for (int i = 0; i < total; i++)   
        {  
            for (int j = i + 1; j < total; j++)   
            {  
                if (a[i] > a[j])   
                {  
                    temp = a[i];  
                    a[i] = a[j];  
                    a[j] = temp;  
                }  
            }  
        }  
       return a[0];  
}  
public static void main(String args[]){  
int a[]={6,1,5,7,3,9};  
int b[]={56,35,60,76,94,26,89,49,};  
System.out.println("Minimum: "+getMinimum(a,6));  
System.out.println("Minimum: "+getMinimum(b,7));  
}}
