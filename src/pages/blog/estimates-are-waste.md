---
templateKey: blog-post
title: Estimates Are Waste
path: blog-post
date: 2020-09-16T09:30:00.000Z
description: Estimates are waste, in that time spent estimating is often time that could have been spent producing something with business value. The first of the 5 laws of software estimates, this one is easy to demonstrate in the context of software developers. However, like so many things in software, it doesn't always hold when that context shifts.
featuredpost: false
featuredimage: /img/estimates-are-waste.png
tags:
  - agile
  - estimates
  - estimation
  - lean
  - noestimates
  - waste
category:
  - Software Development
comments: true
share: true
---

This is the first of the [5 Laws of Software Estimates](/the-5-laws-of-software-estimates/).

It's all about context. In the context of software development, of delivering business value in the form of working software, estimates provide no value. In the context of choosing what software to build, there may certainly be value in estimates, but even there it's an ROI calculation, with the hope being that the estimates will provide more value than they cost.

If you're a programmer, working 40 hours per week, and delivering working software as quickly as you can in that time, you produce a certain amount of value for your employer or client. Let's say you have a backlog of bugs and features to work on, and these are roughly prioritized based on how urgent they are to fix. This backlog of work is going to have some average amount of time to complete. It might be 2 hours. It might be 2 days. In any case, you're able to get a certain amount of work done per week by focusing on fixing bugs and adding new features.

Now imagine a new policy is put in place. All bugs and features need to be estimated by the team before they're triaged and added to the backlog. These can't just be simple guesses - these need to be estimates that can be relied upon. Investigating each individual backlog item in order to estimate it (in addition to time spent meeting and documenting the estimates) will require a minimum of half an hour and sometimes more. Now let's imagine that previously the average time to complete a work item was 2 hours, so in a 40 hour week (of which let's say 30 are available for programming work outside of meetings, emails, communicating, etc.) you were able to complete 15 of these work items. Now, each of these work items is going to require an additional half an hour (or more) of time spent estimating. Also, since that time isn't being spent right when you're working on the problem at hand, you can't argue that that time is helping you understand the problem as you get ready to work on it. The estimating might have happened weeks earlier, and might have been done mainly by one of your teammates. Now instead of getting 15 work items done per week, you're down to 12 - a 20% reduction in your productivity.

This isn't just a thought experiment. In 2005, David Anderson was working at Microsoft, where he was put in charge of a team that was responsible for maintaining over 80 applications used internally by Microsoft employees. The team worked mainly on relatively small changes requests involving less than 120 hours of development work. The team was considered the worst performing in its business unit based on the fact that its work backlog exceeded its capacity 5 times and its typical lead time for a change request was 5 months. The team's customers were unhappy.

Anderson analyzed the situation and applied steps from [Theory of Constraints](https://en.wikipedia.org/wiki/Theory_of_constraints) and Kanban. He published a book about his experience, [Kanban](http://amzn.to/1P7qpI0), which is also a large influence on my [Kanban Fundamentals](https://www.pluralsight.com/courses/kanban-fundamentals) course on Pluralsight. In the book (as well as this [white paper](http://images.itrevolution.com/images/kanbans/From_Worst_to_Best_in_9_Months_Final_1_3-aw.pdf)) Anderson describes how, with no added resources, the team increased productivity by 155% in 9 months. Lead time dropped to a maximum of 5 weeks, with 14 days being typical. The excess backlog was worked off and customers became delighted. How was this accomplished?

One of the key problems with the status quo that Anderson inherited was that new change requests, which arrived about once a day, had to have a "rough order of magnitude" (ROM) estimate. The turnaround time on these estimates was part of the group's Service Level Agreement (SLA) with their internal customers. The SLA stated that all ROMs would be completed within 48 hours. To deliver on this agreement, when new change requests arrived, a developer and a tester would each need to interrupt their work, check out the source code for the change request (which would likely belong to a different repository than where they were working), read the request, analyze the code to determine what changes it would require, and document their findings in the system. This would typically take about 4 hours for each of the two individuals. Anderson calculated that responding to ROM requests was using about 1 day of work effort per request.

One reason these ROMs were used was to determine whether the maintenance team would take on the work, or if it should be given to the product team. Change requests in excess of a certain threshold of effort would not be given to the maintenance team, but would be kicked back to the product team for their consideration. Given this as well as other reasons, only about 50% of requests that were estimated were ever actually completed by the team. A huge amount of time was being spent by the team estimating work they would never do.

Anderson implemented a number of changes, but one of the biggest was the elimination of ROMs from the team's SLA. Instead, all change requests were considered equal based on the average production rate of the team. Additionally, time spent prioritizing the backlog of change requests was all but eliminated by instead having the managers responsible choose the next item to work on from the backlog only when one was completed. This dramatically reduced the amount of time required by these managers to meet and agree on a precise sequence and importance of every backlog item (based, at least in part, on ROMs that were no longer being done).

Estimates are always a cost, and often a complete waste. In Anderson's book and case study, he demonstrates clearly how overuse of estimates was killing the productivity of an otherwise capable team. In many situations and organizations, the average size of change requests is sufficient to prioritize the work, and the increase in developer productivity exceeds the marginal gains that might be had from getting this or that change request done before or after another one.

Learn more about the [5 Laws of Software Estimates](/the-5-laws-of-software-estimates/), and share your own experience in the comments below.
