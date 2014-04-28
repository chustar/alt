I open sourced Now Readable.  
I didn't want to charge for it (since its a client for Readability), didn't care about the code (its a glorified REST client); and its not that successful.  
Actually, I said I didn't care about the code, but that's not exactly true. I felt attachment to the end product that I built, but I do care about the code that I wrote. I care that it looks good, runs as well as possible and is easy to understand.
I think I wrote reasonably clever code (I think) but I'm still a little wary of releasing it out there, since its probably embaracing to other people.
In the end, I open sourced it because someone asked me to.
They asked me to, and I had no compelling reason not to.  
That's about it.  

That being said, I'm dissapointed in myself and the design of my project. I didn't think through this possibility when I created the project, and now its coming to bite me. 

* There are no tests.
* The code isn't even testable (funny because I'm an SDET).
* Its ugly in a lot of places.
* A lot of the algorithms are incredibly inefficient.
* There's a lot of coupling between the API and the app that had to be manually seperated.

I also checked in API keys. Why? Why the hell did I do this?! Even when I was in WAMAD I knew better than to do this! What was I thinking when I did this the first time and why did I never fix it? I really actually want to ask past me about this, because I'm concerned that I let this happen.
Because of this mistake, I've lost the largest revision history in any project I own.