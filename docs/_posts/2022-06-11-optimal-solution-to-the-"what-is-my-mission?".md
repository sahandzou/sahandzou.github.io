In the first year semester of university, I went to the office of one of my university professors. And I want to get some advice for the **"finding my purpose"** question. 


There was one statement that sticks to my mind **"you have time till the end of your 20s to taste, and find the one that fits you but whatever you do, you should take it seriously"**.

Days passed till I read the book [Algorithms to Live By: The Computer Science of Human Decisions](https://www.amazon.com/Algorithms-Live-Computer-Science-Decisions/dp/1627790365) which triggered my mind to think about that statement from a different view.


One section of the book is about **exploring/exploiting** problem a famous classic problem in Reinforcement Learning.

In the following I am trying to use the idea of the book to answer my question.

So let's begin

Think of a Mars 2020 rover([Perseverance](https://mars.nasa.gov/mars2020/)) whose goal is to “seeking preserved signs of biosignatures in rock samples”; it has a limited amount of resources, and it should find the best rock samples to drill.

# Approaches:
1. **blind try:** the approach sums up to drilling every rock it sees and taking samples from.  
In this scenario, The exploration zone is very small, and the expected reward becomes small too.

2. **selection with heuristic:** choosing probable good rock with a program that tells robots to drill or not, the heuristic could be hard coded or learned over time from nothing, in the case of hard coded heuristic the exploration zone becomes much bigger than approach 1 and the expected reward becomes larger too in case of the heuristic learns over time the reward is totally proportional to the amount of resource we have and with the Mars robot scenario I think the reward is laid down between blind try and hard coded heuristic.

3. **secretary problem approach; heuristic learned over time:**  
[The secretary problem](https://en.wikipedia.org/wiki/Secretary_problem): assume you are a boss and want to hire one secretary, and you don’t have any heuristic about how well is one secretary is, and you should tell them if they are rejected or accepted after interview .when you interview with him/her the optimal approach to hiring is that you should just see 37% of first secretaries and rejecting all of them and after that select the first one who is better than every applicant interviewed so far (or continuing to the last applicant if this never occurs).  
So assuming that the robot can’t take back the road it navigates before, the robot first should just explore the 37% of the road it can navigate, and after that, with heuristics he learned, start to take samples from rocks.

Approache 3 is the optimal solution to the Mars rover question with simplified assumptions!

Now think of a human child that puts into the new world and his goal is to find his mission. What is the optimal solution? Seems familiar? Explore/exploit problems. 
Should he stick with the first thing he finds interesting or …?

# Human Agent first scenario
The problem is more complicated than the Mars rover but let's simplify it.  
First, think that child has no ability to infer except that he just has memory, and also ignore that child can roll back to what he did before and do that again.
So the optimal solution for him is the secretary problem approach and assuming that the average life expectancy in first world countries is 78 the threshold for exploration is Around age 29.

# Human Agent second scenario
But the assumptions we take are strong simplified assumptions; the human can learn over time, have the ability to infer and recognize wrong paths, also he can take back and does the job he did before, so the question becomes much harder, one similar problem could be extension of secretary problem [“secretary problem with recall”](https://projecteuclid.org/journals/annals-of-probability/volume-21/issue-2/The-Infinite-Secretary-Problem-with-Recall/10.1214/aop/1176989273.full) but let's use our intuition to solve this problem.  
With the recall option and ability to learn, we can take much higher risk and put much higher weight on exploring scenarios also in life the exploit/explore scenario are not separated from each other within every time frame you look you have both exploration and exploitation coupled up with each other. Till age 18 a large amount of your time is spent on school(exploit+tiny explore).  
So considering the human life journey till 18 even the optimal solution to the human agent's first scenario should be bigger than 29.

- the ability to learn and inference(heuristic learns over time) reduces the explore weight   
- the major part of our 10s are dedicated to exploit so reduces the exploit weight  
- roll back option reduces the exploit weight

I think choosing the trade of between these is different from human to human. But intuitively it should be more than 37% for exploration in today's world.

So with these explanations even if you don't find your mission till the end of your 20s it's not late at all.



