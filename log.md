# 100 Days Of Code - Log

### Day 0: January, 10th, 2017
##### #BlackGirlMagic Twitter Bot

**Today's Progress**: Created the framework for a Twitter bot that will retweets tweets mentioning #BlackGirlMagic that have more than X amount of RTs. I was able to run the script on my local machine and RT pertinent tweets. 

**Thoughts:** I was able to get my Python script to work with Twython locally. However, after trasnferring the script to DigitalOcean my script broke and I am not sure why :( I submitted an issue to Twython's GitHub repo and will continue to research this issue. As being able to schedule automated cron jobs in DigitalOcean server is crucial to automating this bot!
Additionally, need to research best practices to avoid recieving 403 error for trying to RT the same tweet. I was hoping that this project would be 100% done in one day but alas - coding is always a bit of a game :-) 

Link to my open issue: https://github.com/ryanmcgrath/twython/issues/437

**Link to work:** 
- [BlackGirlMagic (GitHub Repo)](https://github.com/M0nica/blackgirlmagic)
- [Twitter: @BlackGalMagic](https://twitter.com/blackgalmagicblackgalmagic)


### Day 0: January, 10th, 2017
##### Refactored & Improved #BlackGirlMagic Twitter Bot 

**Today's Progress**: Refactored the code in my #BlackGirlMagic twitter bot to iterate searching through a list of related hashtags. Also, was able to get the script to run on my Digital Ocean droplet so now it's actually a bot! I created a cron job to run my script every 5 mins. 

**Thoughts:** 
Submitting an issue on GitHub is relatively painless and I was able to quickly resolve my issues with running Twython on Digital Ocean after submitting an issue. I am still recieinvg 403 errors when my script tries to RT a tweet the account has already retweeted.Will look into ways to cache this value without it getting overriden when the script is run again. May need to store all retweeted tweets in a seperate file. However, this seems like it may be overkill since I chose popular hashtags (which update frequrntly) and the script is only trying to RT the 2 most recent tweets for a given hashtag at any given time. 

fff

Link to my closed issue: https://github.com/ryanmcgrath/twython/issues/437ffffff

**Link to work:** 
- [BlackGirlMagic (GitHub Repo)](https://github.com/M0nica/blackgirlmagic)
   - [BGM Python Script] (https://github.com/M0nica/blackgirlmagic/blob/master/blackgirlmagic_rt.py) 
- [Twitter: @BlackGalMagic](https://twitter.com/blackgalmagicblackgalmagic)






