# trt_data_lit_grp_python
The Repository for Learn Python Hard Way: Mining Social Media Series

Installing Python
---------

If you don't have python on your computer already, please install Anaconda Python 2.7
Follow the instruction here and select the most appropriate option based on your OS
https://www.continuum.io/downloads

Twitter API Access
---------
In order to get access to the Twitter API through OAuth (open standard for authorization), 
we have to obtain our consumer information and access tokens first by registering 
our app on https://apps.twitter.com.

1. Go to https://apps.twitter.com/ and log into your twitter account

2. Click on "Create New App"

3. Obtain the Consumer key, Consumer secret, Access token, and Access token secret. Save them somewhere.
DO NOT SHARE THIS INFORMATION WITH ANYBODY ELSE!

Test Twitter Access
---------
1. We will use Twython to access Twitter data, you can install it by 
```
pip install twython
```

2. Now, create a Twython instance with your Consumer Key and Consumer Secret

```
import Twython

APP_KEY = 'YOUR_CONSUMER_KEY'
APP_SECRET = 'YOUR_CONSUMER_SECRET'
OAUTH_TOKEN = auth['oauth_token']
OAUTH_TOKEN_SECRET = auth['oauth_token_secret']

twitter = Twython(APP_KEY, APP_SECRET,OAUTH_TOKEN, OAUTH_TOKEN_SECRET)
```

3. Let's try to post a status on your twitter account through Python
```
twitter.update_status(status='I am going to TDLG to Learn Python the Hard Way!')
```

4. Check your Twitter Profile. Hooray! You have completed the Prerequisites! See you the session!

Credits
---------
* [Mining Social Media Web 2nd Edition](https://github.com/ptwobrussell/Mining-the-Social-Web-2nd-Edition)
