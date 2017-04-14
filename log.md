# 100 Days Of Code - Log


### Day 102: April 12th, 2017

**Today's Progress:**

   Continued working on Treehouse's track about Core Ruby and writing to files use the `File` class.

**Time Logged:**

   1.25

**Thoughts:**

   Writing to files using the `Marshal` class to "save" data seems pretty cool

--------

### Day 101: April 11th, 2017

**Today's Progress:**

  Started a new section on what's included with Core Ruby and the Ruby Standard Library.

**Time Logged:**

   .75

**Thoughts:**

   Documentation specific and what modules are included in the core install.

--------


### Day 100: April 10th, 2017

**Today's Progress:**

   It's here! Day 100!!!

**Time Logged:**

   3.5

**Thoughts:**

   Today was really focused on summarizing everything that I have learned and built on this last 100 days in my [blog post](https://medium.com/@garret_s/what-i-learned-after-completing-my-first-100daysofcode-ef85799a2212). I seriously can't believe that I made it 100 days straight. I feel pretty damn accomplished right now.

--------

### Day 99: April 9th, 2017

**Today's Progress:**

   Day 99 woot woot!!
   Updated my personal site. Got some new sections updated and will work on deploying my new branch to GH-Pages.

**Time Logged:**

   1.75

**Thoughts:**

   Today was mostly about getting some of the "still in progress" sections pulled out and refactoring some of the Sass stuff. I really tried to get my jQuery bounce animation going on the pointer of the main page but no such luck. I was able to find out that it appears to be an issue with the function I was using being outdated on the latest version of jQuery that I was pulling down so I'll have to look into that.

--------


### Day 98: April 8th, 2017

**Today's Progress:**

   Continued to churn through more ruby module tutorials on Treehouse.

**Time Logged:**

   1

**Thoughts:**

   Finished up finally the Modules section and I can see these patterns in lots of ruby code I have looked at previously. Makes sense to group a lot of functionality together so they can be applied (extended or included) into other classes.

--------


### Day 97: April 7th, 2017

**Today's Progress:**

   Dove more into the RSpotify ruby gem and looked into a lot more of the documentation. Focused on authenticating with my credentials and tried to make a playlist.

**Time Logged:**

   1.25

**Thoughts:**

   I was able to successfully "log in" with during an IRB session with my Spotify Client ID and Secret which allowed me to pull details from my own user profile. This was pretty cool and the first step in being actually being able to create a playlist from this gem.

   The issue I ran into when trying to create a playlist is that I need to send in some additional attributes when the request goes in. Specifically, I need to make sure that `playlist-modify-public` and `playlist-modify-private` are set to true. I'm not exactly sure how to do this in an IRB session as there isn't a lot of documentation around it other than -

   ```
   This method is only available when the current user has granted access to the playlist-modify-public and playlist-modify-private scopes.
   ```
   I have looked at the Spotify documentation around scoping but still coming up short. I'll see if I can crack it this weekend.



--------

### Day 96: April 6th, 2017

**Today's Progress:**

   More time in Treehouse going over Modules in Ruby.

**Time Logged:**

   1.25

**Thoughts:**

   Nothing crazy new to report.

--------


### Day 95: April 5th, 2017

**Today's Progress:**

   Did something totally new today - dove into the [Rspotify ruby gem documentation](http://www.rubydoc.info/github/guilhermesad/rspotify/master/) in the hopes to resurrect my Spotify app idea!

**Time Logged:**

   1.25

**Thoughts:**

   This was seriously a lot of fun. I primarily played around with it in `irb` but did actually setup the beginnings of a small app. Since I'm building it from scratch I ran into problems regarding the best way to store ENV variables. I have loked at [Figaro gem](https://github.com/laserlemon/figaro) but decided to go with the [dotenv gem](https://github.com/bkeepers/dotenv) as I have seen in use more frequently.

   It was super cool just playing around with all the data that is available through the Spotify API and how to access it with certain methods. I had no idea that level of information was available which makes me wonder why I haven't seen any cool apps use it. The documentation seems a little hard to follow and I'm finding that being able to read and understand documentation is a skill unto itself.

--------

### Day 94: April 4th, 2017

**Today's Progress:**

   Worked on Ruby modules again at Treehouse.

**Time Logged:**

   1.25

**Thoughts:**

   Still just chipping away at getting my Ruby knowledge up to snuff.

--------

### Day 93: April 3rd, 2017

**Today's Progress:**

   Re-focusing my time on my personal site to hopefully get it up and running soon (ideally by the 100th day of code).

**Time Logged:**

   1.75

**Thoughts:**

   I learned a very important lesson today about how CSS actually handles cascading and inheritance. I already know that I have too many CSS files being that I have full blown bootstrap in my project as well as a lot of custom partials but I kept running into issues where the bootstrap styling was overriding my custom css (although not all the time). What I found was that in my main `.scss` file where I was handling all my `@imports` I had bootstrap near the bottom which was the reason I was losing my custom styling.

   Essentially this...

   ```CSS
   @import "custom";
   @import "pre-header";
   @import "header";
   @import "work";
   @import "bootstrap";   
   @import "footer";
   ```
   Should of been this...
   ```CSS
   @import "bootstrap";
   @import "custom";
   @import "pre-header";
   @import "header";
   @import "work";
   @import "footer";
   ```

   ![alt text](https://media.giphy.com/media/3og0IMJcSI8p6hYQXS/giphy.gif "The more you know")

--------

### Day 92: April 2nd, 2017

**Today's Progress:**

   Aaaaaaaaaand that's a WRAP on the Michael Hartl - Ruby on Rails tutorial!!! Finished up the last chapter today.

**Time Logged:**

   1.5

**Thoughts:**

   It kind of feels weird that I'm done 😳.

   I have spent soooo much time on this tutorial and it's definitely surreal that I'm done with it. I want to write up a full blog post on it to really summarize what I have learned and how well this tutorial layed out how a Rails app is setup.

**Link to Work:***

   [Sample App!](https://radiant-stream-44428.herokuapp.com/)   

--------

### Day 91: April 1st, 2017

**Today's Progress:**

   Still plowing through Ch 14 of the Hartl tut. Close close close!

**Time Logged:**

   1

**Thoughts:**

   Got the feed working today! Cool to see the last few pieces come together.

--------

### Day 90: March 31st, 2017

**Today's Progress:**

   A little Rails tut and then got to work with a co-worker (Matt D.) on writing some integration tests at work in the QC environment on one of our main applications at work.

**Time Logged:**

   2.25

**Thoughts:**

   During lunch I started to dive into how the Hartl tut showed how AJAX is used for some requests so the page doesn't have to refresh - which was interesting. Also, was pretty excited to be able to see how our actually dev team writes integration tests. I got to work with Matt on that for about 1.5 hours and while we didn't get to fully complete one, I was able to get really close and completely understood how the test was written. He gave me some good feedback on how I was able to really understand what was going on and was impressed with it: definitely encouraging to hear!

--------


### Day 89: March 30th, 2017

**Today's Progress:**

   Just continuing this Hartl Rails tut. Getting suuuuuper close to finishing.

**Time Logged:**

   2.25

**Thoughts:**

   Really getting the hang of writing some of these test as one of the exercises was to just write an integration test without a lot of setup and I was able to do it on the first try. What WHAT!

--------


### Day 88: March 29th, 2017

**Today's Progress:**

   Worked on some of the Treehouse Ruby Modules lessons and then a little DevTips front end jazz.

**Time Logged:**

   1.25

**Thoughts:**

   Long day today with the kids field trip so I was pretty tired - hard to take in a lot of new info. One thing that was covered in the Treehouse training was the difference between `extend` and `include` for modules. It seems that `include` just allows you to use the modules methods on any instance of the class but `extend` only extends the methods to the class itself. I'll have to confirm but that's how I understand it.

--------

### Day 87: March 28th, 2017

**Today's Progress:**

   Circled back to the Hartl tut to keep moving forward on the following users feature.

**Time Logged:**

   2

**Thoughts:**

   Web interface is done now for following/unfollowing users and works well. Also finished the partial for displaying all the users that a selected user follows and how many followers they have.

--------

### Day 86: March 27th, 2017

**Today's Progress:**

   I was feeling a little lagging in my Ruby so I went back to Treehouse tonight and started going over `Modules` and how they work.

**Time Logged:**

   1.25

**Thoughts:**

   Again, I really like how Ruby is set up and some of the advanced stuff (at least for me right now) seems to be with-in grasp. One area that seems like I should *really* get a handle on is the `Enumerable Module`. I have already seen a lot of these methods in the Hartl tutorial but I don't recall ever seeing something like:
   ```Ruby
   class SomeClass
     include Enumerable

     attr_accessor :thing_one, :thing_two

     # Code to follow...

   ```
   ...which makes me curious if there is some sort of Rails "magic" at play that already has something setup to have that module included. I'll have to look into that one.

--------


### Day 85: March 26th, 2017

**Today's Progress:**

   Continued working through Ch 14 of the Rails tut. The data modeling stuff isn't so hard to grasp at this point but definitely complex.

**Time Logged:**

   1.5

**Thoughts:**

   Nothing crazy to report but yup still working through this bad boy so I can get it finished up.

--------

### Day 84: March 25th, 2017

**Today's Progress:**

   Continued working on Ch 14 of the Rails tut but more importantly went to [Minnebar](http://minnestar.org/minnebar/) today!

**Time Logged:**

   1.25

**Thoughts:**

   I can't say enough how great an experience Minnebar was. Such an awesome, welcoming, and informative community. I learned a lot about the new CSS Grid layout method. This seems like it will make creating a responsive site without relying on Bootstrap much much easier. The speaker, Tim Smith, was great, knowledgeable, and super friendly after the session. I'm going to see if I can play around with CSS grid on [my personal site](http://garretsaarinen.com) soon.

--------

### Day 83: March 24th, 2017

**Today's Progress:**

   Started the final chapter (14) of the Hartl Rails Tutorial - Following Users.

**Time Logged:**

   1.25

**Thoughts:**

   This chapter, as even stated by the author, is going to have some harder concepts to understand especially around data modeling. So far it hasn't been too out of reach though as I have been exposed to this a lot at work with various projects and reporting.

--------


### Day 82: March 23rd, 2017

**Today's Progress:**

   FINISHED on Ch 13 of the Hartl tutorial. [It's alive and you can sign up!](https://radiant-stream-44428.herokuapp.com/)

**Time Logged:**

   2.5

**Thoughts:**

   Fully implemented the mircroposts aspect and have it fully rolled out to Heroku. One small issue with my seed data is that there is a lot of it - like a lot. For some reason when I ran the script in the fixtures file it didn't create 50 posts per user, it created 4,950 ... per user. Not that it's a big deal but it just took a while after I ran `heroku rails db:seed`.

   The biggest technical hurdle was getting the Amazon Web Services stuff configured which was my first introduction to it as well. This was set to be quite a stretch of my technical sophistication as stated even by Hartl. I luckily was able to find this [Stackoverflow post](http://stackoverflow.com/questions/28465206/how-to-grant-permissions-to-aws-user-for-hartls-rails-tutorial) that helped prep me with what I need to do and alleviated some of the initial frustration. I "somewhat" understand what I setup with AWS but not thoroughly. Would be best to revist this with someone who has a better understanding at some point to help explain what a bucket is and why it's needed on the app. I assume it has to do with cloud storage for file uploads and what not.  

--------


### Day 81: March 22nd, 2017

**Today's Progress:**

   Continued working on Ch 13 of the Hartl tutorial.

**Time Logged:**

   1.75

**Thoughts:**

   Was able to get the test issues figured out from the previous night. Also, was presented with some less straightforward test writing and was able to figure it out pretty easily looking at previous examples and knowing where to look at other code I have written. Felt good to quickly move on from the initial struggle.


--------


### Day 80: March 21st, 2017

**Today's Progress:**

   Continued working on Ch 13 of the Hartl tutorial.

**Time Logged:**

   1.25

**Thoughts:**

   Continued getting those Microposts setup. Got to the point where I now am writing tests and I again ran into some issues with getting an integration test passing. I'll have to look into the errors more because they don't seem to be an issue with my syntax of the test.




--------


### Day 79: March 20th, 2017

**Today's Progress:**

   Continued working on Ch 13 of the Hartl tutorial.

**Time Logged:**

   1

**Thoughts:**

   Continued getting those Microposts setup. Nothing really new to report - just chugging away.

--------

### Day 78: March 19th, 2017

**Today's Progress:**

   Continued working on Ch 13 of the Hartl tutorial.

**Time Logged:**

   1

**Thoughts:**

   Continued getting those Microposts setup. Worked on the views for creating them and will start to break up the home page view with some partials.

--------

### Day 77: March 18th, 2017

**Today's Progress:**

   Continued working on Ch 13 of the Hartl tutorial.

**Time Logged:**

   1

**Thoughts:**

   Still working through the mircropost section. Played around a little with the Faker gem and I didn't realize how much cool stuff was in there. There is even some Lord of the Rings related methods for faking data. Super cool.

--------

### Day 76: March 17th, 2017

**Today's Progress:**

   Continued working on Ch 13 of the Hartl tutorial.

**Time Logged:**

   1.25

**Thoughts:**

   Started building out how the app will work with Microposts.

--------

### Day 75: March 16th, 2017

**Today's Progress:**

   Continued working on Ch 13 of the Hartl tutorial. Started to go through the Micropost data model and how getting it's dependencies setup on the User object.

**Time Logged:**

   1.25

**Thoughts:**

   Nothing crazy to report but I do like working with additional models and tying them together. It's way more interesting than diving super deep into some of the security and setup stuff in the last few chapters. Nice to see the app will start to function.

--------


### Day 74: March 15th, 2017

**Today's Progress:**

   Started Ch 13 of the Hartl tutorial and then also ran through [this quick and awesome tutorial](https://dev.to/philnash/google-spreadsheets-and-ruby) using a Google Spreadsheets Ruby gem.

**Time Logged:**

   1.5

**Thoughts:**

   I really liked working through the Google Spreadsheets Ruby gem tut. I was able to get the demo working without any big issues (woot!) and it was cool to use something I am familiar with in the real world. I can see how this could actually be applicable to me in the real world. Maybe I could write a script that uses the Clarizen API and dumps some of the data into our resource forecasting spreadsheet, eh eh eh!?!

--------

### Day 73: March 14th, 2017

**Today's Progress:**

   Hartl tutorial - Ch 12

**Time Logged:**

   1.5

**Thoughts:**

   Finished Ch 12. Didn't log in a few day so I don't have a ton to write about. Really just trying to get this tutorial done so I can move on to something API related. Received a good piece of advice from a co-worker and I should be checking to see if there are ruby gems available for APIs I'm interested in working with. It would be a lot simpler than trying to write it all myself.

--------


### Day 72: March 13th, 2017

**Today's Progress:**

   Back to Treehouse - yay!! Finished up building the address book (although I was stuck on one exercise and will have to come back)

**Time Logged:**

   1.25

**Thoughts:**

   The more and more that I do core Ruby, I really like it. Need to figure out some practical ways to start using it at work so I keep it fresh. Ruby just seems like da best.

--------


### Day 71: March 12th, 2017

**Today's Progress:**

   Worked on my site for awhile tonight. Played around with some different landing page designs and found some cool alternatives.

**Time Logged:**

   1

**Thoughts:**

   I randomly was thinking about that effect you get from images/text on old 3d movies and wanted to see if I could replicate it. I found a good site going over it in CSS and found it's called the [Anaglyphic effect](http://line25.com/tutorials/how-to-create-a-cool-anaglyphic-text-effect-with-css) and it's not too hard to replicate.

   Also, struggling with getting images sized correctly as it appears too big on my site. Seems like that should be easy but it's proving difficult.

--------

### Day 70: March 11th, 2017

**Today's Progress:**

   Finished up Ch 12 today of the Hartl tutorial and it's cool to see how this is the bones of a full fledged web app with users.

**Time Logged:**

   1.5

**Thoughts:**

   Getting there! I have started to think about how I can use this tutorial to actually build out a real app that does ... something! Since this tutorial goes through created the bare bones of the an app and how to manage users, security, etc. I now just need to figure out something cool for it to do.

--------


### Day 69: March 10th, 2017

**Today's Progress:**

   Worked on Ch 12 of the Hartl tutorial today a bit at work.

**Time Logged:**

   .75

**Thoughts:**

   Nearly complete - only 2 more chapters left. Today was all about password resets.

--------

### Day 68: March 9th, 2017

**Today's Progress:**

   Worked on more DevTips stuff. Was suuuuuper sick today.

**Time Logged:**

   1

**Thoughts:**

   Seriously - I was all 💩 all day. Hard to focus.

--------


### Day 67: March 8th, 2017

**Today's Progress:**

  Smattering of a few things:
  - New fonts and played with jQuery on my site
  - Updated formatting and CSS on the site
  - Looked at some jQuery tutorials with DevTips

**Time Logged:**

   1.5

**Thoughts:**

   Really liking [Googles font site](https://fonts.google.com) and it makes it super easy to play around with different fonts.

--------


### Day 66: March 7th, 2017

**Today's Progress:**

   Ch 12 of the Hartl Tutorial and DevTips jQuery stuff.

**Time Logged:**

   1.5

**Thoughts:**

   Not much to report. Started with the password reset stuff in the Ch 12 of the Hartl tutorial and re-using a lot stuff from the last chapter with ActionMailer.

   Also really liking the jQuery tutorials from DevTips. Fun stuff 😎

--------


### Day 65: March 6th, 2017

**Today's Progress:**

   More DevTips but branched out a little and checked out how I should create some responsive emails in HTML and CSS. Also, worked on my site a little and started to think about how I want my footer to look.

**Time Logged:**

   1.25

**Thoughts:**

   I'm going to start to take this email/HTML knowledge and update the Project Closing emails out of Salesforce at work so they don't look like garbage. Because, let's face it - they look like hot trash.

   One big take-away from working on my site is that I really need to start, even if briefly, sketching out my thoughts and design first. It's fun to play around with the design while I'm coding it but, it seems to go much slower.

--------

### Day 64: March 5th, 2017

**Today's Progress:**

   Felt like garbage so I stuck with some new DevTips tutorials. I started revisiting his [Build a responsive site from scratch](https://www.youtube.com/watch?v=D2W_oqMM19k&index=8&list=PLqGj3iMvMa4KQZUkRjfwMmTq_f1fbxerI) series which is what got me to check out Jekyll.

**Time Logged:**

   1

**Thoughts:**

   Tough to get my time today because I felt sick so kind of bummed that I only got in an hour. I need to remember to not push it so hard all the time - otherwise I'll stay sick.

   The more I observe other people programming the more I feel confident in my understanding of what they are doing. Like DHH said - "Read a lot of code, write a lot of code".

--------

### Day 63: March 4th, 2017

**Today's Progress:**

   Worked more on my site ( [garretsaarinen.com](http://garretsaarinen.com) ) and I got the new nav bar setup!

**Time Logged:**

   1.75

**Thoughts:**

   I'm loving the new navigation! I took influence from [this post on codepen](http://codepen.io/MightyShaban/pen/CIfdj) and I was successfully able to implement it on my jekyll site. I'm starting to really get the hang of where to put things in terms of folders and how to link to them appropriately in the head file. I have somewhat of a mess with all my sass/css and I know that there are css rules overriding each-other so that is my next big project.

--------

### Day 62: March 3rd, 2017

**Today's Progress:**

   Two main focal points today:
   * Finishing Ch 11 of the Hartl Tutorial
   * Working with Matt to get my machine setup for running evolution locally.

**Time Logged:**

   2.25

**Thoughts:**

   The second item proved to be quite the process. We worked for about 1.25 hours and got about what appeared to be half way through. Ran into a road block where I needed to work with cloud operations to get the right access so I'll pick it up next week.

--------


### Day 61: March 2nd, 2017

**Today's Progress:**

   Worked quite a bit today on the personal site. Finally got it deployed to Github pages so check it out here!
   [garretsaarinen.com](http://garretsaarinen.com)

**Time Logged:**

   2.25

**Thoughts:**

   I'm having a weird issue where my background image isn't loading on the github hosted version of it so I'm wondering if the file is too big for the repo. I have been learning some pretty sweet CSS stuff like how to have an all image landing page that is always 100% of the viewport but has content below it.

   Cool stuff

--------

### Day 60: March 1st, 2017

**Today's Progress:**

   A little Treehouse + DevTips. Again, another long day. I think after this week is over I'll get better at taking better notes and s t r e t c h i n g my mind.

**Time Logged:**

   1.5

**Thoughts:**

   Not much to report.

--------


### Day 59: February 28th, 2017

**Today's Progress:**

   More DevTips videos. Looooong day at work so I just wanted to get in what I could with his vids.

**Time Logged:**

   1.25

**Thoughts:**

   Not much to report.

--------


### Day 58: February 27th, 2017

**Today's Progress:**

   Got back to the Hartl Tutorial and worked more on Ch 11 - account activation and using the mailer. Also, researched and reconfigured some Github email issues messing with my contributions graph.

   Gotta get 'dem green squares! ✅

**Time Logged:**

   1.5

**Thoughts:**

   Still chugging along on the figuring out how the `ActionMailer` is used in a rails app. Regarding the Github email issue - I'm slightly annoyed (at myself) that I had my work email associated locally on my machine with my git profile and that - in turn - was not counting my daily commits to my contributions graph on my Github profile page. I know it's somewhat inconsequential, but when I'm working everyday on something it would of been cool to see all those green squares 😎.

   Curious how that will work when I end up using my machine for actual commits on repos at work?

--------

### Day 57: February 26th, 2017

**Today's Progress:**

   More time working on my site (Jekyll, Sass, Bootstrap, etc.).

**Time Logged:**

   1.5

**Thoughts:**

   Finally got the Bootstrap stuff to show up correctly! Having to create the files and folders manually really are helping me understand how Jekyll works. My main problem was when I introduced Sass and how that needs to compile first before getting compiled again in the `_site` folder.

--------

### Day 56: February 25th, 2017

**Today's Progress:**

   Switched it up - tried to actually build something. Started working on my personal site again and tried to get Bootstrap working with Jeykll.

**Time Logged:**

   2

**Thoughts:**

   Today was primarily about getting the environment setup. I haven't pushed it to git yet because it's not quite in good enough shape. Running into issues actually getting my `SASS` to compile right in my `css`.

--------

### Day 55: February 24th, 2017

**Today's Progress:**

   I was late on logging this day so I don't have a lot of details. I know I spent most of it on the DevTips tutorial.

**Time Logged:**

   1.5

**Thoughts:**

   😬😬😬😬😬😬😬

--------


### Day 54: February 23rd, 2017

**Today's Progress:**

   Continued Ch 11 in the Hartl Rails tutorial and learned about account activation and starting to use mailers. A little DevTips at the end.

**Time Logged:**

   1.5

**Thoughts:**

   Interested to see how `mailers` are used in Rails and how they are applied. Once I have a better understanding I want to see how or if they are implemented at work. I assume not since I can't image the native mailers can handle what our app does in regards to sending email but we'll see.

--------


### Day 53: February 22nd, 2017

**Today's Progress:**

   Treehouse Ruby Basics. Started the "building an address book" course and learned more about designing classes.

**Time Logged:**

   1.25

**Thoughts:**

   Ruby rules!

--------

### Day 52: February 21th, 2017

**Today's Progress:**

   FINALLY finished Ch. 10 of the Hartl Tutorial. That took a pretttaaayy pretttaaayy pretttaaayy long time. Just under 1 month.

**Time Logged:**

   1.75

**Thoughts:**

   Man does it feel good that I have finally moved on from that damn chapter. I did push both my original and new branches up to bitbucket so I can use their `compare` feature to see if I can actually learn what my mistake was.

   While this chapter was a huge pain in the ass, I can say that I honestly learned a ton. Lots of debugging skills, how to re-write tests, how to really navigate the app, and just generally understand more about how the whole things works. Definitely going to remember this one!

--------

### Day 51: February 20th, 2017

**Today's Progress:**

   Completed the Ruby Blocks course of the Treehouse Ruby Basics and did the short Enumerable's workshop.

**Time Logged:**

   1.5

**Thoughts:**

   Getting down there with what's left of the Treehouse Ruby courses. Now it has a few options for me to do as the next course instead of just the standard next course. Watched a few trailers on my next options and really interested to see what the Sinatra one is about as I'm pretty deep in the Hartl Rails tutorial.

--------

### Day 50: February 19th, 2017

**Today's Progress:**

   Continued working on Ch 10 and I *think* I made it past where I was getting tripped up on my previous branch.

**Time Logged:**

   2.5

**Thoughts:**

   So I'm knocking on wood but I believe I made it past my previous issues on this debugging excursion. Spent a lot of time today just re-doing Ch 10 and it feels pretty good to get past the point where I got stuck before. Once I'm completely finished with this branch, I'm going to compare it to the previous one and see where all the issues where - should prove to be quite a learning experience.

--------

### Day 49: February 18th, 2017

**Today's Progress:**

   Continued working on Ch 10 of the rails tutorial on a new branch.

**Time Logged:**

   .75 hours

**Thoughts:**

   Kind of bummed I didn't hit an entire hour today but it was tough to just get in the time that I did with my parents being in town.

--------

### Day 48: February 17th, 2017

**Today's Progress:**

   Really went to town on debugging my editing users branch with Eric at code club. Made some progress in figuring out where some of the redirects where happening but ultimately decided to blow up this branch and start over.

**Time Logged:**

   1

**Thoughts:**

   Yup. Going to start over but excited to learn more about `git diff` and use that to see where my issues were once I get a new branch working.

--------


### Day 47: February 16th, 2017

**Today's Progress:**

   I forgot to put in my log what I did ... now I can't remember. 😁
   I'm pretty sure it was about Ruby blocks.

**Time Logged:**

   1.5

**Thoughts:**

   Ruby blocks are pretty sweet!

--------

### Day 46: February 15th, 2017

**Today's Progress:**

   More time on the [Enki app](https://www.enki.com/), did some trouble shooting on my test issues I'm getting with the Hartl tutorial Ch. 10, and watched some DevTips.

**Time Logged:**

   2.25

**Thoughts:**

   Nothing big to report. Just cranking away.

--------


### Day 45: February 14th, 2017

**Today's Progress:**

   More time on the [Enki app](https://www.enki.com/) and did some trouble shooting at work with Eric on my test issues I'm getting with the Hartl tutorial Ch. 10.

**Time Logged:**

   1.25

**Thoughts:**

   Nothing big to report. Just the fact that in my `users.yml` file in the fixures folder was giving me issues.

--------

### Day 44: February 13th, 2017

**Today's Progress:**

   More time on the [Enki app](https://www.enki.com/) and then continued with DevTips' [Design + Code tutorial](https://www.youtube.com/watch?v=FiJuoFg_Ipc&index=18&list=PLqGj3iMvMa4KeBN2krBtcO3U90_7SOl-A).

**Time Logged:**

   1.25

**Thoughts:**

   Did more of the Linux and Bash Shell exercises and I just love how unix operating systems are setup. They are so logical. I guess I haven't dove into a Windows based OS in a long time so maybe there are more similarities than I remember.

--------


### Day 43: February 12th, 2017

**Today's Progress:**

   Spend a little time on the [Enki app](https://www.enki.com/) and did some of their exercises. I also, continued the Treehouse Ruby tutorials (Booleans) and I take back the thought of this being an overview of previous things. Ended up finishing it up tonight

**Time Logged:**

   1.5

**Thoughts:**

   The more I use the Enki app the more I like it. Today I went through some of the command line/bash shell "workouts" and learned a lot. Also, the Ruby stuff in Treehouse I can tell is starting to ramp up a little the further along I get. I underestimated this section since it was presumably just going over booleans but it was starting to really put together a lot of the work from previous sections.

--------

### Day 42: February 11th, 2017

**Today's Progress:**

   Continued the Treehouse Ruby tutorials (Booleans) which has felt a little like an overview.

**Time Logged:**

   1

**Thoughts:**

   Nothing crazy to report. Just keep chugging along. 🙂

--------


### Day 41: February 10th, 2017

**Today's Progress:**

   Continued the Treehouse Ruby tutorials (Objects and Classes).

**Time Logged:**

   1.5

**Thoughts:**

   Had the day off so was able to spend a little more time on learning today. I feel like this section has been so impactful on my understanding of how all of these methods tie together. I definitely felt like I walked away from this section with a solid understanding of object oriented programing.

--------


### Day 40: February 9th, 2017

**Today's Progress:**

   Continued the Treehouse Ruby tutorials (Objects and Classes)

**Time Logged:**

   1

**Thoughts:**

   Didn't get a ton of time in today as I had to take an impromptu trip to the ER today 😬.

--------


### Day 39: February 8th, 2017

**Today's Progress:**

   Did some Treehouse tuts up in this piece. Finished the section on iteration and all the different flavors of that and then got into OOP and how Classes work in Ruby.

**Time Logged:**

   1.25

**Thoughts:**

   I got really excited when I found out the next section was about **Ruby Objects and Classes** as that is something that I really think needs to get solidified in my learning. While I have learned things in the previous sections, they have felt like review as I have started programming tutorials so many times in the past. And let's face it - almost all tutorials start with data types and how to manipulate them. Objects & Classes FTW!

--------



### Day 38: February 7th, 2017

**Today's Progress:**

   I dove back into debugging my test issues with Ch 10 of the Hartl rails tutorial and also rebuilt my repo in Github so it shows all my commits.

**Time Logged:**

   2.5

**Thoughts:**

   _On the Github side:_

   I had to create a new repository with my existing 100 Days of Code log because I didn't like how all my commits and streak were not showing up in my daily activity [because of the way that Github counts contributions](https://help.github.com/articles/why-are-my-contributions-not-showing-up-on-my-profile/). Essentially, working on a forked repo doesn't count??

   *On the debugging side: ...damn.*

   So progress has been made. Slow and frustrating but progress none-the-less. I finally was able to figure out what code was giving me redirect issues when running certain tests and it all comes down to the `correct_user` method in `users_controller.rb`.

   ```ruby
   # Confirms the correct user.
    def correct_user
      @user = User.find_by(params[:id])
      redirect_to(root_url) unless @user == current_user
    end
   ```
   I'm trying to figure out how to debug it or run a rails console in the test because I suspect that it's not working because the tests pass when I comment out the last line that uses the `redirect_to` method. This method is used as a `before_action` filter on the controller only on the edit and update actions.

   ```ruby
   class UsersController < ApplicationController
     before_action :logged_in_user, only: [:index, :edit, :update]
     before_action :correct_user,   only: [:edit, :update]
     .
     .
     .
   ```
   ...which now makes sense why only the test that were trying to edit a user were failing. Specifically,  the redirect issue was popping up after the test logged a user in, pulled in the user_edit path, and then when it ran `assert_template 'users/edit'` it would pull up as nil or www.example.com instead of www.example.com/user/12345678/edit.

   Anyways, it I figured out that is the specific part that is causing the issue but now I need to figure out WHY it's doing that.

   Also, I get new errors on some test that I somehow missed creating while going through the tutorial and I'm getting `BCrypt::Errors::InvalidHash:` errors. Will need to dive into that later.  


--------


### Day 37: February 6th, 2017

**Today's Progress:**

   Continued more with [DevTips stuff](https://www.youtube.com/watch?v=9XqFV9fy8SU).

**Time Logged:**

   1.25

**Thoughts:**

   Nothing crazy new to report.

--------


### Day 36: February 5th, 2017

**Today's Progress:**

   Focused on Treehouse tuts (working with iterating over hashes now and building a contact list app) and did more [DevTips stuff](https://www.youtube.com/watch?v=9XqFV9fy8SU).

**Time Logged:**

   1.5

**Thoughts:**

   Can't bring myself go back and debug more so I stuck with Treehouse and DevTips. I've been thinking more about front end development lately after all the DevTips vids and I just really like the instant gratification of manipulating the DOM (at least how easy Travis does it). Trying to figure out how I will fit that in after I get through the Hartl tutorial.

--------


### Day 35: February 4th, 2017

**Today's Progress:**

   Had to do something different. Went back to Treehouse and went over iteration with different types of loops.

**Time Logged:**

   1.25

**Thoughts:**

   Today was a little bit of review but it was good to solidify how iteration works in Ruby. It was interesting that `for loops` are used differently in Ruby and as such, not used frequently. I vaguely remember them being pretty prevalent in JavaScript.

--------


### Day 34: February 3rd, 2017

**Today's Progress:**

   Damn. Still debugging. Nothing new.

**Time Logged:**

   1

**Thoughts:**

   See "Today's Progress" 😑

--------


### Day 33: February 2st, 2017

**Today's Progress:**

   Groundhog's Day! I am still debugging 👏 these 👏 test 👏 issues 👏! Yup - Ch 10. Still.

**Time Logged:**

   1.5

**Thoughts:**

   So now I have 2 separate 'but related' test issues in the `user_edit_test.rb` file - `unsuccessful_edits` and `successful edit with friendly forwarding`. It all seems to be related to the `log_in_as` helper and it's doing a weird redirect. I keep getting these types of errors:

   ```
   FAIL["test_unsuccessful_edit", UsersEditTest, 619.0571372920022]
   test_unsuccessful_edit#UsersEditTest (619.06s) expecting <"users/edit"> but rendering with <[] test/integration/users_edit_test.rb:13:in `block in <class:UsersEditTest>
   ```

  It seems that when I run that method it loads this url:

   ```html
   <html><body>You are being <a href=\"http://www.example.com/users/762146111\">redirected</a>.</body></html>"
   ```
   The only thing that I can think of now that the issue could be related to is when trying to visit the `users/edit` path and how it is or isn't using the HTTP patch method.

   Thinking - thinking - thinking

--------

### Day 32: February 1st, 2017

**Today's Progress:**

   Running into a big issue with some tests in Ch 10 so I spent a lot of time debugging that and a little DevTips tutorial in the evening.

**Time Logged:**

   1

**Thoughts:**

   Went in and worked with a co-worker (Eric) to try and figure out the initial issue where the layout links test in the `site_layout_test.rb` file wasn't working. We got it to pass but found that I'm getting a weird redirect issue withe the `log_in_as` helper method.

   Ended up having to do a lot of real work late in the night so I ended my hour time with some DevTips videos so I could at least still get a full hour.
--------

### Day 31: January 31st, 2017

**Today's Progress:**

   Continued Ch 10 of the Rails tut. Got stuck on writing an integration test that now tests page layout links after a user has logged in.

**Time Logged:**

   1.5

**Thoughts:**

   For some reason the test doesn't see the link but it works for an end user so I must be writing something wrong. I originally thought it was something to do with my `routes.rb` file which was a tip from a co-worker (Matt) but alas, that didn't seem to solve it. Checking in with another one of the developers at work (Eric) tomorrow morning to see if he can help me figure it out.

   Got a little into the pagination stuff and seeding a bunch of users with the Faker gem which is pretty cool. I'll have to look at the documentation to see exactly how that works.

--------


### Day 30: January 30th, 2017

**Today's Progress:**

   More time on Ch 10 of the Hartl Rails Tutorial (creating a index page for all users) and then spent a good hour with DevTips watching more of his Design + Code tutorial.

**Time Logged:**

   2.25

**Thoughts:**

   I was finally able to figure out the testing issue I was running into with the `session[:forwarding_url]`. It turns out I was thinking about the problem wrong assuming it was supposed to have a value. I should of listened to my test errors (which were telling me it was nil) as it was supposed to that.

   Also, spent more time watching the DevTips tutorial and again - this is such a great series to just see how someone builds their site. It's getting me excited to dive more into some front end stuff once my Rails tutorial is done.

--------


### Day 29: January 29th, 2017

**Today's Progress:**

   Spent more time on core ruby with the Treehouse tutorials and starting to more of a solid understanding of `arrays` and `hashes`.

**Time Logged:**

   1.5

**Thoughts:**

   Really liking the Treehouse stuff the deeper it goes. I'm glad I ended up getting a full year subscription as I feel that this is something that I will leverage a lot. I like how they point you to the [Ruby Documentation](http://ruby-doc.org/).

--------


### Day 28: January 28th, 2017

**Today's Progress:**

   Got strep so was feeling pretty bleh and just focused on the [DevTips tutorial](https://www.youtube.com/watch?v=wzEl6XWNpK8) on how he built his own site. Super insightful stuff.

**Time Logged:**

   1.25

**Thoughts:**

   With being sick it was pretty tough to find motivation but that's when I have found that the DevTips videos hit me the most. Just watching him organize his files and watch his process is teaching me a lot in how to build and design sites.

--------


### Day 27: January 27th, 2017

**Today's Progress:**

   More of Ch 10 of the Hartl Rails tutorial. Continued to learn more bout how we will allow users to edit their profiles.

**Time Logged:**

   1

**Thoughts:**

   Worked on creating some helper methods to store url locations and how to redirect a user back to their profile when attempting to update another users page. Ended up getting stuck on one of the exercises that had me writing a test to check the value of the `session[:forwarding_url]` but couldn't figure it out. will have to come back.

--------


### Day 26: January 26th, 2017

**Today's Progress:**

   More of Ch 10 of the Hartl Rails tutorial. Today covered how to successfully allow users to edit their profile page in the app and got more specific into [TDD](http://agiledata.org/essays/tdd.html).

**Time Logged:**

   1

**Thoughts:**

   Nothing of consequence to report today. Tough to find time with being at home with a sick kid all day and then had to bring him to the Dr. at 7:30pm but squeezed a little time in. Good thing I don't have to work tomorrow.

--------

### Day 25: January 25th, 2017

**Today's Progress:**

   Change up - went back to Treehouse and did more Ruby tutorials. This time focused on how to interact with arrays and hashes.

**Time Logged:**

   1.5

**Thoughts:**

   It feels good to continue to bounce back and forth between the Hartl Rails tutorial and core Ruby stuff at Treehouse. I feel like this is a good mix to keep continuing where I'm focusing more of my time on actually building things but still spending (25%?) of my time on still learning the basics. The Treehouse classes seem to be solidifying concepts that the Hartl tutorial is exposing me to which I feel is a good system.

--------

### Day 24: January 24th, 2017

**Today's Progress:**

   Continued Ch. 10 and dove into editing users.

**Time Logged:**

   2

**Thoughts:**

   Switched up some of how the edit and signup forms are represented and moved the form parts into partials and used the `render` method in the .erb file. This initially brought up some issues in `invalid signup information` test that was in the `users_signup_test` integration test.

--------

### Day 23: January 23rd, 2017

**Today's Progress:**

   Finished Ch 9 and started Ch 10 of the rails tutorial. Ran into some issues with getting a test to pass and spent a good chunk of time on that.

**Time Logged:**

   1.75

**Thoughts:**

   Had issues with getting my `sessions_helper_test` working and had to comment out some code initially to do a commit. Then spent about 30 minutes the next morning looking into the test and I was able to figure it out. Crazy what a fresh set of eyes can do! It was a pretty simple issue where I was defining the variable `current_user` twice in one of the files being referenced in the test.


--------

### Day 22: January 22nd, 2017

**Today's Progress:**

   Still chugging through Ch 9 and hit a real hurdle today with an integration test but dove head first into regular variables vs. instance variables.

**Time Logged:**

   1.5

**Thoughts:**

   Hoooo boy - I probably got the smallest amount done today in the tutorial but holy crap did I learn a lot. Seriously, I feel a real sense of accomplishment right now!

   So first of all: I had to really dive into understanding the difference of instance variables and how they differ from regular variables. Even though I have seen frequently code like this:
   `var = something` vs. `@var = something`
   - -it never really clicked with me.

   It wasn't until I was required to update a variable to an instance variable on the `sessions controller` and I ran [into this post](http://stackoverflow.com/questions/10280801/normal-variables-vs-instance-variable-in-ruby-whats-the-difference) on Stackoverflow that I was able to really understand how they work.

   ```ruby
    class User
      def set_name
        @name = "Bob"
        surname = "Cratchett"
      end

      def hi
        puts "Hello, " + @name
      end

      def hello
        puts "Hello, Mr " + surname
      end
    end

   irb(main):022:0> u = User.new
   => #<User:0x29cbfb0>
   irb(main):023:0> u.set_name
   irb(main):024:0> u.hi
   Hello, Bob
   => nil
   irb(main):025:0> u.hello
   NameError: undefined local variable or method surname for #<User:0x29cbfb0 @name="Bob">
   ```
   This was big.

   The last part where I got extremely hung up on was actually getting the test to pass. Using the newly available instance variable of `remember_token` I finally figured out how to write a correct `assert_equal` test. Long story short - commas are super important. 🙄

--------


### Day 21: January 21th, 2017

**Today's Progress:**

   Continued to work through Ch 9 of the rails tutorial. Learned about how to shorten up `if ... else` statements.

**Time Logged:**

   1

**Thoughts:**

   Working up north at the wife's parents today so still making sure I get my time in! Big take-away today was learning about the `ternary operator` and how they shorten up writing `if .... else` statements.

--------


### Day 20: January 20th, 2017

**Today's Progress:**

   Continued back with Ch. 9 of the rails tutorial. For some reason my test were giving me issues but now they seem to be in order.

**Time Logged:**

   1

**Thoughts:**

   Basic stuff today - just trying to get time in!!

--------


### Day 19: January 19th, 2017

**Today's Progress:**

   Today was all about core ruby with [TeamTreehouse.com](https://teamtreehouse.com/library/ruby-collections/ruby-arrays/ruby-arrays) yo! Do you know about `case`s - because I do!

**Time Logged:**

   1.25

**Thoughts:**

   Not a ton to add here today. It was nice getting a reminder about using the `case` function as I have even seen that show up in some custom Clarizen workflows but only kind-of grasped it.

--------

### Day 18: January 18th, 2017

**Today's Progress:**

   Dove into Ch 9 of the rails tutorial and worked on the advanced log in stuff with permanent cookies.

**Time Logged:**

   1.75

**Thoughts:**

   This chapter is really stretching my technical understanding. It's really confusing as it gets into some of the more advanced Ruby stuff as well as how the app is setting up storing the permanent user session id and referencing it in the database. Also, after adding in the code in [Listing 9.9](https://www.railstutorial.org/book/advanced_login#code-persistent_current_user) my test should be red but they are passing. 😳

   Overall - this chapter has me feeling like ...

   ![I have no idea what I'm doing](http://i.imgur.com/QyuQiPD.jpg)

   Might have to just straight up repeat this chapter.

--------


### Day 17: January 17th, 2017

**Today's Progress:**

   Finished Ch 8 of the Rails tutorial and now have successful user log in and log out. Also, spent some more time going through the DevTips tutorial "Design + Code".

**Time Logged:**

   2.25

**Thoughts:**

   Felt good to get a large chuck of work done today. Ch 8 of the Rails tutorial seemed to go by pretty quick but I'm sure I will be well suited to go back and revisit it soon. Starting to understand how sites keep track of users being logged in using sessions and how to see them with the developer tools.

   Stating to also get itchy to really dive into updating and creating my own site after watching a lot of the DevTips shows. Need to finish the rails stuff first though!

--------


### Day 16: January 16th, 2017

**Today's Progress:**

   Continued some of the DevTips tutorials on building his own site. This is really great stuff from a design perspective. Really liking how he organizes his projects and will probably work to duplicate his structure.  

**Time Logged:**

   .75

**Thoughts:**

   This is a really great [set of videos](https://www.youtube.com/playlist?list=PLqGj3iMvMa4KeBN2krBtcO3U90_7SOl-A) for anyone interested in some great aspects of how to setup and create a personal site. While it's a bit more complicated in its setup *(using Gulp, Browsersync, Jade, SASS, etc)* it's still SUPER informative and very approachable.

--------

### Day 15: January 15th, 2017

**Today's Progress:**

   Changed it up and got back into playing around with my "personal site" using Jekyll. The more I play around with that framework, I really like it for static sites.

**Time Logged:**

   1.5 hour

**Thoughts:**

   Inevitably, this all brought me to watching more [DevTips Tutorials](https://www.youtube.com/channel/UCyIe-61Y8C4_o-zZCtO4ETQ) on CSS/SASS and that guy is awesome. Seriously, to me he is the Bob Ross of Web Development. Such a great teacher, funny, and genuinely caring.

--------


### Day 14: January 14th, 2017

**Today's Progress:**

   Continued Ch 8 of the [Hartl RoR Tutorial](https://www.railstutorial.org/book/basic_login) and then worked on some markdown and Atom stuff. Also poked around the spomodoro project to try and understand more about how it was created.

**Time Logged:**

   1.75 hour

**Thoughts:**

   Today I was able to get more into the user log-in stuff for the rails app - fun stuff. Also dove into how to do some command line stuff with Atom *(my new favorite text editor)* and I now can open files from the command line with just the `atom .` command. Cool stuffs.

--------


### Day 13: January 13th, 2017

**Today's Progress:**

   Continued Ch 8 of the [Hartl RoR Tutorial](https://www.railstutorial.org/book/basic_login). Finished the failed log in section and started working on how to get a user successfully logged in. Also, looked into a little more about Markdown and have updated the log.md file.

**Time Logged:**

   1.15 hour

**Thoughts:**

   Man - I ran into another testing issues *(that I was able to figure out)* and it ate up about 20 mins of my time. And get this - I was just missing **a single S**. Check this out, this is what I had:
   ```Ruby
   post login_path, params: { sessions: { email: "", password: "" } }
   ```
   and this is what I should of had:
   ```Ruby
   post login_path, params: { session: { email: "", password: "" } }
   ```
   Did you catch that? Yup - I had `sessions:` instead of `session:`. That was 20 minutes right there. Coding is fun sometimes 😐. But honestly, it was a good nights work.

--------

### Day 12: January 12th, 2017

**Today's Progress:** Continued Ch 8 of the [Hartl RoR Tutorial](https://www.railstutorial.org/book/basic_login) and just got a little done on getting the log in view setup.

**Time Logged:** .75 hour

**Thoughts:** Tried to get as much done at work as I could today with my evening being shot by the St. Paul Chamber of Commerce Ypro event. Will try to get additional time in tomorrow.  

--------

### Day 11: January 11th, 2017

**Today's Progress:** Continued Ch 8 of the [Hartl RoR Tutorial](https://www.railstutorial.org/book/basic_login) but went a little down a rabbit hole with all the command line stuff that was referenced in [Learn Enough Command Line to Be Dangerous](https://www.learnenough.com/command-line-tutorial#sec-grepping) and dove into `grep`.

**Time Logged:** 1.25 hour

**Thoughts:** As stated above - didn't complete as much on the actual rails tutorial but really got a better understanding of some command line tools such as `grep` and piping. This stuff was really fun and I created a second sheet to my [logged time google doc](https://docs.google.com/spreadsheets/d/1LGlyuXYwp8y4BxjdkXA4ZEqx3cXMPsKAAetAKwWtrAg/edit#gid=1630023459) that lists future docs in my "curriculum" and the [Learn Enough Command Line ...](https://www.learnenough.com/command-line-tutorial#sec-basics) just made the list! Reminds me of the time back in 2011(?) that I rented a Unix book from the library and started to really like it. Just think about how far I could be now if I would of stuck with it then!

--------

### Day 10: January 10th, 2017

**Today's Progress:** Back to the [Hartl RoR Tutorial](https://www.railstutorial.org/book/basic_login) and was able to finish Ch. 7 which focused on user sign up.

**Time Logged:** 1.25 hour

**Thoughts:** It was a pretty technical chapter but I was grasp a large chunk of it. I think at some point I should go back and review it all. Throughout most of the exercises I was able to get them figured out on the first try so - WOOHOO me 😉.

--------

### Day 9: January 9th, 2017

**Today's Progress:** Focused on the Ruby Basics tutorials on Treehouse.com.

**Time Logged:** 1 hour

**Thoughts:** It was nice to change it up today a little and get into more of the core Ruby. This is a core area that I need to focus on and once the Hartl RoR tutorial is done I think I'm going to split my time between personal projects and basic Ruby stuff.

--------

### Day 8: January 8th, 2017

**Today's Progress:** Continued Ch. 7 of the Rails tutorial, left off at section 7.4.4.

**Time Logged:** 1 hour

**Thoughts:** Finished getting a successful user signup workflow going in the rails app. Started to understand how you would use `flash[:success]` when confirming a successful signup.

--------

### Day 7: January 7th, 2017

**Today's Progress:** Continued Ch. 7 of the Rails tutorial at my parents.

**Time Logged:** 1 hour

**Thoughts:** Brought my laptop to my parents this weekend so I could continue my streak while on vacation. Wrote test today on user signup validation and error handling. The exercises are starting to get more vague but I've still been able to figure them out. It's giving me more confidence. 😎

--------

### Day 6: January 6th, 2017

**Today's Progress:** Continued Ch. 7 of the Rails tutorial at Code Club.

**Time Logged:** .75 hours

**Thoughts:** Was able to get in time at work during our Code Club meeting which will be really helpful on Friday's. Ch. 7 is starting to stretch my technical knowledge but I really like it as it's pushing me. I'm really starting to understand how some of the general aspects of a rails web applications works.

--------

### Day 5: January 5th, 2017

**Today's Progress:** Continued Ch. 7 of the Rails tutorial.

**Time Logged:** .75 hours

**Thoughts:** OOoooof. Today was particularly hard to find time. Spent a lot of the evening finishing a report for work. But, I still pushed through and got some time in. While today's time does come slightly under the 1 hr per day commitment I made - I'm still pretty proud that I pushed through and still did some work. 👊🏻

--------

### Day 4: January 4th, 2017

**Today's Progress:** Continued Ch. 7 of the Rails tutorial. Started getting into `params` on objects and it's starting to make sense how they are worked in HTTP requests.

**Time Logged:** 1 hour

**Thoughts:** Tough to get the time in today but still did it. So much to do - so little time. Glad I still kept the streak going. the idea of `:params` is starting to make sense as it was something that really escaped me before.

--------

### Day 3: January 3rd, 2017

**Today's Progress:** Continued Ch. 7 of the [Ruby on Rails tutorial](https://www.railstutorial.org/book/sign_up).

**Time Logged:** 2 hours

**Thoughts:** Knocked out getting the form gravatar and form completed. Proud that I was able to figure out one issue one my CSS where the gravatar wasn't displaying. It turns out that for some reason the Image tag was set to `Display: none;` which was odd.

Also frustrated that it took me about 10 minutes to figure out why my form wasn't showing up. Turns out that = signs are important and my form started off as:
`<% from_for(@user) do |f| %>`
...but should have been
`<%= form_for(@user) do |f| %>`
Oh how much of a difference an equal sign makes lol!

--------

### Day 2: January 2nd, 2017

**Today's Progress:** Fished Ch. 6 and started Ch. 7 of the Michael Hartl [Ruby on Rails tutorial](https://www.railstutorial.org/book/sign_up). Also, continued some of the Treehouse Ruby tutorials.

**Time Logged:** 2.5 hours

**Thoughts:** Struggled a bit during the day as I tried to get some of my work in with the kids at home but found a lot more free time during the evening.

**Link to work:** [Cloud9 link](https://ide.c9.io/garret_s/rails5-tutortial)

--------

### Day 1: January 1st, 2017

**Today's Progress**: Worked on Ch. 6 of the Michael Hartl [Ruby on Rails tutorial](https://www.railstutorial.org/book/modeling_users#code-validates_format_of_email) and started the Treehouse Ruby tutorial again.  

**Time Logged:** 2 hours

**Thoughts:** Feels good to commit to this. The RoR tutorial is coming along well and I think the Treehouse stuff will be great a filler for times when it's hard to get learning in. Also, this will help me get my personal Jeykll site finally up and running. 👍🏻

**Link to work:** [Cloud9 link](https://ide.c9.io/garret_s/rails5-tutortial)
