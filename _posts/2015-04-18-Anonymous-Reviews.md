---
layout: post
title: "'Did I only get in because I'm a woman?' - Why We Implemted An Anonymous Review Process"
description: "Even a positive bias can have negative consequences. By encouraging woman to apply for Hackership we may give the false impression that we accept women into the programme only because of their gender. To combat this notion we implemented an anonymous review process. Here's how we did that.
"
category:
authors:
    - anouk
tags: ["hackership", "review", "applications"]
image: /content/2015-04-18-mask.jpg
---

From the early days of Hackership we have tried to encourage women to apply. We value diversity and want to create a safe environment for people from all genders and backgrounds. If that means we need to encourage and actively reach out to women (among others) then that's what we will do.

![Anonymous Reviews](/content/2015-04-18-mask.jpg)

But, there's one problem.

As soon as we start urging women to apply, it becomes very easy for women to believe they were only accepted because they have a vagina. Or, for others to think that about them. As a woman in tech, I can relate. More than once I caught myself thinking: “Am I really as qualified as the guy sitting next to me? Or am I only here because of some quota?”

Obviously, this is not the outcome we hope for, quite the opposite. But then, **how do we encourage women to apply, while also making sure every applicant knows we do not have a bias** (in either direction)?

It occurred to us that just saying ‘we don’t have a bias’ wouldn’t be very convincing to anyone. So, instead, we went a couple of steps further and eliminated the need for applicants to trust our biaslessness (try saying that ten times fast) by implementing an anonymous review process.

In a nutshell: when an application comes in it is stripped all identifying factors, like gender, age, or nationality. Then, and only then, is it send to reviewers who will review the application, ask follow up questions and make judgements based on merit. **So, while we encourage women to apply, the moment they do gender stops being a factor.**

##The Anonymous Review Process - a closer look
Once we figured out the solution (theoretically speaking), the next step was building a piece of software that could automatize this process in such a way as to ensure that a) the review process is in fact anonymous and cannot be cheated by one of the reviewers and b) we can still process large numbers of applications.

![Application Process](/content/2015-04-18-application-process.png)

For those interested, here's how it works under the hood:

###Step 1. Application form
In the application form there are a couple of fields that are marked 'anonymous'. These are the fields we take out and put in the anonymized application. Everything else will never be viewed by our reviewers.

###Step 2. An application arrives
One of our admins (who are not reviewers) triple check the anonymized application to make sure there's no way to identify the applicant. When done, the application is marked ready for review and two reviewers will be randomly selected to review the application.

###Step 3. Review
The reviewers read the anonymized application and ask follow up questions to the applicant. They can also comment and make recommendations.

###Step 4. Follow-up questions
Once the reviewers have done their job and asked questions, the moderator (who has only ever seen the anonymized application) will make sure the questions are relevant and then sends them out to the applicant. The e-mailing is completely anonymized. The questions are inserted into a template, which contains the name of the applicant, so that the reviewers and moderators never access this information.

###Step 5. Receiving answers from the applicant
The e-mail is send from a dedicated e-mail address (each applicant gets it's own), so that when the applicant answers, we get know who it is from, without needing to see the name. The incoming e-mail is then anonymized by admins the same way the application was before (step 2).

###Step 6. Reviewing the replies
The reviewers will read the anonymized e-mails (i.e. replies to their questions) and give their feedback and comments. At this point we know with relative certainty whether we want to admit an applicant.

###Step 7. Skype call
This is where we break out of the anonymous stage and, for that reason, we had some discussion about whether we should include this phase. We decided in favor of a Skype call because we think it is important to give applicants a chance to ask their questions. In addition, it's a chance for us to ask more follow-up questions and give feedback on specific project ideas.

Obviously, this is a moment in the process where bias could be introduced and influence the outcome. To combat that, the anonymous part of the process should already result in a strong recommendation. Basically there are four imaginable scenarios:

1. The reviewers tell us that this person is suited for Hackership. Result: we have a Skype call just to get to know the applicant 'in person' and answer any questions they may have.

2. The reviewers tell us that this person is suited for Hackership, BUT they may have one or two concerns that should be removed before accepting the applicant. Result: we have a Skype call where we bring up these concerns. We then relay the applicant's answers to the reviewers (anonymously), who will make a final decision. In addition, we answer any questions the applicant may have.

3. The reviewers tell us that this person does not seem suited for Hackership, UNLESS they clear up the open issues/concerns. Result: we have a Skype call where we bring up these concerns. We then relay the applicant's answers to the reviewers (anonymously), who will make a final decision. In addition, we answer any questions the applicant may have.

4. The reviewers tell us that this person is not suited for Hackership. Result: we do not move forward.

###Step 8. The decision & Grant applications
The applicant is informed of our final decision. At this stage, and only at this stage, we go back to our records and find out whether this applicant applied for a grant. If so, we start the grant application review. This way, whether or not an applicant has applied for a grant does not impact our decision to accept the person into the programme.

##Final notes
This is our first implementation of an anonymous review process and as such, there is definitely room for improvement. So, if you feel there's something missing or you have a suggestion for improvement, do not hesitate to reach out to us, we very much welcome any and all feedback!

Also, should you want to implement your own anonymous review process (and we very much encourage all companies to do so!), please have a look at the [open source review tool](https://github.com/Hackership/reviewapp-backend) we build. It's still in beta and currently only configured for our internal use. However, in the near future, we hope to transform it into a more general review tool that is easily customizable, so that other organizations can use it too. So stay tuned!

---
***Thanks to [Turinboy](https://www.flickr.com/photos/turinboy/) for making this beautiful image available under creative commons.***
