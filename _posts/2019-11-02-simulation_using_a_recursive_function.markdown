---
layout: post
title:      "Simulation using a Recursive function"
date:       2019-11-02 22:41:00 -0400
permalink:  simulation_using_a_recursive_function
---


  My instructor said it best when he stated 'recursive functions make my head hurt.' No more definite truth has ever been spoken however despite the fact they're a tedious puzzle they also incredibly useful .  Now that I've dressed recrusive functions up as wretched problem perhaps I should be slightly more objective with an exact definition according to Wikipedia: 
*Recursion in computer science is a method of solving a problem where the solution depends on solutions to smaller instances of the same problem (as opposed to iteration).[1] The approach can be applied to many types of problems, and recursion is one of the central ideas of computer science.*
   So you're probably thinking Jeff was on the money right now with his assertion and honestly he's never steered me wrong. All is not lost though, I'm writing a blog about recursive functions and i can barely understand that definintion. I had an example that seemed pretty simple from the fine folks at learn.co:
![](https://raw.githubusercontent.com/Edward-Beck/Recursive_Blog/master/Recursive_Function.png)
	Well if you're anything like me, you still don't know what's going on so you start trying to work back from the solution 45 and the input is an array 1,2,3,4,5,6,7,8,9 and the name definition is ' mysum(L) ' Maybe try summing the numbers together? I actually did this without realizing the name of the definion...its been a hard life. So summation of the array that was labeled L in the definition is 45. I probably shouldn't admit this but I feel like were practically besties now that we gotten this far together but i was still lost at this point because i was somewhat overlooking array. notation and also recursive functions just kinda make your head hurt. Best to skip the mental gymnastics for a moment and see what we can pull from a print of L[0]:
	![](https://raw.githubusercontent.com/Edward-Beck/Recursive_Blog/master/L%5B0%5D.png)		
		That makes sense and then the function is being recalled again with a space shorter array (given to you by mysum(L[1:] ) Double checking with an altered print statment including L[1:] 
	![](https://raw.githubusercontent.com/Edward-Beck/Recursive_Blog/master/L%5B1%5D.png)
			Again this kinda makes sense the second last iteration L[1:] is [9] and the last iteration is [ ] so L[1:] is 0 and when this is passed into the argument of mysum( ) the if instead of the else is used which returns a 0 and there are no more recursions...but they're not iterations according to wikipedia who is way smarter than me. Yet this still doesn't seem to make a lot of sense, yes if you sum the array it comes out to 45 but how is the function actually accomplishing this?? Well seeing how the only real option we have to explore here is L[0] lets make a list using the append function.  
	![](https://raw.githubusercontent.com/Edward-Beck/Recursive_Blog/master/append.png)
	 The return value is L[0] + mysum( L[1:] ) which is really return L[0]+L[0]+ L[0]+L[0]+ L[0]+L[0]+ L[0]+L[0]+L[0] + 0 (for the if clause) . Looking at our list of appended values of L[0] were back to 45! 
		   We can move on to bigger things, like what i really want to use a recurse function to do, update my asset and libility portfolio every day on its own. Seeing on how i can get a little wordy to say the least what i'm trying to do is first rebalance my asset portfolio according to ALM guidelines based upon the profits i took in during the day. With my new profits plus my past assets I can then determine how much liability I can safely accomidate.
![](https://raw.githubusercontent.com/Edward-Beck/Recursive_Blog/master/Re_asset.png)
