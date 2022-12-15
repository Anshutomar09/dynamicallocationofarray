# dynamicallocationofarray

#include <iostream>

using namespace std;
 
int getsum(int *arr, int m){
    int sum;
    for(int i=0;i<m;i++){
        sum += arr[i];
    }
    return sum;
} 
 
int main()
{
    int n;
    cin>>n;
    int *arr= new int[n];
    for(int i=0;i<n;i++){
        cin>>arr[i];
    }
    int ans=getsum(arr,n);
    for(int i=0;i<n;i++){
        cout<<ans;
    }

    return 0;
}
