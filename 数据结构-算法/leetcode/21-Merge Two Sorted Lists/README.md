A：Merge two sorted linked lists and return it as a new list. The new list should be made by splicing together the nodes of the first two lists.

**Example:**
```
Input: 1->2->4, 1->3->4
Output: 1->1->2->3->4->4
```
Q：
```cpp
/**
 * Definition for singly-linked list.
 * struct ListNode {
 *   int val;
 *   ListNode *next;
 *   ListNode(int x) : val(x), next(NULL) {}
 * };
 */
class Solution {
  public:
    ListNode* mergeTwoLists(ListNode* l1, ListNode* l2) {
      // 处理为空情况
      if (!l1 && !l2) return NULL;
      if (!l1) return l2;
      else if (!l2) return l1;
      // 设置中间变量指针 p
      ListNode* p;
      // 设置 p 的头结点
      if (l1->val < l2->val) {
        p = l1;
        l1 = l1->next;
      } else {
        p = l2;
        l2 = l2->next;
      }
      // 保存 头结点 指针
      ListNode* result = p;

      while(l1 && l2){
        if (l1->val < l2->val) {
          p->next = l1;
          l1 = l1->next;
        } else {
          p->next = l2;
          l2 = l2->next;
        }

        p = p->next;
      }
      // 处理剩余部分
      if (!l1) p->next = l2;
      else if (!l2) p->next = l1;
      // 返回 头结点 指针即可
      return result;
    }
};
```
