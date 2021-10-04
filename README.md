# Connect-Intellect
<h3>Description:</h3> A Full Stack Realtime Chat Application with features including Direct and Group Chats, emojis & Reactions, Built-in Gif support, the ability to edit & delete messages, specialized commands, Authentication &amp; SMS Notifications.

<h3>Tech Stack used: </h3>

* HTML
* CSS
* Javascript
* React js
* Node js
* getStream
* twilio

<h3>Installation: </h3>

Open a terminal window at the location where you want to install the project and type in the following commands: 

```
git clone https://github.com/secrashi/Connect-Intellect.git
cd connect-intellect\client
npm i
npm start
```
These commands will start the frontend development server. Now to run the backend server, open another terminal window at project folder location and type the following commands:
```
cd server
npm i
```

Now before you start the backend development server, you have to complete the following steps: 

- If you checked the `.gitignore` file in the outer most folder, you must have noticed that a `.env` file is mentioned there. It is hidden because it contains sensitive information (api keys, secrets etc.) of getstream.io and twilio accounts.
- So go into your server folder and create a new file named `.env`.
- Now go to https://getstream.io/ and after signing in, create a new app with any name. I named mine Sakshi_Dhamija. Search for app key and api secret in app overview. 
- Copy them and paste them in your `.env` file as follows:
```
STREAM_APP_ID = 1145181
STREAM_API_KEY = <your api key>
STREAM_API_SECRET = <your api secret>
```
- The `STREAM_APP_ID ` mentioned above is of the application created by me.
- Now go to https://www.twilio.com/ and sign up in your twilio account. 
- Set up your account in 3 steps on the website. (You can use any phone number they provide you in those steps, though login with your own mobile number. Also, choose code in next step and choose language javascript)
- In your dasboard, click the develop section in your sidebar. 
- go to messaging > try it out > get set up.
- After setting up go to send an sms in try it out section, click on messaging service id, and it will show an id in the dropdown menu, click on it. 
- Now copy your account sid, auth token and messaging service sid from the code snippet present in the right side. ( Check figure below to see which ones ) and paste them in your `.env` file as follows: 

![WhatsApp Image 2021-10-02 at 6 20 24 PM](https://user-images.githubusercontent.com/56053777/135716969-e68d4760-a348-4bef-9b48-f43ef2cd0847.jpeg)


```
TWILIO_ACCOUNT_SID = <your accountSid>
TWILIO_AUTH_TOKEN = <your auth token>
TWILIO_MESSAGING_SERVICE_SID = <your messaging service sid>
```
- Now some times on clicking to check the auth token it shows redated. In that case go to general setting of your account and copy the auth token from there. (if you have just one auth token displayed choose that, otherwise choose the auth token from live Credentials category.)
- Save your `.env` file and start your development server using `npm start`
