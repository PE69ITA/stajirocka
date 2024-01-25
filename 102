# Definition for a binary tree node.
# class TreeNode:
#     def __init__(self, val=0, left=None, right=None):
#         self.val = val
#         self.left = left
#         self.right = right
class Solution:
    def maxDepth(self, root: Optional[TreeNode]) -> int:
        depth = 0
        def recurssion(node, depth):
            if node == None:
                return depth
            else:
                depth1 = recurssion(node.left, depth + 1)
                depth2 = recurssion(node.right, depth + 1)
                return max(depth1, depth2)
        return recurssion(root, depth)
