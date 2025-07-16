# 🎥 Real-Time Video Chat App

A fully functional peer-to-peer video calling web application built using **React.js**, **Express.js**, **WebRTC**, and **Socket.io**. Users can join a room via email and room ID, initiate a video call, and communicate in real time with high performance and low latency.

---

## 🚀 Features

* ✉️ Email & Room-based Join System
* 📹 Live One-to-One Video Calling
* ✨ Real-time Peer-to-Peer Media Streaming via WebRTC
* ⚡ Socket.io-based signaling and connection negotiation
* ⚖️ Dynamic offer/answer SDP handling
* 🔌 STUN server support for NAT traversal

---

## 📁 Project Structure

```bash
client/
🔺 components/
  🔺 LobbyScreen.jsx        # Email & Room form
  🔺 RoomPage.jsx          # Video call screen
  🔺 context/SocketProvider.jsx
  🔺 service/peer.js       # Peer connection logic

dependencies: react, react-player, socket.io-client

server/
🔺 index.js               # Express + Socket.io signaling server

dependencies: express, socket.io
```

---

## 🔧 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/UsamaSani/video-Webchat.git
cd video-Webchat
```

### 2. Install Server Dependencies

```bash
cd server
npm install
node index.js
```

### 3. Install Client Dependencies

```bash
cd ../client
npm install
npm start
```

---

## 🛠️ How It Works

1. **User enters email & room ID** in the Lobby form
2. **Socket.io connects** user to the backend and joins the room
3. **WebRTC creates an offer/answer SDP** between peers
4. **Socket.io handles negotiation and ICE candidate exchange**
5. **WebRTC streams audio/video directly between clients** (P2P)

---

## 🤖 Technologies Used

| Technology   | Purpose                                   |
| ------------ | ----------------------------------------- |
| React.js     | Frontend UI framework                     |
| Express.js   | Backend server                            |
| Socket.io    | Real-time signaling between clients       |
| WebRTC       | Direct peer-to-peer audio/video streaming |
| React Player | Video rendering for local/remote streams  |

---

## 👾 STUN Server

This app uses public STUN servers to enable NAT traversal and direct P2P connectivity:

```json
stun:stun.l.google.com:19302
stun:global.stun.twilio.com:3478
```

---

## 🌍 Live Demo

Coming Soon... ✨

---

## 🔧 Improvements You Can Add

* 📱 Mobile responsive UI
* 💡 Screen sharing support
* ♻️ Multi-user conferencing
* ⛓ Better authentication / user profiles

---

## 👨‍💻 Author

**Usama Sani Khanzada**
[👨‍💼 GitHub](https://github.com/UsamaSani) • [💼 LinkedIn](https://www.linkedin.com/in/usama-sani-khanzada-5b6552240/) • [📄 Portfolio](https://usamasani.tech)

---

## 📝 License

MIT License — Free to use, modify, and distribute.

> 💡 Pull requests are welcome! If you have ideas or improvements, contribute and make it better together. ✨
