# Yo [Slack](https://slack.com/) Integration

Ever want to get your team's attention when you have standup or an important meeting? You've come to the right place yo. With this repo, you can quickly setup an outgoing webhook from your Slack channels to Yo the team at a moment's notice.

## Requirements

- A [Heroku](http://heroku.com/) account
- [Heroku Toolbelt](https://toolbelt.heroku.com/) installed
- A [Yo API key](http://yoapi.justyo.co/)
- Access to your team's Slack 'Outgoing WebHooks' page
	- https://[YOUR_SLACK_DOMAIN]/services/new/outgoing-webhook
- Note: This integration will only work from within Channels within Slack!

## Setup

1. Clone this repo locally. `git clone https://github.com/Jasdev/slack-yo.git`
2. `cd slack-yo`
3. `heroku login`
4. `heroku create`
5. `heroku config:set YO_API_TOKEN=[YOUR_YO_API_TOKEN]`
  * Make sure to replace '[YOUR_YO_API_TOKEN]'
6. `git push heroku master`
7. `heroku info`
  * Copy the outputted URL on the last line to your clipboard
8. Head over to your team's Slack 'Outgoing WebHooks' page
![](http://i.imgur.com/50jJYUs.png)
9. Click Add Outgoing Webhook
![](http://i.imgur.com/6G9Lsve.png)
10. Click Save Integration
11. Try it out in Slack!

![](http://i.imgur.com/snMdCT4.png)