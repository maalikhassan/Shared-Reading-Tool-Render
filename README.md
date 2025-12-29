# 📖 Shared Reading Tool

A real-time collaborative PDF reading application that enables multiple users to read and discuss PDFs together with synchronized page navigation, shared notes, and live chat.

## ✨ Features

- **📄 PDF Viewing**: Upload and view PDF documents with smooth page navigation
- **🔄 Real-time Synchronization**: Page changes and cursor movements are synchronized across all connected users
- **💬 Live Chat**: Built-in chat functionality to discuss content with other readers
- **📝 Shared Notes**: Collaborative note-taking area that syncs across all users
- **🎯 Ready State System**: Signal when you're ready to turn the page for coordinated group reading
- **🔍 Zoom Controls**: Zoom in/out functionality with keyboard shortcuts (Ctrl/Cmd + +/-)
- **📱 Responsive Design**: Fully responsive layout that works on desktop, tablet, and mobile devices
- **👁️ Cursor Tracking**: See where other users are pointing on the PDF in real-time

## 🛠️ Technology Stack

- **Backend**:
  - Node.js
  - Express.js (Web server)
  - WebSocket (ws) (Real-time communication)

- **Frontend**:
  - Vanilla JavaScript
  - PDF.js (PDF rendering)
  - WebSocket API (Client-side real-time communication)
  - HTML5 & CSS3

## 🚀 Installation

### Prerequisites

- Node.js (v12 or higher)
- npm (comes with Node.js)

### Setup

1. Clone the repository:
```bash
git clone https://github.com/maalikhassan/app.git
cd app
```

2. Install dependencies:
```bash
npm install
```

3. Start the server:
```bash
npm start
```

4. Open your browser and navigate to:
```
http://localhost:8080
```

## 📖 Usage

### Basic Usage

1. **Upload a PDF**: Click on the file input to select a PDF from your computer
2. **Navigate Pages**: Use the "Previous" and "Next" buttons or arrow keys to navigate through the PDF
3. **Zoom**: Use the zoom buttons or keyboard shortcuts (Ctrl/Cmd + +/-) to adjust the PDF size
4. **Ready to Turn**: Click the "Ready to Turn Page" button to signal you're ready for the next page
5. **Chat**: Use the chat box at the bottom right to communicate with other users
6. **Take Notes**: Add notes in the "Shared Notes" section which will be visible to all users

### Collaborative Features

- **Real-time Sync**: All page changes are synchronized across connected users
- **Cursor Sharing**: See where other users are pointing on the PDF
- **Chat Notifications**: Get notified when other users send messages
- **Device Info**: Each user is identified by a unique device ID

## 📁 Project Structure

```
app/
├── public/                 # Frontend files
│   ├── index.html         # Main HTML file with UI structure and styles
│   ├── app.js             # Client-side JavaScript for PDF viewing and WebSocket
│   ├── pdf.mjs            # PDF.js module
│   └── pdf.worker.mjs     # PDF.js web worker
├── server.js              # Express server and WebSocket setup
├── package.json           # Project dependencies and scripts
├── .env                   # Environment variables (not tracked)
└── README.md             # This file
```

## 🔧 Configuration

The server runs on port 8080 by default. You can change this by setting the `PORT` environment variable:

```bash
PORT=3000 npm start
```

Or create a `.env` file:
```
PORT=3000
```

## 🌐 Deployment

This application can be deployed to various platforms:

- **Glitch**: Already configured for Glitch hosting (see `.glitchdotcom.json`)
- **Heroku**: Deploy using the included `package.json` configuration
- **DigitalOcean**: Deploy on App Platform or Droplets
- **Any Node.js hosting service** that supports WebSocket connections

## 🎯 Use Cases

- **Remote Study Groups**: Students can read and discuss academic papers together
- **Book Clubs**: Read and discuss books remotely with synchronized page turns
- **Document Review**: Teams can review documents together in real-time
- **Presentations**: Present PDFs to a remote audience with synchronized viewing
- **Training Sessions**: Conduct training with synchronized material viewing

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the ISC License.

## 👤 Author

Created by the maalikhassan team

## 🐛 Known Issues

- PDF files must be loaded locally by each user (not shared via the server)
- Large PDFs may take time to render on slower devices

## 🔮 Future Enhancements

- Server-side PDF hosting for automatic distribution
- User authentication and persistent sessions
- Annotation and highlighting tools
- Screen share capability
- Recording and playback of reading sessions
