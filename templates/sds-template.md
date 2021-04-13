---
description: Template for Software Design Documents
---

# SDS Template

_This page is an evolving template and should be adjusted from time to time as we learn more about what structure works for us._

_This template is based heavily on_ [_https://www.freecodecamp.org/news/how-to-write-a-good-software-design-document-66fcf019569c/_](https://www.freecodecamp.org/news/how-to-write-a-good-software-design-document-66fcf019569c/)_._

**Title and People**

The title of your design doc, the author\(s\) \(should be the same as the list of people planning to work on this project\), the reviewer\(s\) of the doc, and the date this document was last updated.

**Overview**

A high level summary that every engineer at the company should understand and use to decide if it’s useful for them to read the rest of the doc. It should be 3 paragraphs max.

**Context**

A description of the problem at hand, why this project is necessary, what people need to know to assess this project, and how it fits into the technical strategy, product strategy, or the team’s quarterly goals.

**Goals and Non-Goals**

The Goals section should:

* describe the user-driven impact of your project — where your user might be another engineering team or even another technical system
* specify how to measure success using metrics — bonus points if you can link to a dashboard that tracks those metrics

Non-Goals are equally important to describe which problems you **won’t** be fixing so everyone is on the same page.

**Milestones**

A list of measurable checkpoints, so people can skim it and know roughly when different parts of the project will be done. You should break the project down into major user-facing milestones if the project is more than 1 month long.

Use calendar dates instead of time-from-now so you take into account unrelated delays, vacations, meetings, and so on. It should look something like this:

| Date | Milestone | Deliverable |
| :--- | :--- | :--- |
| June 7, 2018 | Start |  |
| June 28, 2018 | Milestone 1 | New system MVP running in dark mode |
| July 4, 2018 | Milestone 2 | Retire old system |
| July 14, 2018 | End | Add feature X, Y, Z to new system |

_Add an "Update" subsection here if the ETA of some of these milestone changes, so the stakeholders can easily see the most up-to-date estimates._

**Existing Solution**

In addition to describing the current implementation, you should also walk through a high level example flow to illustrate how users interact with this system and/or how data flow through it.

A **user** **story** is a great way to frame this. Keep in mind that your system might have different types of users with different use cases.

**Proposed Solution**

AKA **Technical Architecture** section. Again, try to walk through a user story to concretize this. Feel free to include many sub-sections and diagrams.

Provide a big picture first, then fill in _lots_ of details. Aim for a world where you can write this, then take a vacation on some deserted island, and another engineer on the team can just read it and implement the solution as you described.

**Alternative Solutions**

What else did you consider when coming up with the solution above? What are the pros and cons of the alternatives? Have you considered buying a 3rd-party solution — or using an open source one — that solves this problem as opposed to building your own?

**Testability, Monitoring and Alerting**

People often treat this as an afterthought or skip it all together, and it almost always comes back to bite them later when things break and they have no idea how or why. How are you going to test this work? Will you use an automated monitoring system? What level of test coverage are you aiming for?

**Cross-Team Impact**

How will this increase on call and dev-ops burden?  
How much money will it cost?  
Does it cause any latency regression to the system?  
Does it expose any security vulnerabilities?  
What are some negative consequences and side effects?  
How might the support team communicate this to the customers?

**Open Questions**

Any open issues that you aren’t sure about, contentious decisions that you’d like readers to weigh in on, suggested future work, and so on.

**Detailed Scoping and Timeline**

This is the breakdown of how and when you plan on executing each part of the project. There’s a lot that goes into scoping accurately, so you can read [this post](https://medium.freecodecamp.org/how-to-effectively-scope-your-software-projects-from-planning-to-execution-e96cbcac54b9) to learn more about scoping.

