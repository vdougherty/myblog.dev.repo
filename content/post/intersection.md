---
title: "Intersection of Mental Health and the Developer"
date: 2024-04-20T13:41:49-07:00
draft: false
framed: false
cover: "/img/intersection.jpg"
coverAlt: "The struggle is real"
coverCaption: "Photo Courtesy of Pixabay and tookapic"
description: "Recently, within the last few weeks, there was an attempted backdoor into Linux using XZ. You may have heard about it, you may have not. You can ..."
---

Recently, within the last few weeks, there was an attempted backdoor into Linux using XZ. You may have heard about it, you may have not. You can read the [details here](https://arstechnica.com/security/2024/04/what-we-know-about-the-xz-utils-backdoor-that-almost-infected-the-world/). Had it gotten implemented, it would’ve compromised SSH, rendering every Linux personal computer, server, appliance (think IoT) vulnerable at a possibly profound level. This definitely was a supply chain attack. As I followed the developments over the course of the next few days, it became apparent that the attackers or attacker, had purposely picked a project with one sole maintainer. With the intent of social engineering him into granting co-maintaining of the project so that they could inject compromised code into the project.

Their methodology was plain and simple: Pressuring him into appointing a co-maintainer.

At one point the maintainer, in response to whether XZ was still being maintained ended up having to defend himself as to why releases were moving slowly:
>
>“I haven't lost interest but my ability to care has been fairly limited mostly due to long term mental health issues but also due to some other things. ”
>

I read this and felt that one. 

#### The Impostor

I came to my chosen field late in the game in terms of age, I was a freshly minted graphic designer at 35, with an AA in Applied Science from an art school known more for it’s “Draw Skippy” cartoon advertisements on match book covers, than any particular designer that graduated from said school (although Alex Ross is an alum). I was lucky upon graduation, that through a family connection I got hired to work for a major ad agency on a globally recognized brand, just as the internet exploded. I very quickly learned that my education level was viewed by some as lacking, since I did not posses an undergrad degree in CS. 

Which is to say, that I’ve always been dogged by “Impostor Syndrome” to one degree or another:

>
>“Impostor syndrome, also known as impostor phenomenon or impostorism, is a psychological occurrence. Those who have it may doubt their skills, talents, or accomplishments.”
>

Over the long course of doing web related development, whether as a direct hire, or as a contractor, there was always a sense of pulling rabbits out of hats to solve what ever immediate need presented itself. I got good at masking the impostor. I also got good at what I do. But, when you add mental health into the equation, maintaining emotional health or just trying to maintain a healthy set of boundaries surrounding work life balance, it adds an extra layer to navigate on top of the stress of achieving what ever goal has been handed to you. It’s hard to find balance when your internal life feels unbalanced. It’s harder still when you are constantly under the gun to produce clean code that gets results. 

#### Code, Code, Code

Back in the early days of the web, especially during the IPO madness, there was a troupe about the renegade CEO who would publicly announce nonexistence features, then would commit to impossible timelines for that set of features to be implemented. I believe IBM even used it for the basis of a commercial. Except, I actually lived through that. In my instance it resulted in a nonstop 3 month coding jag, to redesign, retool and reimplement an online entity from the ground up, I basically lived in my office going home every 3-4 days to actually sleep in a bed, also to shower. (Note to the wise, do not fall asleep with your feet up on one office chair and your butt in another, gravity is a cruel mistress. Sleep on the floor.) During this frantic rush to build and release, our head admin in charge of the all the servers at the time, said it reminded him of the Russian roulette scene in the Deer Hunter, except instead of screaming in Vietnamese as the gun was passed, they’re screaming “Code, Code, Code!!!” This is why code refactoring is such a good thing. This is why Agile and Scrums are your friends. At least ideally.

I could go on about other anecdotes from my development past, there are many. Ask any older developer, we all have our war stories of being up way into the middle of the night coding in isolation. All these war stories share one thing in common, we were subjected to extremely stressful situations repeatedly, with the onus of a date on a calendar. Sometimes referred to as the “Drop Dead Date”.  

#### This isn't the Matrix

We as a society romanticize the person coding alone in the night… the lone “hacker”, black hoodie on, face in shadow. In the negative, they are all powerful, able to effortlessly pawn systems and by pass security, spy on your loved ones and wreck havoc upon the innocent, while casually sipping an energy drink. In the positive, they are the antihero not nearly as powerful as the villain, but as capable, eventually thru perseverance and pluck they defeat the system and their antagonist, for some reason always on an Apple computer, while casually sipping an energy drink. However, neither is the reality of what coding really is about, well, except the energy drink. Stripping away this artifice, what we find is not some fashionable person clad all in black, wearing thinly disguised bondage gear and great looking thrift store finds. True, hoodies maybe worn, but that’s mostly because the office is cold. What you discover is a person with a CS degree, or certifications that qualify them for the said job at hand. They are usually part of a team contributing to long term projects and short term projects and are more concerned with their day to day life and their upcoming Scrum. Romanticizing working in isolation is really not a good thing and yet, “May require after hours work and some weekends” is considered a standard part of employment in development. 

When you consider that 1 in 6 people in society (US) have a mental illness of varying degrees and there are 4.3 million developers (US) you realize this potentially is a lot of people. Couple this with a society still coming to grips with a host of post-pandemic issues: political upheaval, price gouging by corporations, wages not tracking with inflation or corporate profits, the debate of return to work policies. There’s a lot of reasons for the average person to not feel comfortable in their own skin, let alone focus on their own internal needs. I personally have struggled with emotional health issues over the years. I’ve been divorced, which frankly was a bit messy, reunited with my daughter after a 30 year absence, not so messy, helped her through her divorce and custody fight for my grandson, really messy. There were very real, emotionally impactful decisions along the way, that at times would leave me awake in bed wondering how I would get through the next day. Juxtapose that against a job possibly having issues from the top down or bottom up, and it will wear on you. During those periods I was grateful for friends and therapy. 

But all of the above becomes laser focused when leadership of a team revolves around a person or persons who really just see their employees as replaceable cogs, to serve their/the bottom line. It becomes rather apparent, rather quickly, when this happens. This often will contribute negatively to a persons emotional health and sense of stability. Couple that with long hours, sometimes isolation, the internal pressure to perform, intentional or unintentional pressuring via unrealistic timelines, and very suddenly the same “feeling limited” can become a very real issue whether in open source or closed source.  

#### No is still a complete sentence

In open source development as opposed to close source, there is the ideal of the maintainer being a hobbyist, working away on some widget to solve a particular problem that they encounter which they then release to the world to prevent others from encountering the same issue. They code and maintain because it’s important to them. Which is great stuff, except when your widget succeeds to the point that it actually interacts with a core part of Linux as XZ did. It’s understandable how the maintainer got to where he found himself, there were no less than 4 individuals pressuring him to appoint a co-maintainer. Their end objective was pushing him into handing part of the control of the project over to them (In all likelihood it was one individual, masquerading as the 4 other individuals through fake accounts.) Having someone constantly remind you of how impactful your widget is, or that contributors and end users have expectations, when you yourself are doing less than spectacular. Well, I can only imagine what started out as a hobby becomes a second job, it’s just that the cast of characters surrounding you change from your day job. Burnout is the same in closed source as in open source, and while “No” is still a complete sentence, we all want to do what we feel is right, to not be seen as neglectful.

Many believe there is a lack of understanding that has arrived with Linux users who are used to closed source software updates, they often do not understand that maintainers do not owe contributors or the end user anything, beyond “I’ll release it when it’s ready.” The truth is they do not owe you. [Read here](https://mikemcquaid.com/open-source-maintainers-owe-you-nothing/). 

In closing, I applaud the maintainers transparency in his response to the pressure campaign, he was forthright, direct and honest. After all, it was the maintainer who caught the back door. It also was the maintainer who reported it immediately. As we used to say on one job, as the highest form of compliment, “Good catch.”

However it is ironic, that after taking 2 years to ingratiate themselves into the XZ project, that the “attacker or attackers” had failed in their state sponsored mission to compromise the project. There is [ample evidence](https://rheaeve.substack.com/p/xz-backdoor-times-damned-times-and) that for them this was a 9 to 5 job, that included time off for holidays. Hmm, I wonder how their "on the job" metal health is doing?

-- E’nuf said, Love and Rockets 

#### Resources:

[Helpful ideas on maintaining emotional health for developers and teams:](https://www.thecodingdiva.com/blog/coding-and-fitness/navigating-coding-mental-health)

[Helpful ideas for software developers](https://www.softwire.com/insights/how-to-take-care-of-your-mental-health-as-a-software-engineer/)

[Find a therapist](https://www.psychologytoday.com/us/therapists)


{{< rawhtml >}}
<p>&nbsp;</p>
{{< /rawhtml >}}

#### Leave a comment:  

{{< chat veeroom >}}



