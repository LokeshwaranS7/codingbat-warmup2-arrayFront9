# codingbat-warmup2-arrayFront9
Given an array of ints, return true if one of the first 4 elements in the array is a 9. The array length may be less than 4.


arrayFront9([1, 2, 9, 3, 4]) → true
arrayFront9([1, 2, 3, 4, 9]) → false
arrayFront9([1, 2, 3, 4, 5]) → false
    
    public boolean arrayFront9(int[] nums) {
    int h=0;
    int n=nums.length;
     if (n>=4) n=4;
     boolean flag=false;
     while(h<n)
     {
      if(nums[h]==9)
      {
       flag=true;
        break;
    
     }
     else
     { 
        if(h>=n) 
        {
        flag=false;
       }
        else
        {
          h+=1;
        }
      }
    
    }
    if(flag==true) return true;
    else return false;

    }
