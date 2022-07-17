# LeetCode - Palindrome Number

### Given an integer x, return true if x is palindrome integer.

### An integer is a palindrome when it reads the same backward as forward.

### For example, 121 is a palindrome while 123 is not.

#### 題目：判斷傳入的數字是否為回文
##### 代表要將數字轉為字串，首先我使用了sstream的函示庫使用stringstream來轉換int
##### 想法是以下：
##### 　　x為偶數時，代表每次比較的字都要相同，如：123321的1-1、2-2、3-3
##### 　　x為奇數時，最中間那個字完全不會影響所以可以不理他，只管左右即可，如：12321的1-1、2-2，以及12521也是比1-1、2-2
##### 　　附帶一個負數時不會是對的，只要以上想法就能解出此題
 
---

### Example 1:

Input: x = 121

Output: true

Explanation: 121 reads as 121 from left to right and from right to left.

### Example 2:

Input: x = -121

Output: false

Explanation: From left to right, it reads -121. From right to left, it becomes 121-. Therefore it is not a palindrome.

### Example 3:

Input: x = 10

Output: false

Explanation: Reads 01 from right to left. Therefore it is not a palindrome.
 
--- 

### Constraints:

-231 <= x <= 231 - 1
 
---

### Follow up: Could you solve it without converting the integer to a string?
