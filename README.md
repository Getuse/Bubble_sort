# Bubble_sort
Bubble Sorting is an one of the way to sort an array elements in O(n^2) time complexity


#include<iostream>
using namespace std;

void Bubble_sort(int arr[],int n)
{
     for(int i=0;i<n-1;i++)
     {
       for(int j=0;j<n-1-i;j++)
       {  
         if(arr[j]>arr[j+1])
         {  
            int temp = arr[j];
            arr[j] = arr[j+1];
            arr[j+1] = temp;
            
          }
          }
     }
}
void print(int arr[],int n)
{
 for(int i=0;i<n;i++){
 cout<<arr[i]<<" ";
}
}


int main()
{
  int n ;
  cout<<"Enter array length"<<endl;
  cin>>n;
  int arr[n];
  cout<<"enter array Elements :"<<endl;
  for(int i=0;i<n;i++)
  {
    cin>>arr[i];
  }
  Bubble_sort(arr,n);
  print(arr,n);
  
  return 0;
}
