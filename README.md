## Introduction

Hi! Welcome to my LeetCode repository. This repository is for my personal reference, where I'll be solving LeetCode problems, identifying patterns, and providing explanations. 

## Sorting
#### Bubble Sort

```python
class Solution(object):
    def sortArray(self, nums): # Selection sort
        for i in range(len(nums)):
            for j in range(i + 1, len(nums)):
                if nums[i] > nums[j]:
                    nums[i], nums[j] = nums[j], nums[i]
        return nums

## Binary Tree
#### Breadth First Search

- Follows a FIFO (First In, First Out) approach.
- Can be implemented using a queue.

                 1
               /   \
              2     3

Step 1: Append root to deque() => queue = [(TreeNode(val: 1))], res = [] \
Step 2: Using while loop, pop first value and append its children queue = [(TreeNode(val: 2), (TreeNode(val: 3))], res = [1] \
Step 3: Pop 2 and append its children, since 2 has no children it will stop at 2. queue = [((TreeNode(val: 3))], res = [1,2] \
Step 3: Pop 3 and append its children, since 3 has no children it will stop at 3. queue = [], res = [1,2,3] \
Step 4: Since queue is empty it will stop while looping. 
#### Depth First Search

- Follows a FILO (First In, Last Out) approach.
- Can be implemented using a stack or recursively.

1) Find the maximum / minimum depth
