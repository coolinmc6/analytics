[Back to Analytics Home](https://github.com/coolinmc6/analytics)

<a name="top"></a>

# Mastering Retention

## Resources Cited 

- [WHY RETENTION IS KING OF GROWTH STRATEGY](http://labs.openviewpartners.com/retention-optimization-is-king-of-growth-strategy/#.V6ltC5MrL4M)
- [OpenView Partners](https://labs.openviewpartners.com/)
- [How to Increase Growth Through Retention Analysis](https://amplitude.com/blog/2015/12/15/how-to-increase-growth-through-retention-analysis)
- [10 Steps To Get You Started with Behavioral Analytics](https://amplitude.com/blog/2016/06/14/10-steps-behavioral-analytics)
- [Avoiding the Wheel of Meaningless Growth](https://brianbalfour.com/essays/growth-principle-two-seek-authentic-growth)
	+ [Culture Of High Performance Growth Teams](https://brianbalfour.com/growth-culture)
		* this is the first in a series of essays on growth; **I MUST READ**
- [Diligence at Social Capital Part 1: Accounting for User Growth](https://medium.com/swlh/diligence-at-social-capital-part-1-accounting-for-user-growth-4a8a449fddfc)
- [You're Measuring Daily Active Users Wrong](https://amplitude.com/blog/2016/01/14/measuring-active-users)
- [Hooking Users In 3 Steps: An Intro to Habit Testing](https://www.nirandfar.com/2012/04/hooking-users-in-3-steps.html)
- [Why You Need Cohorts to Improve Your Retention](https://amplitude.com/blog/2015/11/24/cohorts-to-improve-your-retention)
- [This Is How You Find Your App's Aha! Moment](https://apptimize.com/blog/2016/02/this-is-how-you-find-your-apps-aha-moment/)
- [The Billion Dollar Mind Trick: An Intro to Triggers](https://www.nirandfar.com/2012/04/billion-dollar-mind-trick.html)
- [The Psychology of Notifications: How to Send Triggers that Work](https://www.nirandfar.com/2015/03/notifications-that-work.html)
- [How to Bring Inactive Users Back from the Dead](https://www.appcues.com/blog/how-to-bring-inactive-users-back-from-the-dead)
- [Empty States](http://emptystat.es/)

## Table of Contents

- [Chapter 01: Why You Need to Care About User Retention](#chapter-01-why-you-need-to-care-about-user-retention)
- [Chapter 02: Your Critical Event & Product Usage Interval](https://github.com/coolinmc6/analytics/blob/master/Mastering-Retention.md#chapter-02-your-critical-event--product-usage-interval)
- [Chapter 03: The Retention Lifecycle Framework](https://github.com/coolinmc6/analytics/blob/master/Mastering-Retention.md#chapter-03-the-retention-lifecycle-framework)
- [Chapter 04: Product Analysis Toolkit](https://github.com/coolinmc6/analytics/blob/master/Mastering-Retention.md#chapter-04-product-analysis-toolkit)
- [Chapter 05: Current User Retention](https://github.com/coolinmc6/analytics/blob/master/Mastering-Retention.md#chapter-05-current-user-retention)
- [Chapter 06: New User Retention](https://github.com/coolinmc6/analytics/blob/master/Mastering-Retention.md#chapter-06-new-user-retention)
- [Chapter 07: Resurrected User Retention](https://github.com/coolinmc6/analytics/blob/master/Mastering-Retention.md#chapter-07-resurrected-user-retention)
- [Chapter 08: What to Do Next](https://github.com/coolinmc6/analytics/blob/master/Mastering-Retention.md#chapter-08-what-to-do-next)

## CM Notes

- Chapter 1 explains user retention is so important. Without a user retention curve that eventually flattens out, you don't have product-market fit. Without product-market fit, you don't really have a business. Without product-market fit, new users won't really help you because you can't retain them.
- Chapter 2 explains what a critical event is and why you need to identify it. It also explains what the product usage interval is. These two figures help identify the appropriate time frame by which you can measure retention.
- Chapter 3 explains the User Retention Framework and how you can think about users. There are generally four types of users: new users, current users, dormant users, and resurrected users (these are the lifecycle cohorts). This chapter also explains the three main user retention metrics (Nth-Day Retention, Unbounded Retention, and Bracket Retention).
- Chapter 4 explains what behavioral personas are and how you can use them to understand your users. Diving into the lifecycle information of your behavioral personas can be done in a number of ways and they list a number of analyses you should perform to understand your users better.
- Chapter 5 stresses the importance of keeping current users and making your product habit-forming. This product

## Chapter 01: Why You Need to Care About User Retention

- acquiring users isn't the whole answer - keeping them is key!
- if you don't demonstrate value to your customers early and often, using your product won't become a habit and they won't return
- CM - how often should someone be using your product? How do we ramp them up in the product and get them using it?
- **Retention** is a measure of how many users return to your product over time.

> The point is, every improvement that you make to retention also improves all of these other things — virality, LTV, payback period. It is literally the foundation to all of growth, and that’s really why retention is the king.

- your goal should be increase user retention is minimize churn
- A key metric is **N-Day Retention** where Day 0 is the day they first use the product and then you see whether that user has returned on Day 1, Day 5, etc. It creates a retention curve as shown below:

![Retention Curve](https://github.com/coolinmc6/analytics/blob/master/assets/retention-curve.png)

- If Day 7 is retention is 13%, it means that out of all the users who first used the product on Day 0, 13% came back and were active on Day 7
- Retention matters **IMMEDIATELY**, not later once you're past a certain "growth" period...if you don't retain users, you don't have product-market fit. See below

![Retention Curve Showing Product-Market Fit](https://github.com/coolinmc6/analytics/blob/master/assets/rc-product-market-fit.png)

- You need to build a product that people will get hooked on; you need a *habit-forming* product
- You need to understand what value your users get out of your product - figure out what your power users are doing a nudge your user base to behave more like them
- Diagnosing and improving retention is an iterative, ongoing process
- There are couple ways to improve retention:
	+ #1 - Shift the Retention Curve up
		* move Day 1 retention from 30% to 40%, Day 20 from 20% to 25%, etc.
	+ #2 - Flatten your Retention Curve
		* instead of it gradually sloping down with each passing day, have it flatten out which means upping your further out N-Day retention.
- Amplitude has its own Retention Framework which I'll be examining later

[back to top](#top)

## Chapter 02: Your Critical Event & Product Usage Interval

- Amplitude recommends doing a few things before really digging into this chapter:
	+ make sure analytics is properly tracking the user actions important to you
	+ perform an instrumentation review
		* CM - this looks pretty valuable and would be a good way to get everyone on the team on the same page
	+ have a high-level understanding of users BEFORE you put the retention lifecycle framework in place
- A **critical event** is an action that users take within your product that aligns closely with your core value proposition.
	+ This is what you want your users to do! Think about it - what is the one thing you want your users to do
	+ in Airbnb's case it is book a room
- A good rule of thumb is one critical event per product offering
- in a marketplace, where you have two main types of users (i.e. buyers and sellers), you may have two critical events, one for each
- Determine your product's usage interval - daily? weekly? monthly?
- If you don't have a good gauge of how often users should be using your product, you'll misinterpret your retention metric and misinform your strategies to improve it
- There is a Usage Interval Framework to better understand your usage interval <a name="usage-interval"></a>
	+ **Key Point:** Identify the time interval at which *80%* of users have repeated the critical event
	+ pages 20 - 22 have a little worksheet to look at your analytics; take a look

[back to top](#top)

## Chapter 03: The Retention Lifecycle Framework

### 3 Ways to Measure User Retention

- There are three main types of retention:
	+ N-Day Retention
	+ Unbounded Retention
	+ Bracket Retention
- N-Day Retention is **most popular**; usually, when people talk about retention, they refer to N-Day Retention
	+ this measure is best for gaming or social apps or any other type of product where you're trying to get users to exhibit regular, repeat behavior
- The day a user is **first active** in your app/service is Day 0. You have to define what that means; that could be:
	+ day of first download
	+ day of registration
	+ day they performed an action in your app
	+ day they played their first song
	+ day they added a friend
	+ etc.
- N-Day Retention explained...
	+ Day 1 retention looks at how many users returned **specifically one day** after they were active
	+ Day 3 retention looks how many users returned **on exactly** the third day after they were first active; it does **NOT** matter if they came back on Day 2
	+ Day 7 retention looks at users who returned **exactly** on the seventh day after they were first active
		* Broken down further, a user is only counted if it was active **ON** Day 7; it doesn't matter at all how many times they were active on days 1 - 7; if they aren't active on Day 7, they are not considered Day 7 retained
	+ Question: given that as a measure, wouldn't retention curves be lumpier or do these example retention curves represent a general trend for apps with many users? *CM: I could see certain days, for whatever reason, having a higher retention than earlier days. Even if it's a fluke, is it really THAT unlikely that a day 6 retention could, in some cases, be higher than day 5? Is it ALWAYS the case that day N retention is higher than day N+1 retention?*
- N-Week Retention and N-Month Retention are the same idea but the time period is lengthened; so Week 1 Retention is all users active within that week.
- **Unbounded Retention** shows you the proportion of users who came back on a specific day or anytime after that day.
	+ this is for business that don't expect users to engage with their product or service on any regular cadence
- The inverse of unbounded retention, naturally, is the percent of users that used your app and then never returned again; also known as your **churn rate**
- **Bracket Retention** lets you split your retention analysis into customer periods of instead of limiting yourself to a daily, weekly, or monthly timeframe.
	+ For example: 
		* Bracket 1: Day 0
		* Bracket 2: Days 1 - 3
		* Bracket 3: Days 4 - 6
		* Bracket 4: Days 7 - 11
- If the user is retained in that bucket at all, it is counted

> The right retention metric should show you where you can improve and give you an accurate view of the health of your business.

### The Retention Lifecycle Framework 

![User Retention Cycle](https://github.com/coolinmc6/analytics/blob/master/assets/user-retention-cycle.png)

- New User Retention
	+ your new user experience is your product's first impression
	+ Figure out which behaviors or features bring new users back
- Current User Retention
	+ Don't take current users for granted; each one has the opportunity to turn into a highly-engaged power user
	+ You need to understand and improve the experience for your currently active users
	+ Figure out what certain groups of users are (and aren't) doing
- Resurrected Users are users that have used your product and then left
	+ it's cheaper to resurrect a dormant user than it is to acquire one
	+ Analyze why users are coming back
		* did they respond to a particular winback campaign?
		* a push notification?
		* And did they become current users or drop off again?
- The next two graphs illustrate the danger of only measuring current active users:

### Creating Your Lifecycle Cohorts

- **CM:** This specific section is referenced several times in the following chapters, with each one dealing with a different type of user: Chapter 5 (Current Users), Chapter 6 (New Users), and Chapter 7 (Resurrected Users). Each of those chapters require this section of breaking your users down into these main four groups
- The main crux behind lifecycle cohorts is that a growing "active" user base does not alone suggest that you're doing well. Look at these two graphs:

![Active Users over 12 Weeks](https://github.com/coolinmc6/analytics/blob/master/assets/active-users-bar-chart.png)

![Active Users broken down by type](https://github.com/coolinmc6/analytics/blob/master/assets/active-users-breakdown.png)

- by breaking your users down into cohorts of new users, current users, resurrected users and dormant users, you can see what your "active user" count is really telling you.
- the "Pulse" ratio is (# of new users + # of resurrected users) / (# of dormant users)
	+ a ratio above 1 means that you are gaining more users than you are losing
- As a reminder, determining where a particular user falls depends on your [usage interval](#usage-interval) (the interval at which 80% of current users repeate the critical event)

> Reminder: Be careful about over- optimizing for just your power users. Understanding power usage
is important, but you can't convert everyone into a power user overnight. As you iterate on your product, make sure to optimize for retaining the most number of users, not just the best users

- pages 38 - 39 have a good little worksheet on determining your retention lifecycle split

[back to top](#top)

## Chapter 04: Product Analysis Toolkit

- Users will use your product in various different ways. Breaking your users down in *behavioral personas* will help you understand them better
- A **behavioral persona** represents a specific way of using the product
- An example of this is YouTube:
	+ Creators - people who create videos (small percentage)
	+ Viewers - people watch those videos (the large majority)
	+ Viewers & Commenters - people who watch and comment (creators < view & comment < view only)
- The **1% Rule** or **1/9/90 Rule** that says:
	+ 1% Create
	+ 9% Interact
	+ 90% Consume
- If you optimize only for your power users (in YouTube's case you might think it's the creators), you'd be neglecting the other 99% that largely watch those videos

![1% Rule Illustrated](https://github.com/coolinmc6/analytics/blob/master/assets/1-percent-rule.png)

- You can break your users down into Power, Core and Passive users:
	- **Power Users**: People who use your product with a very high frequency or use a “power” feature that
the majority of users don't take advantage of.
	- **Core Users**: People who are using your app at a regular frequency and in the “expected” way.
	- **Passive Users**: These are people who might not be using your app in the core way that you designed, but are still coming back at a regular frequency to do something.
- Use both qualitative and quantitative methods to determine the personas that use your product
- After breaking your users into your lifecycle cohorts (new, current, and resurrected users) and you have your personas, you need to measure the baseline retention for each cohort and dig deeper into the drivers of retention
- Analyses to Do:
	+ Compare the retention curves of behavioral personas
	+ Investigate user properties (country, age, language, or any other characteristic about these users) to understand who these users are
	+ Segment your retention curves by user properties
	+ Use behavioral cohort analysis to measure the impact of different user actions
		* Based on the actions of your users, study their retention and see which groups of users do what
		* Famous example from Facebook: Users who added at least 7 friends within their first 10 days were more likely to be retained long term. **That is a behavioral cohort: there's a behavior (adding at least 7 friends) and a time period (within 10 days of signing up).**
	+ Conversion rate through your critical path funnel
		* A critical path funnel is the series of actions you anticipate users taking in order to complete your critical event
	+ Find your most common user flows
	+ Measure stickiness
		* **stickiness** refers to the frequency at which people are using your product. Specifically, stickiness measures the number of days out of a given time period that a user was active, or did a specific event (like your critical event).
		* Weekly stickiness - the percentages of users who active or performed a specific event at least *n* days out of a week
		* Monthly stickiness - The percentage of users who were active or performed a specific event at least *n* days out of a month
	+ Session metrics
		* the time spent isn't always a great metric - make sure it makes sense for your app / website
- The reference below is great and I should return to it:

![Product Analysis Toolkit - page 1](https://github.com/coolinmc6/analytics/blob/master/assets/product-analysis-toolkit-1.png)

![Product Analysis Toolkit - page 2](https://github.com/coolinmc6/analytics/blob/master/assets/product-analysis-toolkit-2.png)

- CM - start pg 64

[back to top](#top)

## Chapter 05: Current User Retention

- Improving your current user retention is critical to sustaining a business. If your retention curve doesn't flatten out at some point, it will become impossible to sustain true growth.
- Nir Eyal's 5% Rule and Habit Testing
- These are the steps to Habit Testing:
	+ Identify - find habitual usesr
	+ Codify - understand what these users have in common
	+ Modify - adapt user flow based on these learnings
- The 5% Rule means that if at least 5% of your users aren't coming back to your site, or it isn't habitual, you need to rethink your value proposition
	+ This suggests that you may not have product-market fit
- These are the goals of current user retention analysis:
	+ Get new userst o form habits and become current users
	+ Get current users to become core users, and core users to become power users
- Remember the User Cohort Diagram:

![User Cohort Diagram](https://github.com/coolinmc6/analytics/blob/master/assets/user-retention-cycle.png)

- These are the phases before becoming a current user:
	+ Onboarding
	+ Value Discovery
	+ Habit Formation

![Phases of becoming a current user](https://github.com/coolinmc6/analytics/blob/master/assets/phases-current-user.png)

- I. Current Users Diagnostic
	+ look at baseline retention for the current user cohort
	+ investigate user properties & segment retention curve
- II. Find behavioral personas of current users
- III. Discover the drivers of Habit Formation
- IV. Discover drives from Passive to Core to Power Personas
- This pretty much sums up this chapter: **Studying current user retention is about understanding the factors that encourage people to form a habit.**
- The "A-ha Moment" is when people see the value in the product
- To identify the drivers of habit formation, you need to find the action or set of actions that separates users who form a habit and from those who don't
- Here are some metrics they recommend tracking:
	+ The size (in absolute numbers) and percent- age of your total active users that is made up of your current users (as calculated via lifecycle or manual analysis).
	+ Retention over time of all current users and of each behavioral persona.
	+ Size and percentage breakdown of your important behavioral personas. Are you getting more people into important personas?
	+ Stickiness over time for critical events. This will show you any changes in how active current users are in the product.
	+ Conversion rate over time through your critical path funnel


[back to top](#top)

## Chapter 06: New User Retention

- New user retention is incredibly important and is often the most closely analyzed type of retention
- Understand your onboarding funnel
- Looking at the paths of dropped off users

![Habit Formation Timeframe](https://github.com/coolinmc6/analytics/blob/master/assets/habit-formation-time-frame.png)

- I. New users diagnostic
	+ look at baseline retention for new users cohort
	+ investigate user properties & segment retention curve
- II. Find behavioral personas of your new users
- III. Understand your onboarding funnel
	+ First impressions matter
		+ bad onboarding leads to a bad new user retention
	+ Define your onboarding funnel
		* if there is a well-defined sequence that users move through, then simply tracking those events is easy
	+ If you have an open-ended first-user experience, what are the key events that a user must do to start getting value out of your product
	+ Measure the retention impact of your on-boarding flow
		* start with the largest drop-off in your funnel
- IV. The phases of new user retention: Onboarding and Value Discovery
	+ these are the phases of a new user:
	
![Habit Formation Timeframe](https://github.com/coolinmc6/analytics/blob/master/assets/phases-new-user.png)

- V. Identify the drivers of successful onboarding
- VI. Identify the drivers of successful value discovery

- **There is more here that I need to revisit. There are just certain items that I can't wrap my head around yet.**

[back to top](#top)

## Chapter 07: Resurrected User Retention

- A **resurrected user** is someone who has returned to your product after being inactive, or dormant, for a period of time
- Don't let users come back to a poor empty experience

![Habit Formation Timeframe](https://github.com/coolinmc6/analytics/blob/master/assets/empty-state.png) 

- I. Resurrected users diagnostic
	+ compare resurrected users to other users (current and new)
	+ determine opportunity size of resurrected users
	+ determine percentage of active users that are resurrected
	+ how many potential resurrected users do you have?

- II. Find behavioral personas of resurrected users
- III. Identify triggers of resurrection
	+ Internal vs External Triggers
		* external = push notifications, emails or ads to get users' attention
		* internal = in a person's mind; occurs when a product is tightly coupled with a thought, an emotion, or a pre-existing habit
		* the best habit-forming products start out with external triggers to initially attract and educate uses and then over time, users don't need the external triggers, only the internal ones
	+ for resurrected users, which external triggers work?
		* use session utm parameters to look for common sources
			- [Intro to UTM Parameters and Best Practices](http://blog.rafflecopter.com/2014/04/utm-parameters-best-practices/)

[back to top](#top)

## Chapter 08: What to Do Next

- Good review of the book - if I had to re-read this, I'd start with the first few pages just to see the material initially.
- They recommend using OKRs - Objectives and Key Results. Interesting methodology around retention:
	+ State your goals
	+ Set a timeframe (30 to 90 days)
	+ Assign three key resutls you want to achieve related to retention:
		* #1 - 90% chance of success
		* #2 - 50% chance of success
		* #3 - 10% chance of success
	+ Brainstorm the actionable objectives you'll use to hit your key results

## Instrumentation Review

- One of the first steps is "Organize your event taxonomy" which means takes the time to understand the business that we're in and the success criteria for your business (and in particular, your website or app).
- Here are some questions to ask:
	+ Are the events you're tracking aligned with your analytics goals?
	+ Can everyone understand what each event is and why it's being tracked?
	+ Are you tracking events aligned with your critical path funnel?
	+ How are you defining an active user?
- They next recommend "Validating your data" by going through your onboarding process and the critical paths as you've identified them
- **Habit Formation phase**: This follows the Onboarding and Value Discovery phases of new user retention. Once a user has discovered value in your product, you need to make sure they develop a habit so that they keep coming back over time. Users who successfully pass through the Habit Formation phase become current users of your product.

[back to top](#top)



















