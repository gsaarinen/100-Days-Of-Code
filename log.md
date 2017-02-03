# 100 Days Of Code - Log

### Day 33: February 2st, 2017

**Today's Progress:**

   Groundhog's Day! I am still debugging 👏 these 👏 test 👏 issues 👏! Yup - Ch 10. Still.

**Time Logged:**

   1.5

**Thoughts:**

   So now I have 2 separate 'but related' test issues in the `user_edit_test.rb` file - `unsuccessful_edits` and `successful edit with friendly forwarding`. It all seems to be related to the `log_in_as` helper and it's doing a weird redirect. I keep getting these types of errors:

   ```FAIL["test_unsuccessful_edit", UsersEditTest, 619.0571372920022]
 test_unsuccessful_edit#UsersEditTest (619.06s)
        expecting <"users/edit"> but rendering with <[]>
        test/integration/users_edit_test.rb:13:in `block in <class:UsersEditTest>
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
   NameError: undefined local variable or method `surname' for #<User:0x29cbfb0 @name="Bob">
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
