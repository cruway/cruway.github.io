---
title: Codility Test (1. binaryGap)
excerpt: Codility Testを実施しました。
toc: true
toc_sticky: true
toc_label: index
categories:
- algorithm
tags:
- algorithm
- codility
date: 2019-09-11
---

# Codility Test (1. binaryGap)

A  _binary gap_  within a positive integer N is any maximal sequence of consecutive zeros that is surrounded by ones at both ends in the binary representation of N.

For example, number 9 has binary representation  1001  and contains a binary gap of length 2. The number 529 has binary representation  1000010001  and contains two binary gaps: one of length 4 and one of length 3. The number 20 has binary representation  10100  and contains one binary gap of length 1. The number 15 has binary representation  1111  and has no binary gaps. The number 32 has binary representation  100000  and has no binary gaps.

Write a function:

> class Solution { public int solution(int N); }

that, given a positive integer N, returns the length of its longest binary gap. The function should return 0 if N doesn't contain a binary gap.

For example, given N = 1041 the function should return 5, because N has binary representation  10000010001  and so its longest binary gap is of length 5. Given N = 32 the function should return 0, because N has binary representation '100000' and thus no binary gaps.

Write an  ****efficient****  algorithm for the following assumptions:

> -   N is an integer within the range [1..2,147,483,647].

Copyright 2009–2019 by Codility Limited. All Rights Reserved. Unauthorized copying, publication or disclosure prohibited.

# 問題回答
````
public int resultMethod(int number) {
	int saveResult = 0;
	int binaryResult = 0;
	boolean gapStart = false;
	
	while(true) {
		if(number == 0) {
			break;
		}
		if(number % 2 == 0) {
			if(gapStart) {
				saveResult++;
			}
		} else if(number % 2 == 1) {
			if(gapStart) {
				binaryResult = binaryResult > saveResult ? binaryResult : saveResult;
				saveResult = 0;
			}
			gapStart = true;
		} else {
			return 0;
		}
		number = number / 2;
	}
	return binaryResult;
}
````

# 別のコード参照(超簡単)
````
class Solution {
    public int solution(int n) {
        n >>>= Integer.numberOfTrailingZeros(n);
        int steps = 0;
        while ((n & (n + 1)) != 0) {
            n |= n >>> 1;
            steps++;
        }
        return steps;
    }
}
````
