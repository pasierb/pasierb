---
title: '“The job of a developer is not to write code. It is to solve problems”'
date: 2022-09-18T18:30:27+01:00
summary: "A short story of a startup killed by a well architected code."
showComments: true
---

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">The job of a developer is not to write code. It is to solve problems ⚡️</p>&mdash; Marc Backes (@themarcba) <a href="https://twitter.com/themarcba/status/1571142654565416962?ref_src=twsrc%5Etfw">September 17, 2022</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

I should probably have this quote automatically added to the README of every new project I start.

I had this realization of fetishizing code after I got bored working on a startup and handed it over to some other folks. Functionality wise the idea was super simple – index of spots to surf. Too simple to be fun…

![](https://stuffs.dev/wp-content/uploads/2022/09/kg-infrastructure.jpeg)

I managed to squeeze in this project the amount of fancy 3-letter acronyms and technilogies that would last a full night of bragging to fellow engineers.

*   Monorepo
*   Serverless API on AWS Lambda
*   Serverless database
*   fully automated CI/CD pipelines
*   Next.js with SSG (static site generation)
*   RxJS
*   Infrastructure as a code with AWS CDK
*   Admin panel on AWS Fargate that scales to 0 when no traffic
*   Everything behind AWS Cloudfront for caching
*   …and probably couple more things I already forgot

The whole application should be a simple monolith ([Ruby on Rails](https://rubyonrails.org/) would be a great fit) and a database (for the amount of traffic and size of data even [SQLite would do](https://www.sqlite.org/whentouse.html)).

This architecture does make sense if you have people, traffic and business that already generates money – I saw this pattern deployed successfully many times during my time in AWS.

Technology is facinating and sometimes, we, developers are so eager to try it out that we miss the problem at hand and consequently create new problems – full circle.
