why write tests?  
While looking at a project with a huge set of fragile test cases which often break for non-product reasons, it is sometimes hard to justify investing time in building and maintaining them.  
This could lead us to ask, "Why bother?"  
That's not the right question though. The real question we should ask is, "What are we building?"  
It is extremely important to understand exactly what it is that we're trying to build. To understand it not just as an end product, but also as a collection of functionality.  
I've been in the situation where I created soemthing that worked by accident. I understood why it happened, in post, but I didn't expect it.  
This is not a good thing.  
As i've learned about about writing testable software, I'm starting to see testing in a different light.  
There is one primary goal of having tests:  

####Tests specify exactly what should happen.
The other goal having tests, to be sure that nothing has broken, is a sub goal of that first point.

Writing tests forces us to think through what we expect the application to do in various cases.
If we expect Input A to result in Output B, but we don't have a test for it, then its not functionality, its an accident.

I think this is important.
