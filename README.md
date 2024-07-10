# My Current Attempt At A Minimalist SEO Website Testing Process

*Disclaimer: This is a frequently iterating process with plenty of ideas or processes that need to be fully fleshed out. And if you're reading this, there's still some data and screenshots to be added.*

There's plenty of information on the internet about "how to do SEO." What things are ranking factors, how you should link your content, what google is looking for, etc. A lot of that information is even good. But how many people who do SEO in some capacity actually know - how many have actually tested it? 

Without actually running a proper test you could argue it's all technically guesswork.

This is why when I came across [Kyle Roof's ideas on testing](https://www.linkedin.com/posts/kyle-roof-seo_seo-seotests-seoscience-activity-6894357516210327552-u5Pt/?trk=public_profile_like_view)I almost immediately got a test site propped up and started running tests. The frequency of the tests quickly died off however. I'd build a process that ultimately was too cumbersome to easily set up and run a test, and between work and other things I rarely tested things the way I wanted. 

This V2 iteration is an ongoing process to systematize this as much as I can in order to keep the testing (and learning) flowing as smoothly as possible. 

## Setting Up Your Testing Environment
***First and foremost I've got to reiterate that I first came across this idea via Kyle Roof. I didn't make up the actual testing process on my own.***

[How To Run Clean SEO Tests - Kyle Roof](https://hvseo.co/blog/how-to-run-clean-seo-tests/)

The process simplified is as follows. Get yourself a nonsense domain and a nonsense keyword with **zero results**. 

![image ](https://github.com/krutzar/my-seo-testing-system/assets/28541671/fe5bbf9b-f2dc-4599-a198-b37c4e363ece)

This gives you a clean environment to run a test. From here you can publish pages on that website, using lorem ipsum and inserting your gibberish keyword to get those pages indexed. This allows you to make changes and compare different variables in about a clean an environment on Google's algorithm as is possible. 

## Testing Methods

Right now I have primary test methods. 
1. Just like Kyle Roof's linkedin post above, rank 5 pages and change something on the 3rd. 
2. Publish pages with different variables changed to see their ranking order, and then try to reverse or change their order. 
3. Some variation of this on a non-dedicated-test site to test other factors (I'm still sorting this one out...)

### Rank 5 Pages, Change the 3rd. 
The idea here is to get 5 identical pages ranking on your target keyword. This sets up the environment for you to make a change and see how it affects the rankings. 

By making changes to the 3rd, such as adding words or extra keyword insertions, you can see how it changes the middle result. Then you can revert the changes to see how the algorithm reacts. 

For example, below is a test on word count. In the below screenshot all of the pages are identical, each with 800 words of lorem ipsum text, and the keyword placed once in the first paragraph. 

From here, I went to the middle option and added 200 words of lorem ipsum to see how it reacted. 

From here I can continue experimenting. Does a keyword in the H1 outrank extra words? Does more words always work or is there a band outside the current pages in which a page will rank worse? 

### Publishing Multiple Variables
The other ideas is to take several pages, each with a different variable, and publish them all to see the order in which they rank. 

After things have ranked you have part of the answer, though their order doesn't always give a clear answer. Now you try to change results by switching variables. 

Below is a super foundational (and also via Kyle Roof, credit where credit is due) test looking at various ranking factors. 11 pages were published, each placing a keyword in a different location on the page, and only in that location. 

Each letter corresponds with the letter in the page's meta-title. 

**Ranking Factors & Their Pages**
1. a. Meta title
2. b. Meta description
3. c. H1
4. d. H2
5. e. H3
6. f. H4
7. g. First paragraph
8. h. Last paragraph
9. i. Image alt attribute
10. j. Bolded text
11. k. URL

And here's how they ranked: 

Next step would be to change around items. Let's remove the keyword from the first paragraph in G, and place it in the H1. And do the opposite for C, removing the keyword from the H1 and placing it in the first paragraph.

### Live Site Testing
This is more of a placeholder than anything. I'd like to create a similar testing environment to run on a live site with other ranking content. Less controlled of an environment, but allows for testing other things like theories related to "link juice" for example...

Outside of the personal reminder to actually get this put together, I don't have much more to put here. I guess come back later if you're reading this? 

## How I'm Doing It: My Workflow and Tech Stack
I wanted to keep this relatively straightforward but still keep some sort of graphical interface to use. Through some research I landed on Ghost and hosted it on a DigitalOcean droplet. 

All it took was a bit of setup through DigitalOcean and stripping down a Ghost theme to have a barebones and easy to manage environment for running these tests. 

From here I am manually keeping track of data and results in a document. I'm working on a more proper framework and workflow for tracking new and old data, but at this point it's relatively unrefined and just a markdown document...
### List of Tools And Resources
- [Ghost: The best open source blog & newsletter platform](https://ghost.org/)
- [DigitalOcean | Cloud Infrastructure for Developers](https://www.digitalocean.com/)
- [Lorem Ipsum Generator (generate # of paragraphs, words, or characters)](https://www.lipsum.com/)
