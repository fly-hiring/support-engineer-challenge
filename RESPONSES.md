#### Support Email Response

Hello Alex, 

I hope you are doing well!

My name is Saurabh, one of the support engineers at Fly.io and I will be glad to help you.

I’m sorry you are facing this issue and can truly understand the frustration on your end. May not make sense to face it while deploying the second time when it deployed successfully the first time. 

While going through the short log you sent, I see an error message on c2258102
: v83 failed - Failed due to unhealthy allocations

Unhealthy allocations errors mean the app could boot alright but couldn’t connect to our health checks. Normally this happens when an app is listening on 127.0.0.1 , or an app is listening on a different port than internal_port in the config. Unhealthy allocations can also happen when a process crashes after it boots too.

Have you had a chance to go through our community forum where other developers post about these issues they faced while deploying? You may find some posts with similar issues as you.

I see two posts that could be relevant. Have a look here:
https://community.fly.io/t/v3-failed-failed-due-to-unhealthy-allocations-no-stable-job-version-to-auto-revert-to-and-deploying-as-v4/4274/5 

https://community.fly.io/t/source-of-deployment-failing-due-to-unhealthy-allocations/4247 

If this is not the case, I’d like to ask a few questions, please. May I please know in what language or framework your app is written? Was there any major update done to the app? Also, could you forward me the fly.toml, please? 

---

#### Support Email Troubleshooting steps

Hey Alex,

I have a few recommendations for troubleshooting the issue that may help. This is what I would do:
1. Go through the troubleshooting docs of fly.io: https://fly.io/docs/getting-started/troubleshooting/ and make sure all the standard requirements are in place from Port Checking until the end.
2. Logs tell the entire story: Try running the logs with fly status --all then fly logs -i <id> of one of the failing vms which should give you a little more information.
3. Take a look at the community forum. There may be someone who had the same issue as you who then ended up solving with. 
4. Some of the syntaxes of the tech you are using to build the app would be depreciated. Worth taking a quick peek into it. 

If none of the above works, let me know and I can check internally if we have any kind of outages at the moment. Or perhaps check with the internal team to troubleshoot it. 


---

#### Community Forum Response

Hello there,

Can you run "fly logs" to see if it throws any issues or errors?
After that, try running "fly status --all" to see if the app did really deploy. 

Maybe take a look at the way Greg did here on this post: https://community.fly.io/t/503-error-when-resuming-an-app/1173

---

#### Rails App URL

Once you've deployed your Rails app, put the link here: `<app>.fly.dev`
