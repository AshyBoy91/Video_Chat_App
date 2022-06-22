# Video Chat App Using Agora SDK

App is made made with Django - Python using Agora SDK. Live project is [here] (https://videochatapp91.herokuapp.com/). You may have to refresh the page as sometime heroku takes time to run the project

With this app, you can:

- Join / leave channel
- Mute / unmute audio
- Enable / disable video

If you share the 'room name' you can invite other users to join the same channel

Agora Video SDK details can be found here
```
https://console.agora.io/
```

### 1 Running the App
First, clone the repo
```
https://github.com/AshyBoy91/Video_Chat_App.git
```
### 2 - Install requirements
```
cd <to dir>
pip install -r requirements.txt
```

### 3 - Update Agora credentals
In order to use this project you will need to replace the Agora credentials in `views.py` and `streams.js`.

Create an account at agora.io and create an `app`. Once you create your app, you will want to copy the `appid` & `appCertificate` to update `views.py` and `streams.js`.

#### views.py
```
def getToken(request):
    appId = "YOUR APP ID"
    appCertificate = "YOUR APPS CERTIFICATE"
    ......
```

#### streams.js
```
....
const APP_ID = 'YOUR APP ID'
....
```


#### 4 - Start server
```
python manage.py runserver
```


## License
The MIT License (MIT).


