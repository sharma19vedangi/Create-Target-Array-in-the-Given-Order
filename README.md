# Create-Target-Array-in-the-Given-Order
#Array Leetcode Problem Solution
class Solution {
    public int[] createTargetArray(int[] nums, int[] index) {
    List ans=new ArrayList();
     for(int i=0;i<index.length;i++) {
         ans.add(index[i],nums[i]);
        }
     for(int i=0;i<index.length;i++) {
         nums[i]= (int)ans.get(i);
         }
      return nums;
    }
}
