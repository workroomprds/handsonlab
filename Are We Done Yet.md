# Are we Done Yet?

*Basics:* Are we Done Yet? - estimation in a non-linear world, leading to insights into diversity.

*Source:* Insights into Exploratory Testing workshop, blog articles http://workroomprds.blogspot.com/2012/11/an-experiment-with-probability.html to http://workroomprds.blogspot.com/2012/12/modelling-super-powers.html

*Output:* Experience of estimating done-ness. To act as a trigger / example for conversations about diversity and completeness.

## Requirements

At least one device that runs flash (for now)

## Logistics

(Currently) an experience to trigger discussion.

Can be rushed in under 10 minutes. Better if it takes 20-30 in the activity, and 10 more in conversation afterwards.

There are 4 examples – the early ones take longer.

Works as a large-group exercise if individuals are prepared to talk about their decisions and predictions. It's possible to give participants the chance to make their own conclusions, but as fewer people can run flash on their kit, it becomes less possible to give them their own direct experience for talking about. Better to do an all-group thing – a bit like watching a video and talking about it. Non-flash version is under developemnt.


## Process

Introduce the simplification – we know how many bugs there are. Some are hard to find, some easy. We have a limit on how many bugs we can find, in a single bit of work.

Introduce the simulation – a budget for work. Work that has been done / yet to be done. Bugs that have been found / yet to be found.

### Example 1

Ask the group to predict what will happen. Specifically, ask them how early work might be differnt from later work – perhaps as a graph of bugs found by effort put in. How does this model differ from experience? Is it an understandable difference?

Skip through the sim, ~100 at a time. Does the model match expectations? Does it match experience? We see a "curtain fall" of yellow – what does it represent?

Open question, to be repeated: "Are we done yet? How do we know?" 

The reasonable (and most-common) answer is "We don't know" – so dig into what we'd need to know, and whether we usually know the answers to that as we work. Adjust to "shall we spend another 100?", as the sim reveals diminishing returns. Adjust to "Should we test at all?", "Should we test after our budget has run out?", "Could we reduce our budget if we did the same thing again?".

### Example 2

What's changed? Now, 6 testers. 

What will happen? This model will chew through the budget faster, but the graph of found vs effort will be much the same. Are we doing better? 

"Are we done yet?" – is there any difference with Example 2? Skip through, 100 by 100.

### Example 3

What's changed? Each of the 6 testers finds in a different way. So a bug that is hard for one to find is easy for another to find.

What will happen? 

Run the sim. How did the first 100 of this sim's budget compare with Examples 1 and 2?

Compare the first 100 with the last 500. "Are we done yet?" "Where might we stop?".

Open a conversation on what we saw: what does it mean, that the same problem is hard to spot for one tester, but easy for another? How might that reflect the world? Who has worked in a situation / team where that was a bit true? Is it true about bugs / testers? What difference might it make to have a variety of strengths (and weaknesses) on a team? How does your experience differ – and what do those differences say about the model?

### Example 4

What's changed? We have one tester, who switches randomly between "techniques". Each time the sim switches their technique, the tester's skill at their new approach resets to 0, and builds over time.

How will this compare? Your audience may be sick of hypotheising at this point, so run the sim and compare what happens.

Again, at what point might we say "Are we done yet?". After a given budget, or can we use another measure?

How does this model compare with experience? What might we change to make it more useful – or more accurate (and would that be more useful?).

### Discussion

With these models, diversity is an advantage. Why?

Diversity of what?

In what circumstances might diversity not be an advantage? How would you show that, with a model?

How might you, in practice, adjust yourselves as a team? As an individual? What can you encourage? What choices might be especially useful?


## Versions

Each purple dot, when revealed, becomes a yellow dot. Its size changes; 1 in 10 are 10x as big, 1 in 100 are 100x as big, 1 in 1000 are 1000x as big and so on. This is a [power law](https://en.wikipedia.org/wiki/Power_law "Power law - Wikipedia") relationship. Power laws are found in nature where stuff is distributed unevenly (star mass, city size, income), and means (if you don't know the overall size of a distributed resource) that the more samples you take, the more the average moves around.

Might an individual bug (whatever that might be) have a power-law distribution in some quality? What would that mean for our assessment of that quality for a given system which might contain / used to contain a collection of those bugs?

## Website text / abstract
These simulations model testing and discovery. 

We've made a groteque simplification: we know how many bugs there are, and we model our work to discover them by deciding that some are hard to find, some easy. 

We introduce a wrinkle: a limit on how many bugs we can find, in a single bit of work. This adjustment makes the output easier to grasp, and is closer to experience.

In this simulation, we have a budget for work. We can see work that has been done / yet to be done, and bugs that have been found / yet to be found.

We'll play and predict to dig more deeply into the model, to examine one role of diversity in testing, and to understand our own beliefs about how we organise and budget discovery activities.

Exercise [1 - basic](http://exercises.workroomprds.com/bugfinder/Exercise03.00%20-%20basic/)

Exercise [2 - single tactic](http://exercises.workroomprds.com/bugfinder/Exercise03.01%20-%20single%20tactic/)

Exercise [3 - mulitple tactics](http://exercises.workroomprds.com/bugfinder/Exercise03.02%20-%20multiple%20tactics/)

Exercise [4 - switching tester](http://exercises.workroomprds.com/bugfinder/Exercise04.01%20-%20switching%20tester/)

Exercise [5 - switching testers](http://exercises.workroomprds.com/bugfinder/Exercise04.02%20-%20switching%20testers/)


