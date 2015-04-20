---
layout: post
title: "'Did I only get in because I'm a woman?' - Why We Implemented An Anonymous Review Process"
description: "Even a positive bias can have negative consequences. By encouraging woman to apply for Hackership we may give the false impression that we accept women into the programme only because of their gender. To combat this notion we implemented an anonymous review process. Here's how we did that.
"
category:
authors:
    - anouk
tags: ["hackership", "review", "applications"]
image: /content/2015-04-18-mask.jpg
---

From the early days of Hackership we have tried to encourage women to apply. We value diversity and want to create a safe environment for people from all genders and backgrounds. On top of that, helping our industry become more diverse is high on our agendas.

If that means we need to encourage and actively reach out to women (among others) then that's what we will do.

![Anonymous Reviews](/content/2015-04-18-mask.jpg)

But, there's one problem.

As soon as we start urging women to apply, it becomes very easy for women to believe they were only accepted because of gender. Or, for others to think that about them. As a woman in tech, I can relate. More than once I caught myself thinking: “Am I really as qualified as the guy sitting next to me? Or am I only here because of some quota?”

Obviously, this is not the outcome we are looking for, quite the opposite. But then, **how can we encourage women to apply, while also making sure every applicant knows they are not admitted because of positive descrimination**?

Just saying ‘we don’t have a bias’ wouldn’t be very convincing to anyone. And, whether it's conscious or not, we DO have a bias. So, we looked around to see how other organisations are solving this problem. We found a very interesting approach, pioneered by [Courtney Stanton for the Gamer Conference](http://geekfeminism.org/2012/05/21/how-i-got-50-women-speakers-at-my-tech-conference/) and also [successfully implemented by JSConf](http://2012.jsconf.eu/2012/09/17/beating-the-odds-how-we-got-25-percent-women-speakers.html): anonymous selection.

Both conferences select speakers by having their communities vote for talk proposals without knowing the gender (or much else) of the speaker. That way that way it becomes possible to **encourage women to apply, while also making clear that the moment they do, gender stops being a factor.**

As we are not a conference, we had to adapt the process a little, but the main idea is the same. In a nutshell our application process goes as follows: applications come in on a rolling basis. Once an application arrives, it is anonymized and stripped of all factors that should be irrelevant during the review process, like gender, age, or nationality. Then, and only then, is it send to reviewers who will review the application, ask follow up questions and make judgements, based on merit.

## The Anonymous Review Process - a closer look
Once we found the solution (theoretically speaking), the next step was building a piece of software that could automatize this process in such a way as to ensure that a) the review process is in fact anonymous and cannot be cheated by one of the reviewers and b) we can still process large numbers of applications.

![Application Process](/content/2015-04-18-application-process.png)

For those interested, here's how it works under the hood:

### Automatic and manual anonymization
In the application form there are a couple of fields that are marked 'anonymous'. These are the fields we take out and put in the anonymized application. Everything else will never be viewed by our reviewers. One of our admins (who are not reviewers) triple check the anonymized application to make sure there's no way to identify the applicant.

### Sending emails
E-mails send to the applicant by our reviewers, for instance to ask follow-up questions, are completely anonymized as well. The reviewer will only write the body of an e-mail, while the header and name are added by the app. E-mails are send from a dedicated account (each applicant gets their own) and we ask applicants to reply to this account, so that once a reply arrives we do know who it came from, without ever having to see the e-mail address. The body of the reply is, again, anonymized before it is shown to the reviewers.

### Skype calls
Traditionally, at the end of the review cycle, we would have a Skype call. Clearly, this is where we'd break out of the anonymous stage and, for that reason, we had some discussion about whether we should include this phase. We decided in favor of a Skype call because we think it is important to give applicants a chance to ask their questions, too. In addition, it's a chance for us to ask more follow-up questions and give feedback on specific project ideas.

Obviously, this is a moment in the process where bias could be introduced and influence the outcome. To combat that, the anonymous part of the process should already result in a strong recommendation. Basically there are four imaginable scenarios before the skype call:

1. The reviewers tell us that this person is suited for Hackership. Result: we have a Skype call just to get to know the applicant 'in person' and answer any questions they may have.

2. The reviewers tell us that this person is suited for Hackership, BUT they may have one or two concerns that should be removed before accepting the applicant. Result: we have a Skype call where we bring up these concerns. We then relay the applicant's answers to the reviewers (anonymously), who will make a final decision. In addition, we answer any questions the applicant may have.

3. The reviewers tell us that this person does not seem suited for Hackership, UNLESS they clear up the open issues/concerns. Result: we have a Skype call where we bring up these concerns. We then relay the applicant's answers to the reviewers (anonymously), who will make a final decision. In addition, we answer any questions the applicant may have.

4. The reviewers tell us that this person is not suited for Hackership. Result: we do not move forward.

### Seperating grants applications from the normal review
Once applicant is informed of our final decision, we go back to our records and find out whether this applicant applied for a grant. If so, we start the grant application review. This way, whether or not an applicant has applied for a grant does not impact our decision to accept the person into the programme.

## Final notes
This is our first implementation of an anonymous review process and as such, there is definitely room for improvement. So, if you feel there's something missing or you have a suggestion for improvement, do not hesitate to reach out to us, we very much welcome any and all feedback!

Also, should you want to implement your own anonymous review process (and we very much encourage all everyone to do so!), please have a look at the [open source review tool](https://github.com/Hackership/reviewapp-backend) we are building. It's still in its early development and currently only configured for our internal use. However, in the near future, we hope to transform it into a more general review tool that is easily customizable, so that other organizations can use it, too. Check it out and give us your feedback!

---
***Thanks to [Turinboy](https://www.flickr.com/photos/turinboy/) 	for making this beautiful image available under creative commons.***
