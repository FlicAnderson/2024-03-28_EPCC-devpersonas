# 3min Lightning Talk Prep 

## Slide Design: SWIPE 

Style:  
  - visually simple, without too much clutter
  - sans-serif font, > 24pt
  - bold for key points and takeaways
  - no animations / video clips / sound    

Words:  
  - 5-7 lines of text
  - 5-7 words per line only
  - ONE IDEA PER SLIDE - signpost ideas, don't use them as notes for my talk   
  - (optional: bitly for the slide? Probably not unless it's a link to the poster in this case)
  - any refs should be readable and at the bottom of the text; no more than a couple per slide or you've got too many ideas in the slide
  - CAPS are read SLOWER than lower case text; also, don't be shouty!  

Images:  
  - Graphs need to be presented SLOWLY, and explained SLOWLY and carefully; the audience hasn't seen it before, the presenter knows it inside out. Give them time.
  - You need to give enough time for audience to take in the content of the plot: explain axes, relationships, (obvs outliers), takeaway.
  - graphs should be uncluttered and as simple as possible
  - ONE per slide tbh
  - use images / photos to break up presentations if there's lots of text/data/dry content and make things relatable.
  - maintain same style of images throughout.  

Palette:  
  - aiming to follow EPCC branding largely (white background, dandelion highlights, epcc navy text/lines, + university red for emphasis/titles.)
  - think about accessibility of content for colour-blindness/screen reading etc  

Extras:  
  - could bring in bulletpoints slide by slide to emphasise each point if there are several and to avoid overloading audience with sudden wall of text



## Talk Prep:  

### Key point I want to get across:  
(come see my poster; my poster is interesting; you will benefit from coming to see my poster)  

There are different ways of assigning tasks
 

### Story of my talk:   

Introduce myself / why am I entitled to talk about this? Give my credentials    

#### Background / why is this relevant to you?:   
Research software research is a recent field  
But almost everyone in research uses or writes research software  
Every researcher I speak to agrees that academic code is usually terrible...  
So why is it so bad? How can we fix it?   
To fix something, you need to know what's going wrong: that's research software research.   

#### Methods: My research goals: 

Describing the landscape  
What are the common RS devt practices? 
(Do they apply to all projects? All developers? All fields of research?)

Focussing on people first - looking at the developers. 
To be able to communicate about something and discuss it, you need to be able to name key concepts and describe it.  
For my purposes, looking for groupings of ways people interact with their RS codebases

Why not talk to them? 
People don't always tell you what they're doing accurately - survey data is intensive to obtain, and a lot of these ideas are complex!

#### Methods: my actual methods:   

What did I do instead? 
Mining data from research software repositories.  
Harder to unpick the 'why' but gives a good idea of the 'what'/'how'. 

Selected a group of 10 large repos: developers > 6 (average is much smaller but for proof of concept work I've started with larger repos more likely to show clear differences between groups of devs).

Grabbed data about how developers use the features in the repository and how much code they add/change to it (in 'commits').  

GitHub allows users to create items called 'issue tickets' and 'pull requests'. 

Issue tickets are essentially discussion pages centred around a particular feature, task or bug within the code. 
They don't actually change anything in the code, but they can help organise and prioritise development tasks.  

Pull requests are a type of item which relate to chunks of code that a developer might want to add to the main codebase. 
These tend to be created to add new features, or fix problems, and can sometimes relate to specific existing issue tickets. 
Because pull requests change the codebase, they are potentially risky and could break things as well as fixing things... 

These features can give us a tentative proxy measure of 'developer responsibility' if we look at whether one or both types (or neither!) of these items were assigned to each developer.

Assignment doesn't equal activity, but that's where we can bring in 'commit' data as a tentative proxy for 'activity' within the codebase.  

Q: How do these measures of responsibility and activity interact? Are the developers assigned both types of item any different to developers in other categories? Can we identify any 'superstar' developers using these measures?   

Assignment can be categorised very basically as adding someone's name to an item (perhaps to ask them to lead on this, do the work, or to let them know about this item): 

![29a77179-35df-454c-b6af-4cb2ba04e281](https://github.com/FlicAnderson/2024-03-28_EPCC-devpersonas/assets/5812129/3fff5024-5c93-45d7-8dcc-69b9dd20451d)

We can place each developer into one of 4 categories. 


#### Results:  

Amongst these 10 larger repositories I'm looking at, they all assigned at least some of their issues and pull requests.  

Assignment distribution: 
![image](https://github.com/FlicAnderson/2024-03-28_EPCC-devpersonas/assets/5812129/90fc6353-a572-4bc8-b7b3-65591721152a)

- most developers don't get assigned any items
- of those who are assigned something, it's most likely to be just issue tickets (less 'responsibility' than PRs), with about a 5th assigned to 'both' issue tickets and PRs, with only a few folks assigned to only pull requests and not issue tickets (most pull requests tend to be related to issue tickets, which might explain why this is rarer?)
- not everyone is assigned the same: this is interesting because presumably there's some underlying difference which explains why?  

Average commits per developer by category: 
![image](https://github.com/FlicAnderson/2024-03-28_EPCC-devpersonas/assets/5812129/bec2b4ff-bfcd-4b50-94c1-8ce280cde039)

 - looking at the averages of commits within each of these categories, we can see that the mean number of commits for developers who are assigned both types of item is MUCH higher than that of any of the other categories - even though the majority of our developers don't get assigned to anything!
 - the 'both' category developers also out-commit their single-item-type colleagues, so we know it's nothing specially related to assignment to one of these types of item (e.g. being assigned pull requests doesn't automatically make you a committing legend for example).
 - the standard error lines on the bars show us that the standard deviations of the samples here are really different, even accounting for the sample sizes.

So it looks like there's some real differences going on amongst our developers - dare I say, are groupings starting to form? 


A to our Q: the developers assigned to 'both' types of feature are much more active within the codebase! This suggests a positive correlation between the two measures.  

But is this really the case?  


#### Call to Action:
Come to my poster to find out whether this is really the case, and what I plan to do to investigate further!

Thanks for your attention! 
(give my name and poster location) 



#### Concepts I need to make sure I explain:  
  - RS
  - repositories s.a. github
  - issue tickets - these are items where 
  - pull requests - these are branches of code which a developer wants to be added to the codebase 
  - assignment categories
  - commits
  - 10x programmer concept  
  - 'developer personas'    
 

### Pause points in my talk:   
  - context  
  - key graph 
  - takeaways   

### Length: aim to finish at 2min 50sec  







## Stuff NOT to include: 

#### Next Steps  

 - clustering developers into 'personas' by their practices (e.g. those assigned more 'responsibility' with more PRs + those who are more active in terms of commits == 'superstar developers' vs devs without assigned items and who have low commit numbers?)  
 - combine with code analysis tools to look at correlations with various 'code metrics' - do 'best practices' result in 'high quality code'?
 - compare to 'citations' and 'users (contributors not core-devteam)' of the software and 'usage (via forks, stars, watching etc)' with repo practices to check correlation: do 'best practices' result in 'widely used' code?  
 - do projects with specific persona types of developers onboard create 'more successful' projects than others? (considering metrics such as usage, citations, code quality)  
 - combine developer survey data + repo data to combine 'what' and 'why'!  

'Threads' to add to the clustering:  
  - external user vs developer?
  - mentions in issue tickets
  - commit frequency
  - average code files touched per commit
  - average time to close issue ticket / PR


Future work: users vs devrs/users; 

