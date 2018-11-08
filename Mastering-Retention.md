[Back to Analytics Home](https://github.com/coolinmc6/analytics)

<a name="top"></a>

# Mastering Retention

## Resources Cited 

- [https://labs.openviewpartners.com/](https://labs.openviewpartners.com/)
- [https://amplitude.com/blog/2015/12/15/how-to-increase-growth-through-retention-analysis](https://amplitude.com/blog/2015/12/15/how-to-increase-growth-through-retention-analysis)
- [10 Steps To Get You Started with Behavioral Analytics](https://amplitude.com/blog/2016/06/14/10-steps-behavioral-analytics)
- [Avoiding the Wheel of Meaningless Growth](https://brianbalfour.com/essays/growth-principle-two-seek-authentic-growth)
	+ [Culture Of High Performance Growth Teams](https://brianbalfour.com/growth-culture)
		* this is the first in a series of essays on growth; **I MUST READ**
- [Diligence at Social Capital Part 1: Accounting for User Growth](https://medium.com/swlh/diligence-at-social-capital-part-1-accounting-for-user-growth-4a8a449fddfc)
- [You're Measuring Daily Active Users Wrong](https://amplitude.com/blog/2016/01/14/measuring-active-users)

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
- Determine your products usage interval - daily? weekly? monthly?
- If you don't have a good gauge of how often users should be using your product, you'll misinterpret your retention metric and misinform your strategies to improve it
- There is a Usage Interval Framework to better understand your usage interval
	+ **Key Point:** Identify the time interval at which *80%* of users have repeated the critical event
	+ pages 20 - 22 have a little worksheet to look at your analytics; take a look

[back to top](#top)

## Chapter 03: The Retention Lifecycle Framework

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

![User Retention Cycle]()

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

![Active Users over 12 Weeks]()


![Active Users broken down by type]()

- by breaking your users down into cohorts of new users, current users, resurrected users and dormant users, you can see what your "active user" count is really telling you.
- the "Pulse" ratio is (# of new users + # of resurrected users) / (# of dormant users)
	+ a ratio above 1 means that you are gaining more users than you are losing

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

![1% Rule Illustrated]()



[back to top](#top)

## Chapter 05: Current User Retention



[back to top](#top)

## Chapter 06: New User Retention



[back to top](#top)

## Chapter 07: Resurrected User Retention



[back to top](#top)

## Chapter 08: What to Do Next



[back to top](#top)

