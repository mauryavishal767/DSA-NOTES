# Two Pointer

**Given an array B find the number of pairs such that `b[i] + b[j] <= K`**

- i =0; j=n-1; sum≤k? i++ : j—; count += j-i

---

**Given an array B find the number of pairs such that `L <= (b[i] + b[j]) <= R`**

0 1 2 3 4 5 6.
L = 3  R = 5.
- Sort
- `F[g]` = no. of pairs such that `b[i]+b[j] <=g`
- Answer = `F[R] - F[L-1]`

---

**Two Sum**

- sort
- `i = 0`, `j = n-1`;
- sum = `arr[i] + arr[j]`;
- if sum is greater `j--` to reduce the sum
- if sum is smaller `i++` to increase sum.

---

**Two Sum from two array**

same as above
- `i = 0` of array `A[ ]` 
- `j = n-1` of array `B[ ]`

---

**Largest subarray with unique elements**
[Document](https://docs.google.com/document/d/1Utku2AUwPW4iiXhQDi-MUzMpyNm_78VCCWec55g2cas/edit)

B = [ 3 2 4 5 2 6 7 8 9 10] 
O/P - 8 

- i = 0, j = 0;
- j++, 
- if num repeat, i = last index + 1;
- maintain max length, to check repeating elements use map
- after resetting i delete all elements before i from the map;

---

**Given an array B[ ], find the number of pairs such that `b[i] + b[j] <= k`**
[Document](https://docs.google.com/document/d/1BAtrKGHmF-OxSRuHtrdtR_5iG24nIGi1Oa7mjEKaumY/edit)

- `i = 0` and `j = n-1`
- if sum is greater `j--` 
- else `count += j-i+1`, `i++`;

---

**Given an array of size `N` find the longest subarray which has all distinct number in it**

same as above question 
"Largest subarray with unique elements"

---

**Given Two strings A and B. Find if B is sub string of A (could be non-consicutive)**
A = vishal
B = sl
o\p = yes

- `i = 0` of string A
- `j = 0` of string B
- if char are not same `i++`;
- if same `i++`, `j++`;

---

**Same as before but -> You are allowed to changed at max 1 character(not first) in string B , If match return index of first matching else -1**
[Document](https://docs.google.com/document/d/1xEhtam-dLx9GABHz0xAphXWq0NaQ6uCYTUYwA3P9R1k/edit)

- if find first char of B in A then do next step else return -1
- change every char to (a-z) and check every varient of staring if it exsist A.

---

**Given two array A and B :- Find the number of good indices in array B**

**Good Index meaning - When you remove this index :- array B becomes a subsequence of array A**

[Document](https://docs.google.com/document/d/18JsYIqpFFBRxa9k63jeotMcPnGeU9-rlC3IvNEGw-8s/edit)

- simmilar as above, where `b[j]` means every element of array B till j exist in array A till `A[i]`.

- if we want to remove any element(X) of array B we can check if all elements before X exists in A and all element after X also exist in A. 

- to do so we can keep a array to store for `B[j]` what is the i till where they are same, and same from back side.

- for every index we will check if index(i<sub>1</sub>) in A associated with `b[j-1]` is occure before index(i<sub>2</sub>) which is associated with `b[j+1]`. or else j is not a good index.

---
