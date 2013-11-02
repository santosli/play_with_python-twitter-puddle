#Twitter-Puddle
===================
question from: *[I Failed A Twitter Interview][1]*  
问题来自:[《I Failed A Twitter Interview》][2]  
译文:[《我的Twitter技术面试失败了》][3]  
译者:CuGBabyBeaR

##Question 题目简述:  

**Note:*** All the English description of question and logic of solution comes from original author.*   
**注意:** *所有英文的关于问题、算法逻辑的描述都是来自原作者。*

"Consider the following picture:"  
"如下图所示"

![enter image description here][4]

"In this picture we have walls of different heights. This picture is represented by an array of integers, where the value at each index is the height of the wall. The picture above is represented with an array as [2,5,1,2,3,4,7,7,6]."  
"Now imagine it rains. How much water is going to be accumulated in puddles between walls?"  
“在这个图片里我们有不同高度的墙。这个图片由一个整数数组所代表，数组中每个数是墙的高度。上边的图可以表示为数组[2,5,1,2,3,4,7,7,6]”  
“假如开始下雨了，那么墙之间的水坑能够装多少水呢？”  

![enter image description here][5]  
"We count volume in square blocks of 1X1. So in the picture above, everything to the left of index 1 spills out. Water to the right of index 7 also spills out. We are left with a puddle between 1 and 6 and the volume is 10."  
“以1×1的方块为单位计算容积。所以，在上边的图中下标为1以左的都会漏掉。下标7以右的也会漏掉。剩下的只有在1和6之间的一坑水，容积是10”

##Solution  算法逻辑  
双向遍历，同时保存左右两边的最大值，并计算可以装多少水直到两个指针相遇为止。和二叉排序的双向遍历比较相似。


  [1]: http://qandwhat.apps.runkite.com/i-failed-a-twitter-interview/
  [2]: http://qandwhat.apps.runkite.com/i-failed-a-twitter-interview/
  [3]: http://blog.jobbole.com/50705/
  [4]: http://ww1.sinaimg.cn/mw690/7cc829d3gw1ea56snnnkzj205m03z744.jpg
  [5]: http://ww3.sinaimg.cn/mw690/7cc829d3gw1ea56pjntkoj205m03zaa2.jpg
