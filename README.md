# Connect-Intellect
## Description
A Full Stack Realtime Chat Application with features including Direct and Group Chats, emojis & Reactions, Built-in Gif support, the ability to edit & delete messages, specialized commands, Authentication &amp; SMS Notifications.

## Tech Stack used

* HTML
* CSS
* Javascript
* React js
* Node js
* getStream
* twilio

## Local Setup: 

Clone the repository, cd into them individually, install the packages using `npm install` and then follow the below mentioned steps for setting up client and server.

## 1. Client
- Create a .env file same as the given env file (.env.example).
```
REACT_APP_BACKEND_LOCAL = <development_localhost> || http://localhost:5000/
REACT_APP_BACKEND = <deployed_app_backend> || https://connect-intellect.netlify.app/
REACT_APP_STREAM_API_KEY = <STREAM_API_KEY>
```

## 2. Server
-  Create a .env file same as the given env file (.env.example).
```
STREAM_APP_ID = <stream_app_id>
STREAM_API_KEY = <stream_api_key>
STREAM_API_SECRET = <stream_api_secret>

TWILIO_ACCOUNT_SID = <twilio_account_sid>
TWILIO_AUTH_TOKEN = <twilio_account_token>
TWILIO_MESSAGING_SERVICE_SID = <twilio_messaging_service_sid>

NODE_ENV = <development || production>
FRONTEND_DEVELOPMENT = <http://localhost:3000>
FRONTEND_PRODUCTION = <frontend_production_web_app>
```
- You can get your `stream api key ` from [here](https://getstream.io/)
- To get `Twilio api and secret keys`
 > Go to https://www.twilio.com/ and sign up in your twilio account. 
 > Set up your account in 3 steps on the website. (You can use any phone number they provide you in those steps, though login with your own mobile number. Also, choose code in next step and choose language javascript)
 > In your dasboard, click the develop section in your sidebar. 
 > Go to messaging > try it out > get set up.
 > After setting up go to send an sms in try it out section, click on messaging service id, and it will show an id in the dropdown menu, click on it. 
 > Now copy your account sid, auth token and messaging service sid from the code snippet present in the right side.

![WhatsApp Image 2021-10-02 at 6 20 24 PM](https://user-images.githubusercontent.com/56053777/135716969-e68d4760-a348-4bef-9b48-f43ef2cd0847.jpeg)

> Now some times on clicking to check the auth token it shows redated. In that case go to general setting of your account and copy the auth token from there. (if you have just one auth token displayed choose that, otherwise choose the auth token from live Credentials category.)
> Save your `.env` file and start your development server using `npm start`

## Run it
Run in development mode

Runs the application is development mode. Should not be used in production
- Clinet
```
cd client
npm start
```
- Server
```
cd server
npm run dev
```
