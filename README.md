# COMP30020
The University of Melbourne School of Computing and Information Systems

COMP30020 - 墨尔本大学计算机课程 COMP30020 全程满分攻略

## 专业一对一 **原创开发 + 辅导答疑** ， 有需要可联系 QQ ： **1215714557**

墨尔本大学计算机专业课程 COMP30020 的课程作业， 全程满分， 可辅导开发。

## Proj1 - 第一次作业 解题记录

### 1. 题目分析

首先是我的分析, 手稿，就不敲了，上图，每个 `guess` 总共五种情况，说白了就是每种情况都去分析，根据 `feedback` 计算下一次`guess`， 直到`guess`全部正确

![proj1_1](project%201/pic/proj1_1.jpg)

### 2. 编译
编译就是常规的haskell编译方式：
``` bash
ghc -O2 --make Proj1Test
```

### 3. 运行结果
``` bash
sandy@sandy:~/haskell/proj$ ./Proj1Test 2C 3C 4H 5S
Your guess 1:  [4C,7D,TH,KS]
My answer:  (0,2,1,0,3)
Your guess 2:  [2C,3C,4D,4H]
My answer:  (3,0,3,1,3)
Your guess 3:  [2C,3C,4D,5S]
My answer:  (3,0,4,0,3)
Your guess 4:  [2C,3C,4H,5S]
My answer:  (4,0,4,0,4)
You got it in 4 guesses!
Approximate quality = 100.0%
sandy@sandy:~/haskell/proj$ ./Proj1Test 2C TC 4H TS
Your guess 1:  [4C,7D,TH,KS]
My answer:  (0,1,2,0,3)
Your guess 2:  [2C,5C,4D,7H]
My answer:  (1,0,2,2,3)
Your guess 3:  [2C,7C,8D,TS]
My answer:  (2,0,2,0,3)
Your guess 4:  [2C,9C,4H,TS]
My answer:  (3,0,3,0,4)
Your guess 5:  [2C,TC,4H,TS]
My answer:  (4,0,4,0,4)
You got it in 5 guesses!
Approximate quality = 100.0%
sandy@sandy:~/haskell/proj$ ./Proj1Test 2C TC TH TS
Your guess 1:  [4C,7D,TH,KS]
My answer:  (1,1,1,0,3)
Your guess 2:  [2C,4C,4D,4H]
My answer:  (1,0,1,3,3)
Your guess 3:  [2C,5C,5D,KS]
My answer:  (1,0,1,0,3)
Your guess 4:  [2C,6C,TH,6S]
My answer:  (2,0,2,0,4)
Your guess 5:  [2C,8C,TH,8S]
My answer:  (2,0,2,0,4)
Your guess 6:  [2C,9C,TH,9S]
My answer:  (2,0,2,0,4)
Your guess 7:  [2C,TC,TH,TS]
My answer:  (4,0,4,0,4)
You got it in 7 guesses!
Approximate quality = 93.11542806914406%
sandy@sandy:~/haskell/proj$ ./Proj1Test 2C TC
Your guess 1:  [5C,TD]
My answer:  (0,1,1,0,1)
Your guess 2:  [2C,TC]
My answer:  (2,0,2,0,2)
You got it in 2 guesses!
Approximate quality = 100.0%
sandy@sandy:~/haskell/proj$ ./Proj1Test 2C 3C 4C 5C
Your guess 1:  [4C,7D,TH,KS]
My answer:  (1,2,1,0,1)
Your guess 2:  [2C,3C,4C,5C]
My answer:  (4,0,4,0,4)
You got it in 2 guesses!
Approximate quality = 100.0%
sandy@sandy:~/haskell/proj$
```
