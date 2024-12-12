# Longest-Consecutive-Sequence
Given an unsorted array of integers nums, return the length of the longest consecutive elements sequence.
Explanation:
HashSet for Quick Lookup:

Add all numbers to a HashSet to check if a number is part of a sequence in O(1) time.
Identify Sequence Starts:

For each number, check if num - 1 exists in the set. If it doesn’t, the current number is the start of a sequence.
Count Sequence Length:

Increment the sequence by checking if num + 1 exists in the set until the sequence ends.
Update Longest Streak:

Keep track of the longest streak by comparing the current streak to the previously recorded maximum.
Time and Space Complexity:
Time Complexity: O(n)
Each number is processed once to add to the set and once to count the sequence.
Space Complexity: O(n)
Space required for the HashSet.
