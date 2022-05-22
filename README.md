# News Bot: A Slack Plugin

News Bot is a Slack app that automatically sends a Slack message containing links to the top news headlines for the day according to CNN. The message is sent out every morning at 9 am to the workspace's General channel. This is achieved by setting up a [Cron Job](https://www.npmjs.com/package/cron) that ensures data is fetched from CNN's API, parsed accordingly, and sent to Slack every 24 hours. 

![image](https://i.ibb.co/B45RmPx/Screen-Shot-2018-12-01-at-8-10-02-PM.png)


## Built With

- Node.js 
- Slack API 

## Folder Structure

_Folder Structure:_

    ├── controllers                                 
            ├── message_controller                 # Parses API response and creates message object
    ├── services                                     
            ├── request_controller                 # Fetches data from CNN API
    ├── app.js                                     # App entry point       
    ├── main.js                                    # Main function call
    ├── package.json
    └── README.md

## Deployment 
The application is hosted on Heroku. There is no front-end portion to this application, however this ensures the Cron Job is running and the application will fetch and send data periodically. 

## Authors 

_Saurav Saha, Ahmed Abdelmoneim, Seif Ghazi_

### 📤 Deploy
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/chathush999/SlackNewsBot)

