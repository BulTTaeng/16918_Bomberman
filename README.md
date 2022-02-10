# 16918_Bomberman

made by Jaehyeok Choi

## Welcome to Jaehyeok's github!

## What is the problem?

![image](https://github.com/Choi-JaeHyeok-21500749/16918_Bomberman/blob/main/16918_pro.PNG)

## What Algorithm should I use?

Graph Algorithm , BFS , Simulation

## What was the key point and the hard part?

I thought first situation (1 second situation) will be repeated. However that was not true.

If bombs explode and that section is not affected by 3 second situation, there is possibility that the number of bombs can increase.

So, I divide situation by 4 case.

1. N == 1

Same as first situation.

2. N % 4 == 2 or 0 ( N is even)

Fill bombs and print it.

3. N % 4 == 3

This is situation when first bombs are explode. In this case , we don't have to consider possibility of getting extra bombs. 

Extra bombs are always in the explosion range, so we don't have to consider it.

So, run BFS in bombs location and print it.

4. N % 4 == 1

This situation is tricky one.

As I said, because there is a possibility of extra bombs, I have to check the explosion range of original bombs location(which is given by input), and beside those range,

the bombs gonna be survive so if we check original bomb's explosion range as 'O'(This is because we fill all location with bombs in N%4 == 0 situation) , '.' part will be where bombs are exist.

So, run BFS in every location '.' and explode near location and print it.

The key point is that (0,1) second situation is not always repeated as in the example part in the problem!!

There is a possibility of bombs increase!

## Where can I get more help, if I need it?

You can contact me through email, which is wogur7496@gmail.com.
Thank you for visiting this github!
