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

