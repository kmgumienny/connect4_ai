Kamil Gumienny

For the Connect 4 AI, I implemented the Alpha Beta pruning minimax algorithm to calculate the heuristics. I believed that the alpha-beta pruning algorithm is the best option and will produce the best results if it is optimized correctly.

1)	How did I test my agents?
a.	I tested my agent by using the tournament and run and classes to play games. I would switch up the seeds to see how my code kept up with the random bots. I also went into debug mode to try and follow my code to see how it was thinking and where I could improve it. 
2)	What did your tests reveal?
a.	My tests showed that there were quite a few bugs in my code when it came to traversing the playing field to see where the best position to put a chip would be. Following the code along in debug mode proved to be very difficult as seeing how it came to a decision took far too much time. At a depth of 4, I could imagine there were thousands and thousands of evaluations being completed. I could not really keep up and would go to the parts of the code where I knew what was going on to try and tweak it.
b.	The best method for modifying the code was making a change and running the tournament. That was the basic strategy I used to try and test the code to decide between iterations. Some methods worked a lot better than others and I would occasionally get frustrated trying to back peddle to better working code. 
c.	In the end, I think my code came out to be fine enough to win a tournament, but it was still very buggy and would not make the decisions I thought I designed it to make. I’m still unsure of what the best method is to test the code or how to best implement the evaluation function I had in my mind. 
3)	What was I able to accomplish?
a.	In HW2 I was very optimistic in how easy I thought I could test my code. My original goal was to go through every single point in the game board and calculate heuristics that way. I changed my mind and decided to go about heuristics a different way by simply going through a game board and evaluating it that way. It still proved to be buggy regardless which was a little frustrating but I believe I was able to do the bare minimum.
a.	My original evaluation function was going to focus on:
i.	The score evaluation method will require the most fine-tuning. As of right now, my implementation will probably include +100 points for an available winning configuration and -100 for an available losing configuration. Then, different point values will be assigned for the following scenarios:
1.	x in a row disjoint
2.	x in a row continuous
3.	x in a row unobstructed
4.	x in a row one side obstructed (either with a piece or board edge)
5.	x in a row blocked off (non-threats)
6.	x in a row streaks of the above
7.	A possible move’s distance from middle 
b.	I was not able to get around to implementing an evaluation function for a move’s distance from the middle but everything else was implemented in a “decent” manner although it did not work perfectly. 
4)	How would you improve your code?
a.	I would improve my code by finding a better way to test it. The testing I underwent proved far too difficult for tracking every decision the AI made. I could only make changes and follow along that way which was very, very annoying and I was not able to sweep the tournament no matter what changes I made. 



https://cs.stackexchange.com/questions/13453/trying-to-improve-minimax-heuristic-function-for-connect-four-game-in-js
https://stackoverflow.com/questions/10985000/how-should-i-design-a-good-evaluation-function-for-connect-4
https://towardsdatascience.com/creating-the-perfect-connect-four-ai-bot-c165115557b0
https://www.youtube.com/watch?v=MMLtza3CZFM
https://www.youtube.com/watch?v=m1l3k_rcG0M&t=238s
