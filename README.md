# Popular-Site-Subdomains
A list of subdomains for some of the most popular sites on the internet. Made as a result of [this tweet]
(https://twitter.com/soaj1664ashar/status/777182478075326464). "Sometimes simple things are ignored" - nobody should struggle and waste time trying to find subdomains for sites.

# Why?
There are plenty of reasons why people sometimes want a list of subdomains for a website. Whether you're just curious what type of stuff
the company are working on or you want to check for security vulnerabilities, a list of subdomains can really come in handy. Not so long back
someone figured out that he could get in to [anybody's Facebook account](http://www.anandpraka.sh/2016/03/how-i-could-have-hacked-your-facebook.html) 
due the a vulnerability that was only there on their very old subdomains.

#Why the Fork ather than update Jamie's Page.
Well there are 2 reasons. 
1) it was a permission issue with attempting the GitHub push, This is quicker for me and also easier as I'm still testing my RedTeamRecon tool which is being used to find all of these newly added SubDomains.
2) the next reason is linked to the top and why do it at all, well it's the same question as why reinvent the wheel, ANSWER = my wheel is rounder


# Contribute to this list with how you found a Sub I missed.
At the moment RedTeamRecon is I beleive the most through and detailed SubDomain Scanner out there. It only uses OSINT and does not touch a scanned hosts network at all. All of the Subs in this updated list are found with ZERO bruteforcing. 
To reiterate there it currently has no brute force functionality but would be an easy addition if people requested it.

# Thanks  
In no particular order I should thank the people who got me to where I am today. Many of them helped without knowing it. 

Fravia (RIP) - Back in the day You tought me how to "Really" search the web and find what is hidden, and that helped me to make my contributions to the next person.
Johnny Long - I had been working on dorks without giving it a name for ages and then somehow found you and the forums. thanks for creating an amazing place where a collective formed to create what became known as Google Dorks and us you named Google Masters :-)
Rain Forest Puppy (RFP) - Again tought me tons when I hungry to learn. 
LOPHT, Cult of the Dead Cow, Robert Hansen and Jeremiah Grossman - Again lessons learnt. Thanks for sharing 
Guy from GulfTech Security - Sorry I forgot your name but these newly updated Subdomain lists really should be dedicated to you. About 12 years ago we had been speaking and you had created one of the first SubDom scanners I had seen. I think it was in perl/python and I thought I'm sure I could program a tool to do that and quicker. And within a few months I had. this list and the RedTeamRecon tool is the result of iterations (hundreds/thousands over the years). Thanks for the initial spark. We lost contact as you got hit hard by Hurricaine Katrina. Hope everything worked out for you.

# Contribute to Jamies List 
The idea behind this is to let everyone contribute and get a fairly big list of subdomains of all the most popular sites on the internet.

Before opening a pull request, please make sure that:

* Each domain has its own .txt file, eg. Facebook.com.txt, Facebook.co.uk.txt
* There are no duplicates in the list
* The list is in alphabetical order, [you could use this site to do that](http://alphabetizer.flap.tv/)
* http:// or https:// is not in any of the subdomains (as well as no trailing slashes at the end of the domain)

If you're not sure how you can help out, [this site can find subdomains ](https://pentest-tools.com/information-gathering/find-subdomains-of-domain) for you but it also includes the IP addresses which we don't really want. What I do is open open the list in Notepad which has subdomains like:

Facebook.com  127.0.0.1

m.Facebook.com 127.0.0.2

Next, to get rid of everything other than just the subdomain do a regex find and replace. Find "[ \t].*" and replace it with "\1"
