Reverse-Linked-List-II-LeetCode
"C implementation of LeetCode #92: Reverse Linked List II using an in-place, one-pass pointer manipulation technique. Optimized for
space complexity."
🧩 LeetCode 92: Reverse Linked List II (C Solution)
A robust and efficient solution to the Reverse Linked List II problem on LeetCode, implemented in pure C using iterative pointer manipulation.
📖 Problem Description
Given the head of a singly linked list and two integers left and right where left <= right, reverse the nodes of the list from position left to position right, and return the reversed list.
Example

    Input: head = [1,2,3,4,5], left = 2, right = 4
    Output: [1,4,3,2,5]
    Explanation: The nodes from position 2 to 4 (2, 3, and 4) are reversed, while 1 and 5 remain in their original positions.

🛠️ Technical Approach
This solution uses a One-Pass Iterative approach to avoid the overhead of recursion or creating a new list.

    Dummy Node: A stack-allocated dummy node points to the head to gracefully handle cases where left = 1.
    Pointer Navigation: A prev pointer is moved to the position exactly before the reversal starts.
    In-Place Swapping: We use a "bridge" technique where each node in the [left, right] range is plucked and re-inserted immediately after the prev node.
    Efficiency: The iterative approach ensures the list is traversed only once.

📊 Complexity Analysis

    Time Complexity:
    — Single pass through the list to reach the target segment and perform swaps.
    Space Complexity:
    — Only a constant amount of extra pointer variables are used.

🚀 How to Use

    Copy the reverseBetween function into the LeetCode editor.
    The struct ListNode is pre-defined by the LeetCode environment.
    To run locally, include the standard <stdio.h> and <stdlib.h> headers and a main function to build and print the list.
