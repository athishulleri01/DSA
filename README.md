# DSA
## _placement preparation_


   ### 1.  [Two Sum](https://leetcode.com/problems/two-sum/description/) - 
My approach or brute force approach:

```python
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
       for i in range(len(nums)-1):
            for j in range(i+1,len(nums)):
                if nums[i]+nums[j] == target :
                    return [i,j]
```
**Time Complexity : 0(n)^2^**
**Space Complexity : 0(n)**

Best Approach:
```python
class Solution(object):
    def twoSum(self, nums, target):
        seen = {}
        for i in range(len(nums)):
            diff = target - nums[i]
            if diff in seen:
                return [seen[diff], i]
            else:
                seen[nums[i]] = i
```

**Time Complexity : 0(n)**
**Space Complexity : 0(n)**

[![alt text](https://img.youtube.com/vi/video-id/0.jpg)](https://youtu.be/dRUpbt8vHpo?si=ORy5I438ePzSUkX5)

