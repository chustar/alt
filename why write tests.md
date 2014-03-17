why write tests?  
looking at a project with a huge set of test cases that are fragile and often break for expected reasons, it is sometimes hard to justify investing all the time it takes to build and maintain tests.  
so why bother?  
the real question we should be asking is, what are we building?  
it is extremely important to understand exactly what it is that we're trying to build. to understand it, not just as an end goal, but also as a collection of functionality.  
i used to think it was a good thing when i wrote code that worked by accident. i understood why it happened, but i hadn't expected it to do that when it happened.  
as i've learned about about writing testable software and also writing tests for software, i'm starting to see testing in a different light.  
there's two goals to having tests:  

- to be sure that we haven't broken anything.
- to know what we're actually building.

the first part is straightfoward, we write tests, then make changes. if the test fails, we broke something.
the second part is a little more nuanced to me.  
the second one is more spec oriented. writing test cases allows us to think about what we're trying to build before hand. all the features we want to have in the application should be explicitly called out as a test case. if we don't have a test case for it, it shouldn't work.
this seems really important. we need to know for a fact that everything we're building works exactly as we expect it to.  
this is a little ambitious, but i think if the application does something it wasn't expected to do, the test should fail.
if a note taking application is explicitly designed to support adding notes from one page, but then accidentally also supports adding notes from another page, now there's no coverage for that other scenario. that other way of adding notes could break, and no one would know, because no one knew to go look.  
this conflicts with my previous thinking on how certain micro interactions should work. i was of the opinion that the height of user experience is to build a bunch of pipelines and allow the user to connec them as they see fit. A lot of incredible things have been created that only exist because someone provided a series of tools that know how to talk to each other, and then other people taught those tools what to say.
i think that's still true, the problem is that we still need to be somewhat strict about how we talk. even if we don't know what users will use our tools for, we need to be clear and driven about how they'll use them.  
at the end of the day, there should be one way to do it, adn that way should have a test written for it.