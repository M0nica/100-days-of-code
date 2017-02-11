# 100 Days Of Code - Log

### Day 1: January, 10th, 2017
##### #BlackGirlMagic Twitter Bot

**Today's Progress**: Created the framework for a Twitter bot that will retweets tweets mentioning #BlackGirlMagic that have more than X amount of RTs. I was able to run the script on my local machine and RT pertinent tweets. 

**Thoughts:** I was able to get my Python script to work with Twython locally. However, after trasnferring the script to DigitalOcean my script broke and I am not sure why :( I submitted an issue to Twython's GitHub repo and will continue to research this issue. As being able to schedule automated cron jobs in DigitalOcean server is crucial to automating this bot!
Additionally, need to research best practices to avoid recieving 403 error for trying to RT the same tweet. I was hoping that this project would be 100% done in one day but alas - coding is always a bit of a game :-) 

Link to my open issue: https://github.com/ryanmcgrath/twython/issues/437

**Link to work:** 
- [BlackGirlMagic (GitHub Repo)](https://github.com/M0nica/blackgirlmagic)
- [Twitter: @BlackGalMagic](https://twitter.com/blackgalmagic)


### Day 2: January, 11th, 2017
##### Refactored & Improved #BlackGirlMagic Twitter Bot 

**Today's Progress**: Refactored the code in my #BlackGirlMagic twitter bot to iterate searching through a list of related hashtags. Also, was able to get the script to run on my Digital Ocean droplet so now it's actually a bot! I created a cron job to run my script every 5 mins. 

**Thoughts:** 
Submitting an issue on GitHub is relatively painless and I was able to quickly resolve my issues with running Twython on Digital Ocean after submitting an issue. I am still recieinvg 403 errors when my script tries to RT a tweet the account has already retweeted.Will look into ways to cache this value without it getting overriden when the script is run again. May need to store all retweeted tweets in a seperate file. However, this seems like it may be overkill since I chose popular hashtags (which update frequrntly) and the script is only trying to RT the 2 most recent tweets for a given hashtag at any given time. 

In the couple of hours that my bot has had the training wheels off I recieved a 3 followers and was added to 2 lists. 

Link to my closed issue: https://github.com/ryanmcgrath/twython/issues/437ffffff

**Link to work:** 
- [BlackGirlMagic (GitHub Repo)](https://github.com/M0nica/blackgirlmagic)
   - [BGM Python Script] (https://github.com/M0nica/blackgirlmagic/blob/master/blackgirlmagic_rt.py) 
- [Twitter: @BlackGalMagic](https://twitter.com/blackgalmagic)

### Day 3: February, 5th, 2017
##### Flask App to Auto-Detect Weather 
**Today's Progress**: Created a Flask app that uses ipgetter to get a user's IP address and then used http://freegeoip.net to get more specific location information to pass into Weather API. Weather information (current temperature and % chance of rain) is returned based on the location associated with the IP. 

**Thoughts:** 
I am looking forward to re-factoring to beautify with CSS and ask user for location input if the script is unable to detect their location or if they would like the weather from a different location.


**Link to work:** 
- [Detect_Location_Weather (GitHub Repo)](https://github.com/M0nica/flask_weather/blob/master/detect_location_weather.py)
  



### Day 4: February, 6th, 2017
##### Flask App to Auto-Detect Weather - Enhancements
**Today's Progress**: Added in a template weather.html to display the weather information and include an appropriate weather icon (https://erikflowers.github.io/weather-icons/) based on what the current weather is. I play around with the Flask app structure and was able to get everything to work well.

**Thoughts:** 
Next, I would like to add additional CSS styling and pull in hourly weather info to display in the weather.html page -- so that it displays the current weather & hourly projections. Preliminary research revealed I will have to convert time from Epoch Unix Time to something tha makes sense for hte user. http://www.unixtimestamp.com/index.php

**Link to work:** 
- [Detect_Location_Weather (GitHub Repo)](https://github.com/M0nica/flask_weather/blob/master/detect_location_weather.py)


### Day 5: February, 7th, 2017
##### Flask App to Auto-Detect Weather - Enhancements
**Today's Progress**: Updated the styling of the app, worked on the rain language logic and added my first `.gitattributes` file.

**Thoughts:** 
To re-iterate my thoughts from yesterday I need to add CSS styling and pull in hourly weather info to display in the weather.html page -- so that it displays the current weather & hourly projections. Preliminary research revealed I will have to convert time from Epoch Unix Time to something tha makes sense for the user. http://www.unixtimestamp.com/index.php

**Link to work:** 
- [Detect_Location_Weather (GitHub Repo)](https://github.com/M0nica/flask_weather/blob/master/detect_location_weather.py)
  


### Day 6: February, 8th, 2017
##### Kicked off contributions to Code Corps
**Today's Progress**: I set up my developer environment to play nicely with [Code Corp](https://github.com/code-corps)'s ember app. I needed to install `npm` `bower` `ember` since my hardrive was recently wiped! I was able to get the app running locally and reached out to other members throughout the process. 

**Thoughts:** 
Contributing to open-source projects can be fun! It seems like others are eager to help and there are is a wide range in the scope of issues that need help. I am looking forward to being more involved in Open Source Software initiatives moving forward. 


**Link to work:** 
I submitted two pull requests:
- [https://github.com/code-corps/code-corps-ember/pull/1026 - tackled a form validation issue](https://github.com/code-corps/code-corps-ember/pull/1026)
- [https://github.com/code-corps/code-corps-ember/pull/1027 - adding additional information to documentation](https://github.com/code-corps/code-corps-ember/pull/1027)

### Day 7: February, 9th, 2017
##### Still coding!
**Today's Progress**: My two pull requests from yesterday were accepted by Code Corps! I am looking forward to contributing more. Today, I was a bit all over the place and looked at www.data.gov for inspiration...I even sent a test Slack message from a Python Script. I ended up creating a Percent Change Calculator in Python with basic validation (requires field to be filled out + requires numeric value). 

**Thoughts:** 
I think as I progress in #100DaysOfCode I should plan out my project(s) for the upcoming week to help stay concentrated on building projects with more depth. 


**Link to work:** 
- [https://github.com/M0nica/percent-calc](https://github.com/M0nica/percent-calc)


### Day 8: February, 10th, 2017
##### Debugging Heroku!
**Today's Progress**: Worked to get my two Python apps on Heroku. However, after the deployment process I realized my apps function differently locally versus on Heroku. I am still debugging these issues. I've started to track these issues and future enhancements with GitHub issues. 

### Day 9: February, 11th, 2017
#####Finished Debugging Heroku and Better Error Handling :)
Day 9: I was able to get my percentage change calculator up and running on Heroku. This was a multi-day process because my Heroku environment was behaving differently than my local Python environment despite them both running the same version of Python they handled floats differently which needed to be resolved.
After getting the app and running I added additional logic:
- handle decimals (`step="any"`)
- error handling(`404.html/405.html`) 
- context logic for how the result is displayed based on if the % change is positive/negative/neither. 
- parameters to my URL - so that each output has a unique page URL
- layout template with header and footer for other pages to extend.

**Thoughts:** 
I am still trying to figure out how to handle required fields not being properly validated on iOS Safari. I feel a lot better now that my Flask app was properly deployed on Heroku and am looking forward to refactoring and deploying more apps to Heroku in the future.

Fun fact: Heroku doesn't charge for you to run basic apps. [https://devcenter.heroku.com/articles/free-dyno-hours](https://devcenter.heroku.com/articles/free-dyno-hours)

**Links to work:** 
- [https://percentcalc-pro.herokuapp.com](https://percentcalc-pro.herokuapp.com)
- [https://github.com/M0nica/percent-calc](https://github.com/M0nica/percent-calc)

