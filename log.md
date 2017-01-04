# 100 Days Of Code - Log

### Day 1: January 1st, 2017

**Today's Progress**: Worked on Ch. 6 of the Michael Hartl [Ruby on Rails tutorial](https://www.railstutorial.org/book/modeling_users#code-validates_format_of_email) and started the Treehouse Ruby tutorial again.  

**Time Logged:** 2 hours

**Thoughts:** Feels good to commit to this. The RoR tutorial is coming along well and I think the Treehouse stuff will be great a filler for times when it's hard to get learning in. Also, this will help me get my personal Jeykll site finally up and running. 👍🏻

**Link to work:** [Cloud9 link](https://ide.c9.io/garret_s/rails5-tutortial)

### Day 2: January 2nd, 2017

**Today's Progress:** Fished Ch. 6 and started Ch. 7 of the Michael Hartl [Ruby on Rails tutorial](https://www.railstutorial.org/book/sign_up). Also, continued some of the Treehouse Ruby tutorials.

**Time Logged:** 2.5 hours

**Thoughts:** Struggled a bit during the day as I tried to get some of my work in with the kids at home but found a lot more free time during the evening.

**Link to work:** [Cloud9 link](https://ide.c9.io/garret_s/rails5-tutortial)

### Day 3: January 3rd, 2017

**Today's Progress:** Continued Ch. 7 of the [Ruby on Rails tutorial](https://www.railstutorial.org/book/sign_up).

**Time Logged:** 2 hours

**Thoughts:** Knocked out getting the form gravatar and form completed. Proud that I was able to figure out one issue one my CSS where the gravatar wasn't displaying. It turns out that for some reason the Image tag was set to `Display: none;` which was odd.

Also frustrated that it took me about 10 minutes to figure out why my form wasn't showing up. Turns out that = signs are important and my form started off as:
`<% from_for(@user) do |f| %>`
...but should have been
`<%= form_for(@user) do |f| %>`
Oh how much of a difference an equal sign makes lol!
