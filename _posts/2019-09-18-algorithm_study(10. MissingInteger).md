---
title: Codility Test (10. MissingInteger)
excerpt: Codility Testを実施しました。
toc: true
toc_sticky: true
toc_label: index
categories:
- algorithm
tags:
- algorithm
- codility
date: 2019-09-18
---
# Codility Test (10. MissingInteger)
This is a demo task.

Write a function:

class Solution { public int solution(int[] A); }

that, given an array A of N integers, returns the smallest positive integer (greater than 0) that does not occur in A.

For example, given A = [1, 3, 6, 4, 1, 2], the function should return 5.

Given A = [1, 2, 3], the function should return 4.

Given A = [−1, −3], the function should return 1.

Write an efficient algorithm for the following assumptions:

N is an integer within the range [1..100,000];
each element of array A is an integer within the range [−1,000,000..1,000,000].

# 問題回答
````
import java.util.*;

class Solution {
    public int solution(int[] A) {
        Set<Integer> setList = new HashSet<Integer>();
        for(int n : A) {
            setList.add(n);
        }
        
        for(int i = 1; i < Integer.MAX_VALUE; i++) {
            if(!setList.contains(i)) {
                return i;
            }
        }
        return -1;
    }
}
````
