# HCI584
## _Twitter Sentiment Analysis_
Repo for HCI 584 Summer 2022

![Project Image](https://iowastate-my.sharepoint.com/personal/imalma_iastate_edu/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fimalma%5Fiastate%5Fedu%2FDocuments%2FHCI%20584%2Fgithub%2FTwitter%5Fsentiment%5Fanalysis%5FHCI584%2Fproject%2EPNG&parent=%2Fpersonal%2Fimalma%5Fiastate%5Fedu%2FDocuments%2FHCI%20584%2Fgithub%2FTwitter%5Fsentiment%5Fanalysis%5FHCI584)

This app allows for users to search up a hashtag to retrieve the given sentiment surrounding it, whether it is positive, negative or neutral. 

- Sorts tweet by most recent to oldest
- Simulate user input via hardcoding values
- Put results on GUI
- ✨Magic ✨

## Project structure

- TwitterSent1 - GUI version.py: Main file with GUI
- TwitterSent1 - Elevated Version.ipynb: Standard access via Twitter Developer

## Buy me a coffee
Whether you use this project, have learned something from it, or just like it, please consider supporting it by buying me a coffee, so I can dedicate more time on open-source projects like this :)
[Buy Me a Coffee](https://www.buymeacoffee.com/almagueris9)

## Tech

This project was made possible using the following:

- [Visual Studio Code](https://code.visualstudio.com/) -editor!
- [Developer Platform](https://developer.twitter.com/en) - Twitter API to listen to and analyze the public conversation, engage with people on Twitter, and innovate.
- [Python](https://www.python.org/) - Project made possible with this programming language

And of course Dillinger itself is open source with a [public repository][dill] on GitHub.

## Installation

In order to run this project, it is recommended to sign up for an account for Twitter's [Developer Platform](https://developer.twitter.com/en). At the time of this project, there are three levels of access available, Essential, Elevated, and Acedemic Research. 'TwitterSent1 - Essential Version' will run using the essential version of Twitter's API. This is the free version recieved once you sign up for an account. 'TwitterSent1 - GUI version' will run with the elevated access. An application must be submitted in order to run this. 

More information on the access levels can be found [here](https://developer.twitter.com/en/docs/twitter-api/getting-started/about-twitter-api).

## Plugins

Once a Twitter Developer account is made, it is recommended to store all your access keys and tokens within a csv file.
The csv file will house the consumer_key, consumer_secret, access_token, and access_secret

```sh
config.csv
```
![Code here](https://iowastate-my.sharepoint.com/:i:/r/personal/imalma_iastate_edu/Documents/HCI%20584/github/Twitter_sentiment_analysis_HCI584/config.PNG?csf=1&web=1&e=M75AbF)

Within the GUI version of the project you will see the following to retrieve the code from your file:
```sh
    #============================Insert here twitter API keys===========================
def r_twitterApiKey():
    config = pd.read_csv("config.csv")
    twitterApiKey = config['consumer_key'][0]
    return twitterApiKey
def r_twitterApiSecret():
    config = pd.read_csv("config.csv")
    twitterApiSecret = config['consumer_secret'][0]
    return twitterApiSecret
def r_twitterApiAccessToken():
    config = pd.read_csv("config.csv")
    twitterApiAccessToken = config['access_token'][0]
    return twitterApiAccessToken
def r_twitterApiAccessTokenSecret():
    config = pd.read_csv("config.csv")
    twitterApiAccessTokenSecret = config['access_secret'][0]
    return twitterApiAccessTokenSecret
    #============================End twitter API keys section===========================
```

## Usage

After you clone this repo to your desktop, insure that your config.csv file is saved within the same area of the project. Any name changes will need to reflect in both the csv file and code. The following python libraries will need to be installed in order to use the code:

- tkinter
- tweepy
- textblob
- wordcloud
- pandas
- re
- matplotlib
- pylab

No additional installs required. 

## License

MIT

**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
