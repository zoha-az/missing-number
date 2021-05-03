# missing-number
# Given an array nums containing n distinct numbers in the range [0, n], return the only number in the range that is missing from the array.
class Solution:
    def missingNumber(self, nums: List[int]) -> int:
    
        # receiving the length of the array
        
        l=len(nums)
        
        # creating a new list containing all the required numbers
        
        new=list(range(0,l+1))
        
        # comparing the expected array with input array
        
        for i in new:
            if i not in nums:
                return i
