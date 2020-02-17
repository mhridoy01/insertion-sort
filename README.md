# insertion-sort
#cse2026,Rb,lecture-2(17february2020)


#include<bits/stdc++.h>
using namespace std;
void insertion_sort(int a[],int s)
{
    for(int i=1;i<=s;i++)
    {
        int k=i;
        while(k>1 && a[k]<a[k-1])
        {
            swap(a[k],a[k-1]);
            k--;
        }
    }

}
int main()
{
    int arr[100],n;
    scanf("%d",&n);
    for(int i=1;i<=n;i++)
       scanf("%d",&arr[i]);
       insertion_sort(arr,n);
       for(int i=1;i<=n;i++)
        printf("%d ",arr[i]);
       return 0;
}
