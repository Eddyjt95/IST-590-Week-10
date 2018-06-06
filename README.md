# IST-590-Week-10

# IST 590: Week 10 Assignment

## Part 1

### Challenge 1.0: Hello, Shodan

In this challenge, I have created a Shodan account; you’ll notice that I am signed in since it says “My Account on the upper right instead of “Login or Register”:

<img src="https://i.imgur.com/tXN3kew.png?1"/>

### Challenge 1.1: Webcams

In this challenge, I looked around to see what kind of contents Shodan has. I found some IP addresses dedicated to webcams:

<img src="https://i.imgur.com/pAzZLce.png?1"/>

### Challenge 1.2: Filtering

> Challenge: use the filters in Shodan to find a specific target, which is a public webcam at a zoo in Japan. Here's some information:

* The hostname contains "p6026-ipbffx02yosida"

* The port "8080" is exposed

* The asn (network identifier) is “AS 4713”

It appears that the host does not exist. It could be that it was removed, or the filter provided by code path no longer works or does not return the specific result:

<img src="https://i.imgur.com/gugF7rr.png?1"/>

## Part 2: The Darknet & Cryptocurrency

### Challenge 2.0: Tool Up

I have set Tor up as specified by both codepath and this site. Below is the work URL of a guide I used and a working VM with Tails running along with an opened TOR browser: 

[https://tails.boum.org/doc/advanced_topics/virtualization/virtualbox/index.en.html]

<img src="https://i.imgur.com/5vl7yWL.png?1"/>

### Challenge 2.1: Switching Circuits

I have attempted to switch circuits about 19 times. And I was not able to connect to the Craigslist site:

<img src="https://i.imgur.com/i70P8wh.png?1"/>

### challenge 2.2: Onions

I have followed code path’s guide on entering these .onion websites. The first website appears to be a News outlet while the second site is a search engine:

<img src="https://i.imgur.com/GKZCLqI.png?1"/>

### Challenge 2.3: Into the Darkness

I have attempted to connect to the links provided by code path, which you can see within the following image (some were Not Available (N/A) while others were):. 

* The first left window: The Hidden Wiki (N/A)

* The top-middle window: Anarchist Bookstore (Avail.)

* The bottom-middle window: ParaZite – forbidden files (N/A)

* The right-upper window: Ahmia search engine (Avail.)

* The right-lower window: Onion Crate search engine (N/A)

<img src="https://i.imgur.com/WxiDeIz.png?1"/>

### Challenge 2.4: How (Not) To Get Busted

I followed the code path guide on selecting a new identity, which clears out all cookies that have been saved and it took me back to the tails website. Next, the guide mentioned that a user could experiment with the security settings that could help a user stay safe when navigating within the TOR browser. When opening the “Security Settings…” tab, you are presented with 3 options: Standard, Safer, and Safest. The Standard option is the default option that all TOR browsers are configured too. The Safer option disables some features on website, such as: JavaScript (in non-HTTPs sites), Some fonts and symbols, and audio as well as video options are “click-to-play.” The Safest option disables all JavaScript, some fonts, symbols, icons, and images are disabled, but audio as well as video options are still “click-to-play”

<img src="https://i.imgur.com/ovIBRIL.png?1"/>

### Challenge 2.5: Then Came The Money

In this challenge, we took a look at bitcoin and a bitcoin wallet. The code path guide had us look into an address which is said to contain and be controlled by the creator of bitcoin, Satoshi Nakamoto. The amount of bitcoin (mBTC) in this address is:  $168,585,002. However, to get the true amount, the mBTC must be divided by one thousand (1,000), so $168,585,002 / 1,000 = $168,585.002 (Bitcoin available).

<img src="https://i.imgur.com/e7DPiaV.png?1"/>



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
