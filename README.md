//Program for Bubblesort
//Input:Enter number of elements:5
//Enter elements:45 23 78 9 10
//Output:Sorted list in ascending order: 9 10 23 45 78
#include <stdio.h>
void main()
{
    int a[10],n,i,j,temp;
    printf("Enter the value of n");
    scanf("%d",&n);
    printf("Enter the array elements");
    for(i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    for(i=0;i<n-1;i++)
    {
        for(j=0;j<n-1-i;j++)
        {
            if(a[j]>a[j+1])
            {
                temp=a[j];
                a[j]=a[j+1];
                a[j+1]=temp;
            }
        }
    }
    printf("Sorted list in ascending order:");
    for(i=0;i<n;i++)
    {
        printf("  %d",a[i]);
    }

}
