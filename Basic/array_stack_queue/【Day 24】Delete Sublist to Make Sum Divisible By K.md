
##  【Day 24】Delete Sublist to Make Sum Divisible By K

https://binarysearch.com/problems/Delete-Sublist-to-Make-Sum-Divisible-By-K

* [题目描述](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%205%E3%80%91232.%20%E7%94%A8%E6%A0%88%E5%AE%9E%E7%8E%B0%E9%98%9F%E5%88%97.md#%E9%A2%98%E7%9B%AE%E6%8F%8F%E8%BF%B0)
* [方法](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%205%E3%80%91232.%20%E7%94%A8%E6%A0%88%E5%AE%9E%E7%8E%B0%E9%98%9F%E5%88%97.md#%E6%96%B9%E6%B3%95)
     * [思路](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%205%E3%80%91232.%20%E7%94%A8%E6%A0%88%E5%AE%9E%E7%8E%B0%E9%98%9F%E5%88%97.md#%E6%80%9D%E8%B7%AF)
     * [复杂度](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%205%E3%80%91232.%20%E7%94%A8%E6%A0%88%E5%AE%9E%E7%8E%B0%E9%98%9F%E5%88%97.md#%E5%A4%8D%E6%9D%82%E5%BA%A6)
     * [代码](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%205%E3%80%91232.%20%E7%94%A8%E6%A0%88%E5%AE%9E%E7%8E%B0%E9%98%9F%E5%88%97.md#%E4%BB%A3%E7%A0%81)
* [特别注意](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%205%E3%80%91232.%20%E7%94%A8%E6%A0%88%E5%AE%9E%E7%8E%B0%E9%98%9F%E5%88%97.md#%E7%89%B9%E5%88%AB%E6%B3%A8%E6%84%8F)

### 题目描述
    You are given a list of positive integers nums and a positive integer k. Return the length of the shortest sublist (can be empty sublist ) you can delete such that the resulting list's sum is divisible by k. You cannot delete the entire list. If it's not possible, return -1.

    Constraints
    1 ≤ n ≤ 100,000 where n is the length of nums

### 方法

#### 思路
* 前缀和+同余定理
https://leetcode-solution.cn/solutionDetail?type=3&id=24&max_id=2

#### 复杂度
* 时间复杂度: `O(n)`
* 空间复杂度: `O(min(n,k))`

#### 代码
```python
class Solution:
    def solve(self, nums, k):
        #先计算出总体的数组和 total 模 k 的余数，记为 target，那么我们的目标就是找到一段模 k 等于 target 的子数组

        total = sum(nums) #求和
        mod = total % k #求余数

        ans = len(nums) 
        total = 0
        dic = {0: -1} #用来最新的余数对应的下标
        for j in range(len(nums)): #遍历nums
            total += nums[j] #当前总和
            cur = total % k #当前的余数
            target = (cur - mod + k) % k 
            if target in dic:
                ans = min(ans, j - dic[target])
            dic[cur] = j

        if ans == len(nums):
            return -1
        return ans       
```
### 特别注意
* 前缀和
