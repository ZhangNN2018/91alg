##  【Day 19】两数之和

https://leetcode-cn.com/problems/two-sum/

* [题目描述](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%205%E3%80%91232.%20%E7%94%A8%E6%A0%88%E5%AE%9E%E7%8E%B0%E9%98%9F%E5%88%97.md#%E9%A2%98%E7%9B%AE%E6%8F%8F%E8%BF%B0)
* [方法](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%205%E3%80%91232.%20%E7%94%A8%E6%A0%88%E5%AE%9E%E7%8E%B0%E9%98%9F%E5%88%97.md#%E6%96%B9%E6%B3%95)
     * [思路](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%205%E3%80%91232.%20%E7%94%A8%E6%A0%88%E5%AE%9E%E7%8E%B0%E9%98%9F%E5%88%97.md#%E6%80%9D%E8%B7%AF)
     * [复杂度](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%205%E3%80%91232.%20%E7%94%A8%E6%A0%88%E5%AE%9E%E7%8E%B0%E9%98%9F%E5%88%97.md#%E5%A4%8D%E6%9D%82%E5%BA%A6)
     * [代码](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%205%E3%80%91232.%20%E7%94%A8%E6%A0%88%E5%AE%9E%E7%8E%B0%E9%98%9F%E5%88%97.md#%E4%BB%A3%E7%A0%81)
* [特别注意](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%205%E3%80%91232.%20%E7%94%A8%E6%A0%88%E5%AE%9E%E7%8E%B0%E9%98%9F%E5%88%97.md#%E7%89%B9%E5%88%AB%E6%B3%A8%E6%84%8F)

### 题目描述
    给定一个整数数组 nums 和一个整数目标值 target，请你在该数组中找出 和为目标值 target  的那 两个 整数，并返回它们的数组下标。
    你可以假设每种输入只会对应一个答案。但是，数组中同一个元素在答案里不能重复出现。
    你可以按任意顺序返回答案。

    示例 1：
    输入：nums = [2,7,11,15], target = 9
    输出：[0,1]
    解释：因为 nums[0] + nums[1] == 9 ，返回 [0, 1] 。
    
    示例 2：
    输入：nums = [3,2,4], target = 6
    输出：[1,2]
    
    示例 3
    输入：nums = [3,3], target = 6
    输出：[0,1]

    提示：
    2 <= nums.length <= 104
    -109 <= nums[i] <= 109
    -109 <= target <= 109
    只会存在一个有效答案
    进阶：你可以想出一个时间复杂度小于 O(n2) 的算法吗？

    来源：力扣（LeetCode）
    链接：https://leetcode-cn.com/problems/two-sum
    著作权归领扣网络所有。商业转载请联系官方授权，非商业转载请注明出处。
### 方法

#### 思路
* 两层for循环遍历

#### 复杂度
* 时间复杂度: `O(N^2)`
* 空间复杂度: `O(1)`

#### 代码
```python
class Solution(object):
    def twoSum(self, nums, target):
        """
        :type nums: List[int]
        :type target: int
        :rtype: List[int]
        """
        '''
        for i in range(len(nums)):
            for j in range(i+1,len(nums)):
                sumij=nums[i]+nums[j]
                if sumij == target:
                    return [i,j]
```
### 特别注意
* none
* 
