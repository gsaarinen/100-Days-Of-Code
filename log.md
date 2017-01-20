# 100 Days Of Code - Log

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
