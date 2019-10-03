class Solution {
    public void rotate(int[] nums, int k) {
    
        //If k is multiple of array's length, then resulting array will always be same
        if(k%nums.length == 0){
            return;
        }
        
       //If k is greater than array's length, ten reducing k as rotaion of array by its length results in same array
         while(k>nums.length){
            k = k%nums.length;
        }
        
        //Reverse array function
        reverse(nums,0,nums.length-1-k);
		    reverse(nums, nums.length-k, nums.length-1);
		    reverse(nums, 0, nums.length-1);
    }
    
	private static void reverse(int[] nums, int i, int j) {
		while(i<j) {
			swap(nums,i,j);
			i++;
			j--;
		}
		
	}

	private static void swap(int[] nums, int i, int j) {
     	int temp = nums[i];
		nums[i] = nums[j];
		nums[j] = temp;	
	}
}
