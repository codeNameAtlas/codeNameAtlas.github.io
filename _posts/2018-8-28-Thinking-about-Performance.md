---
layout: post
title: Thinking About Performance
---

Modern day sites and apps are more robust and richer in functionality than ever before. This rise in usability has led to an increased challenge to deliver a high level of performance across a variety of network conditions and devices. Simply put, **Performance** refers to the speed in which pages are downloaded and displayed on a user's browser.


### Performance is about retaining users and improving conversions

Performance impacts key business metrics. [Research shows](https://headspin.io/resources/marketing/reports/5136-RR-performance-web-application.pdf) that a **1 second** slow down resulted in **11%** fewer page views and **7%** less conversion rate.

Currently, the average web page is greater than **3MB** and the average web application is getting larger.

While we collectively push the boundaries of what is capable on the web, we continue running into a common issue: **Performance**.

### Different Kinds of Performance

*This is part one of a four part series on Performance.* This post will address **why** performance matters and **how** to measure it. Subsequent posts will take a deep dive into three different performance considerations, complete with suggestions for addressing each.

1. **[Parsing, JavaScript, and Compilation Performance](http://alexnavarrete.com/Parsing-JS-Compilation-Performance/)**

2. **[Network Load Performance]()**

3. **[Rendering Performance]()**


### How to think about Performance

When starting to think about your applications performance it's important to think about the product you are working on and think about the unique needs of your site or app.

For example, the `New York Times` might care about time to first headline. `Twitter` might care about time to first tweet. `Google` might care about time to first result rendered or time to first ad displayed.

### How to measure impact and start improving Performance

There is not a silver bullet that will solve every performance issue out of the box, but the first step to improving performance is to **measure your current performance against performance metrics that are important to your application**. Ideally, you would also simulate this with less than perfect network conditions as well.

Google has released a helpful [Impact Calculator tool](https://www.thinkwithgoogle.com/feature/mobile/) to help teams visualize how small performance improvements could impact revenue.

![an image alt text]({{ site.baseurl }}/images/impact-calculator.png "impact calculator")

Ultimately, **improving performance will lead to a better user experience and an increase in business revenue**.

If you don't have an existing process in place to measure performance **RAIL** is a great resource to establish a performance framework for your team. [RAIL](https://developers.google.com/web/fundamentals/performance/rail) is a user-centric performance framework established by Google to measure performance.

Next, were going to take a deep dive into three different performance considerations, complete with suggestions for addressing each.

1. **[Parsing, JavaScript, and Compilation Performance](http://alexnavarrete.com/Parsing-JS-Compilation-Performance/)**

2. **[Network Load Performance]()**

3. **[Rendering Performance]()**

While a deep understanding of all of these may seem daunting, understand you don't need to do all of these things to improve the performance of your site. They are just suggestions or potential starting points, so don't feel overwhelmed!

**Congratulations!** You just finished part one of *Thinking about Performance*! [Parsing, JavaScript, and Compilation Performance](http://alexnavarrete.com/Parsing-JS-Compilation-Performance/) is the next part of this series.

Any questions about **Performance**? Feel free to reach out. I regularly work with customers and engineers to remove their technical hurdles 🙂
