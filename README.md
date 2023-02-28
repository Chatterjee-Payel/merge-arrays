# merge-arrays
	
class Solution{
	public:
	void sortedMerge(int a[], int b[], int res[],int n, int m)
	{
	   // Your code goes here
	    for(int i=0;i<n;i++){
	        res[i]=a[i];
	    }
	    int j=0;
	    for(int i=n;i<m+n;i++){
	        res[i]=b[j];
	        j++;
	    }
	    sort(res,res+(n+m));
	}
};
