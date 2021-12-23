# 91alg
第6期（2021.12.12-2022.3.12）

|基础篇|专题篇|进阶篇|
|------|-----|------|
|[数组、栈、队列](https://github.com/ZhangNN2018/91alg#%E6%95%B0%E7%BB%84%E6%A0%88%E9%98%9F%E5%88%97)  |二分     |Trie|
|链表           |滑动窗口 |并查集|
|树             |搜索    |剪枝|
|哈希表         |动态规划 |字符串匹配|
|双指针         |背包     |堆|
|图             |分治    |跳表|
|模拟、枚举、递推 |贪心     |线段树|
|排序            |位运算  |-|

## 基础篇
### 数组、栈、队列
#### 每日一题
- [x] [【Day 01】989. 数组形式的整数加法](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%201%E3%80%91989.%20%E6%95%B0%E7%BB%84%E5%BD%A2%E5%BC%8F%E7%9A%84%E6%95%B4%E6%95%B0%E5%8A%A0%E6%B3%95.md)   
- [x] [【Day 02】821. 字符的最短距离](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%202%E3%80%91821.%20%E5%AD%97%E7%AC%A6%E7%9A%84%E6%9C%80%E7%9F%AD%E8%B7%9D%E7%A6%BB.md)
- [x] [【Day 03】1381. 设计一个支持增量操作的栈](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%203%E3%80%911381.%20%E8%AE%BE%E8%AE%A1%E4%B8%80%E4%B8%AA%E6%94%AF%E6%8C%81%E5%A2%9E%E9%87%8F%E6%93%8D%E4%BD%9C%E7%9A%84%E6%A0%88.md)
- [x] [【Day 04】394. 字符串解码](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%204%E3%80%91394.%20%E5%AD%97%E7%AC%A6%E4%B8%B2%E8%A7%A3%E7%A0%81.md)
- [x] [【Day 05】232. 用栈实现队列](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%205%E3%80%91232.%20%E7%94%A8%E6%A0%88%E5%AE%9E%E7%8E%B0%E9%98%9F%E5%88%97.md#%E9%A2%98%E7%9B%AE%E6%8F%8F%E8%BF%B0)
- [x] [【Day 06】768. 最多能完成排序的块 II](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%206%E3%80%91768.%20%E6%9C%80%E5%A4%9A%E8%83%BD%E5%AE%8C%E6%88%90%E6%8E%92%E5%BA%8F%E7%9A%84%E5%9D%97%20II.md)
- [x] [【Day 07】61. 旋转链表](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%207%E3%80%9161.%20%E6%97%8B%E8%BD%AC%E9%93%BE%E8%A1%A8.md)
- [x] [【Day 08】24. 两两交换链表中的节点](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%208%E3%80%9124.%20%E4%B8%A4%E4%B8%A4%E4%BA%A4%E6%8D%A2%E9%93%BE%E8%A1%A8%E4%B8%AD%E7%9A%84%E8%8A%82%E7%82%B9.md)
- [x] [【Day 09】109. 有序链表转换二叉搜索树](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%209%E3%80%91109.%20%E6%9C%89%E5%BA%8F%E9%93%BE%E8%A1%A8%E8%BD%AC%E6%8D%A2%E4%BA%8C%E5%8F%89%E6%90%9C%E7%B4%A2%E6%A0%91.md)
- [x] [【Day 10】160. 相交链表](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%2010%E3%80%91160.%20%E7%9B%B8%E4%BA%A4%E9%93%BE%E8%A1%A8.md)
- [x] [【Day 11】142. 环形链表 II](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%2011%E3%80%91142.%20%E7%8E%AF%E5%BD%A2%E9%93%BE%E8%A1%A8%20II.md)
- [x] [【Day 12】146. LRU 缓存机制](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%2012%E3%80%91146.%20LRU%20%E7%BC%93%E5%AD%98%E6%9C%BA%E5%88%B6.md)
- [x] [【Day 13】【Day 13】104. 二叉树的最大深度](https://github.com/ZhangNN2018/91alg/blob/main/Basic/array_stack_queue/%E3%80%90Day%2013%E3%80%91104.%20%E4%BA%8C%E5%8F%89%E6%A0%91%E7%9A%84%E6%9C%80%E5%A4%A7%E6%B7%B1%E5%BA%A6.md)
- [ ] [【Day 14】]()
- [ ] [【Day 15】]()
- [ ] [【Day 16】]()
- [ ] [【Day 17】]()
- [ ] [【Day 18】]()
- [ ] [【Day 19】]()
- [ ] [【Day 20】]() 
- [ ] [【Day 21】]() 
