### 精选题目
- LeetCode题目地址`leetcode`为英文版本，`leetcode-cn`为中文版本。
- 面试题 + 3位数字内指《剑指offer》，+ 4位数字指《程序员面试金典》。


- 递归类题目三步法：
    1. 递归终止条件？
    2. 递归 前or后 处理？怎么处理？
    3. 返回什么？

- 回溯问题，参考[labuladong的文章](https://leetcode-cn.com/problems/permutations/solution/hui-su-suan-fa-xiang-jie-by-labuladong-2/)：
```python
result = []
def backtrack(路径, 选择列表):
    if 满足结束条件:
        result.add(路径)
        return
    
    for 选择 in 选择列表:
        做选择
        backtrack(路径, 选择列表)
        撤销选择
```

- 树和图的算法：
    - 递归：DFS参考前序遍历、BFS参考层序遍历。
    - 非递归：DFS用栈、BFS用队列。
- 队列建议使用`from collections import deque`支持从头和尾部的常数时间append/pop操作。若使用Python的list，通过list.pop(0)去除头部会消耗$O(n)$的时间。

```
- 栈、链表：
        - 2（两数相加，栈）
        - 445（两数相加2，栈+头插法/反转链表）
        - 206（反转链表, 面试题24题相同）
        - 15（三数之和）
        - 125（验证回文串 列表 配合234.回文链表看）
        - 557（反转字符串中单词）
        - 859（亲密字符串）
        - 138（复制带随机指针的链表，面试题35题相同，迭代+节点拆分）
        - 1019（链表中的下一个更大节点，单调栈。类似题目有42/84/907/768/402）
        - 1290（链表二进制转十进制）
        - 3（滑动窗口）
- 双指针：
        - 141（环形链表I）
        - 142（环形链表II）
        - 19（删除链表的倒数第N个节点）
        - 82（删除排序链表中的重复元素II）
        - 143（重排链表）
        - 160（相交链表）
        - 234（验证回文链 + 链表反转）
        - 面试题 02.06（回文链表）
- 动态规划：
        - 53（最大子序和）
        - 120（三角最小路径和）
        - 70（爬楼梯，同面试题10-II）
        - 面试题08.01（三步问题）
        - 221（最大正方形）
        - 面试题47（礼物的最大价值）
        - 面试题17.16（按摩师）
        - 647（回文子串）
        - 面试题 17.06（2出现的次数）
        - 面试题 08.11（硬币）
        - 337（打家劫舍III, 动态规划+DFS）
- 回溯法：
    - 784（字母大小写全排列）
    - 17（电话号）
    - 面试题08.07（字符串组合）
        - 面试题08.09（括号）
    - 79（单词搜索，面试题12相同）
        - 51（N皇后）
        - 78（子集）
        - 90（子集II）
    - 93（复原IP地址）
- 递归：
        - 100（验证树相同）
    - 面试题08.05（递归乘法）
        - 面试题08.06（汉诺塔问题）
    - 面试题16（数值的整数次方）
- 排序：
        - 215（排序，和面试题51题一起看）
    - 148（链表排序）
    - 23（分治法）
    - 147（链表插入排序）
    - 1046（最后一块石头重量）
- 二叉树：
        - 654（最大二叉树）
        - 105（从前序与中序遍历序列构造二叉树，面试题07题相同）
        - 面试题26题（树的子结构）
    - 124（最大路径和）
        - 144（前序遍历）
        - 98（验证二叉搜索树）
        - 426(中序遍历, 双向循环链表)
        - 面试题54（反向中序遍历）
        - 面试题36（二叉搜索树与双向链表）
        - 110（平衡二叉树）
        - 508（出现次数最多的子树元素和, 递归DFS）  
        - 103（交叉层序遍历, D/BFS）
        - 面试题32-I（从上到下打印二叉树）
        - 面试题32-III（从上到下打印二叉树）
- DFS、BFS：
        - 111（二叉树的最小深度，BFS）
    - 543（二叉树的直径, DFS）
    - 130（被围绕的区域, 图DFS）
    - 200（岛屿数量, 图DFS）
    - 529（扫雷游戏, 图DFS）
    - 994（腐烂的橘子, BFS简单）
    - 199（树右视图, D/BFS）
    - 112（路径总和I）
    - 113（路径和II, DFS）
    - 257（二叉树的所有路径, DFS）
        - 226（翻转二叉树，面试题27题相同）
- 贪心算法：
    - 122（股票收益最好）
    - 123（股票，一种通用解法）
    - 455（分饼干）
    - 134（加油站）
    - 763（划分字母区间）
    - 435（五重叠区间）
    - 910（最小差值II）
```







