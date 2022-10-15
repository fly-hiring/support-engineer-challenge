# Support Engineer Hiring Project

Hello! This is a hiring project for our Support Engineer role.  If you apply, we'll ask you to do this project so we can see how you work through type of work you'd do at Fly.io.

## Hiring Project: Technical Challenge

Our customers are developers. They usually need support when things are going wrong. In many ways, they're looking less for answers and more for empathy and understanding. Don't get us wrong, they want answers too. But they're happiest when they talk to people who understands what they're going through.

The first part of the hiring process is a technical challenge. We want you to do two things with the starter Rails project in this repository:

1. Make it send an email when the button is clicked. 
2. Deploy it to Fly.io

The project is mostly ready to go, it's just missing some functionality. All you need to do is handle the button click, write the code to send an email, and then deploy it.

You do not need to do any special setup to send emails. The project is configured to show a preview in a new tab when an email send is triggered.

If you've never done Rails before, that's ok! Our customers will use languages you have never experienced before, too. There's plenty of time to figure it out.

## Hiring Project: Customer Interaction

We interact with customers in two ways: over email, and in our public discussion forums. We want you to write a sample response for each.

### Support Email Response

Paid customers use email for support. When a paid customer writes in, we want to do two things:

1. Get them a helpful response very quickly
2. Investigate their issue

A paid customer reports that they made a small change to their app and now it is failing to deploy. When they attempt to deploy, they get the following message: 

```text
v83 is being deployed 
c2258102: yyz pending 
c2258102: yyz pending 
c2258102: yyz running unhealthy [health checks: 1 total] 
c2258102: yyz pending 
c2258102: yyz pending 
c2258102: yyz pending 
c2258102: yyz pending v83 failed - Failed due to unhealthy allocations - not rolling back to stable job version 83 as current job has same specification
```

Write an initial response to the customer. This might be a problem they can solve, so it would be good to give them some pointers. It's ok to ask them questions about their app, too.

Then, write some notes about how you'd investigate their issue in parallel. If we can figure out what's wrong with a paid customer app, they'll be happy when we tell 'em. If we discover it's an issue on our end, they'll be happy when we fix it. Win win.

Investigating a customer issue can get complicated. Here are some tools you can use to investigate customer issues:

* Google + Community forums.
* The same tools customers have, you're probably just better at using them
* On call Fly.io product engineers. 
* On call Fly.io operations engineers

### Community Forum Response

A community member posted this question:

> I deployed my app to two regions and I keep getting 503 status code errors when I try to visit my app. This app works fine when I run it locally so there must be something wrong with fly.

There are no known outages (if there were, we'd post them on status.flyio.net). Please write a forum response for this user. Keep in mind that forum responses will be public in real life! You're writing for everyone who will ever read this post.

We have some rough internal guidelines we use for forum posts. Here they are:

Community support should mainly be for community members to help each other out. 
Our job in community is to:

* give users the tools they need to troubleshoot/resolve their own issues
* point users in the right direction by linking docs or other community posts
* "train" users to be better community members

We should not be promising things to users, don't tell them you will look into an issue unless you have already determined it to be on our end and we are working on it, don't tell them something might be a feature later on, get used to saying "no."

You also do not need to spend an inordinate amount of time trying to solve a user's issue, take your time to decide if this is an issue on our end, and if it is not and you have given the user some tools to solve it themselves, it is okay to let them go on their own, other community members will also jump in if they feel they can help and we should be encouraging this. The best way to encourage users to help themselves/others is to get out of their way.

## What we care about

Your writing and code do not need to be perfect. We get that you have a life outside of work. What we're looking for is:

* The ability to reason about customer problems
* Google skills
* Writing developers will understand
* Just enough Rails skills to get by 

Do not spend time on:

* Multiple edits to your writing
* Making the Rails app pretty
* Code tests

If you've ever written rails before, we expect the Rails challenge to take about 30 minutes. You can spend as long as you need, though, don't stress if you're learning on the fly.

We think the written responses should take about 1.5 hours total. When we write responses to customers, we usually spend about 10 minutes each. We're not immune to typos ether.

## Submitting your work

We'll invite you to a private GitHub repo based on this template. 

Do all of your work in the `main` branch. Don't bother with PRs, branches, or spend time on tidy commits -- we have software to help us review. Just don't force push over the initial commit or we can't generate a diff of only your work.

Add your written responses and a link to your deployed Rails app in [RESPONSES.md](RESPONSES.md).

When you're ready, let us know and we'll schedule it for review. Make sure you add the URL to your deployed Rails app!

We review submissions once a week. You'll hear back from us no matter what by the end of the _following_ week, possibly sooner if you submit early in the week.
