# Using-Sorting-techiniques
#include <stdio.h> 

#include <stdlib.h> 

int main() 

{int n,k,a[20]; 

printf("enter number of elements in the array:"); 

scanf("%d",&n); 

printf("\nenter the elements in the array:\n"); 

for(int i=0;i<n;i++) 

{ 

  scanf("%d",&a[i]); 

} 

int m, j,temp; 

   for (m = 0; m < n-1; m++) 

       { 

          for (j = 0; j < n-m-1; j++) 

          { 

              if (a[j] > a[j+1]) 

              {   temp=a[j]; 

                  a[j]=a[j+1]; 

                  a[j+1]=temp; 

              } 

          } 

       } 

printf("\n enter the kth smallest element to find:"); 

scanf("%d",&k); 

printf("%d",a[k-1]); 

}
