int subarraySum(int* nums, int numsSize, int k) {
   int i,j,cnt=0;
   for (i=0;i<numsSize;i++){
    int sum=0;
    for(j=i;j<numsSize;j++){
        sum+=nums[j];
        if(sum==k){
            cnt++;
        }
    }
   } 
   return cnt;
}