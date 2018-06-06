# IST-590-Week-10

# IST 590: Week 10 Lab

## Milestone 0: Kali Gone Wild

I setup Kali just as how it is specified within the codepath guide

<img src="https://i.imgur.com/wyo7Omq.png?1"/>

## Milestone 1: Hello, SET

I followed the guide to send myself a couple emails. At first I had trouble sending them. I would not receive any emails. I figured that on the password section, when choosing a target email, you are supposed to enter the password for that target email. During my third attempt, I used the password for the target email and received an email.

<img src="https://i.imgur.com/oYZHKB7.png?1"/>

<img src="https://i.imgur.com/0E1RVmq.png?1"/>

## Milestone 2: Try a Real Payload

* Take a moment to read the available options. There's a clear pattern here of malicious payloads embedded in the kinds of files you'd typically see as email attachments: PDFs, ZIP, even RTF.

> Which two software companies are heavily represented on this list?

Microsoft and Adobe are both heavily represented on the list

> Which operating system would most of these exploits require?

It appears that these exploits cater to Microsoft Windows


I attempted the challenge with an actual payload, but the email failed to deliver. Codepath expected this to happen since Google scans pdf files and will detect and drop any malicious files:

<img src="https://i.imgur.com/YbuR3eG.png?1"/>

## Milestone 3: Fakebook

I have attempted to imitate a website’s log in page using the SET app from Kali. I have attempted Facebook, but it did not work. I moved on to Twitter, but it did not work as well since you need to navigate to the login page, escaping the “localhost” fake page setup. The following image is from my third attempt, using LinkedIn:

<img src="https://i.imgur.com/asmyXRc.png?1"/>

<img src="https://i.imgur.com/Heaeb8M.png?1"/>

The SET kit did not intercept any credentials for each of the attempts.

## Milestone 5: Cleanup

I am switching the adapters from bridged to NAT as shown in the following images:

<img src="https://i.imgur.com/OyCleUy.png?1"/>

<img src="https://i.imgur.com/71iHE7G.png?1"/>

VM still works after switching to NAT again

<img src="https://i.imgur.com/EPPPkPR.png?1"/>

## Milestone 6: SE In Situ

> What vulnerabilities were beyond the control of the user?

There was a security flaw in place within Amazon. Through Amazon, hackers were able to see a 4-digit portion of the user’s credit card, which Amazon deemed safe enough to show to the public. This 4-digit piece of information was used on Apple to verify the user’s ID

> What if anything could have been done by the user to mitigate the severity of the attack?

The user mentioned that the hackers were able to login to his twitter by piggybacking from one platform to another. Hackers gained one piece of information that led them to the next piece. The user also mentioned that the hackers were able to login to his twitter via his Gmail account. The hackers attempted to recover information, which they managed to do so because the user did not have two-factor authentication turned on. The user could have minimized the attack if he had the two-factor authorization option on.

> What could the user do to mitigate this, making a successful login impossible for the attacker even with the credentials? (Hint: FB offers this as an option; not all sites do)

Facebook has a two-factor authentication which can help minimize unauthorized logins by unknown entities.

> Why might the username/password still be of value to the attacker even if she can’t use them to login to Facebook? (Hint: think about how users come up with passwords)

People do not bother to use random characters consisting of numbers, letters (upper/lower case), and symbols because they do not want to remember complex passwords. The solution to this is for them to use the same password for each site to make life a little easy. With that being said, if a hacker uncovered a username and password from someone, they can plug in those same credentials to a bunch of other sites; it will be a matter of time before they are able to log in to another site with the same username and password.
