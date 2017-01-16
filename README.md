insertion sort <iostream>
using namespace std;
void insertionSort(int n, int * arr) 
{
 int temp,i,j,k;
 for(i=1;i<n;i++)
 {
 	
 	j=i;
 	while(j>0 && arr[j]<arr[j-1])
 	{
 		temp=arr[j];
 		arr[j]=arr[j-1];
 		arr[j-1]=temp;
 		j--;
 		 for(k=0;k<n;k++)
                  cout<<arr[k]<<" ";
              cout<<endl;
 		
 	}
}
}
int main()
{
    int n;
    cin>>n;
    int arr[n];
    for(int i=0;i<n;i++)
        {
        cin>>arr[i];
        }
    insertionSort(n,arr);
   return 0;
}
