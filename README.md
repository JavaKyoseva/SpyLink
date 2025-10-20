# 🕵️‍♂️ SpyLink — Demo Link Generator 🌐

**Description**  
SpyLink is a demo tool that generates unique links which, upon user consent, request browser permissions such as camera and location. The collected data is stored securely on the site for educational, testing, or authorized research purposes.  

---

## ⚙️ What It Does

- Generates unique session links for demonstrations or controlled environments.  
- Requests camera and location access only after explicit user consent.  
- Saves approved data directly to the server for review and analysis.  

---

## 🚀 Quick Installation & Run
```bash
#Install dependencies
pkg install github -y
pkg install nodejs -y
pkg install unzip -y
# Clone repository
git clone https://github.com/JavaKyoseva/SpyLink
#Unzip zip file
cd SpyLink
unzip main.zip
```
## 🔥 Firebase Setup

1. Go to [Firebase Console](https://console.firebase.google.com) and create a new project (e.g., "SpyLink").  
2. Add a web app to your project and copy the generated `firebaseConfig`.  
3. HTML/JS, include Firebase SDK:

```html
<script src="https://www.gstatic.com/firebasejs/11.0.0/firebase-app.js"></script>
<script src="https://www.gstatic.com/firebasejs/11.0.0/firebase-database.js"></script>
```
4. Initialize Firebase in your JS:

```javascript
const app = firebase.initializeApp(firebaseConfig);
const db = firebase.database();
```

5. Secure your database via Firebase Rules to allow only authorized writes and reads.

```bash
# start localhost
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
