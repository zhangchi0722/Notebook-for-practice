#Leetcode.01
#该提问题为：给定一个整数数组 nums 和一个整数目标值 target，
#请你在该数组中找出 和为目标值 target的两个整数，并返回它们的数组下标。
#你可以假设每种输入只会对应一个答案，并且你不能使用两次相同的元素。
#你可以按任意顺序返回答案。
''' 示例 1：
输入：nums = [2,7,11,15], target = 9
输出：[0,1]
解释：因为 nums[0] + nums[1] == 9 ，返回 [0, 1] 。'''


#以下是我经豆包修改后给出的答案：
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        for i in range(len(nums)):
            for k in range(i+1,len(nums)):
                if nums[i] + nums[k] == target:
                    return [i,k]


