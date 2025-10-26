# 🤖 Yuktra AI Chatbot  
Website is live here -> https://yuktra-ai.vercel.app/ 

An intelligent conversational AI chatbot powered by Google's Gemini API, built with Next.js and React.

![Next.js](https://img.shields.io/badge/Next.js-14-black?style=flat-square&logo=next.js)
![React](https://img.shields.io/badge/React-18-blue?style=flat-square&logo=react)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.0-38B2AC?style=flat-square&logo=tailwind-css)
![Gemini API](https://img.shields.io/badge/Gemini-API-4285F4?style=flat-square&logo=google)

## ✨ Features

- 💬 **Real-time AI Conversations** - Instant responses powered by Google Gemini 2.0
- 🎨 **Modern UI/UX** - Clean, gradient-based design with smooth animations
- 🔒 **Secure API Integration** - Backend API routes protect your API keys
- 📱 **Responsive Design** - Works seamlessly on desktop, tablet, and mobile
- ⚡ **Fast Performance** - Built with Next.js App Router for optimal speed
- 🗑️ **Chat Management** - Clear chat history with one click
- 💡 **Quick Prompts** - Suggested questions to get started
- ⌨️ **Keyboard Shortcuts** - Press Enter to send messages

## 🛠️ Tech Stack

- **Framework**: Next.js 14 (App Router)
- **Frontend**: React 18 with Hooks
- **Styling**: Tailwind CSS
- **AI Model**: Google Gemini 2.0 Flash
- **API**: RESTful API with Next.js Route Handlers
- **Language**: JavaScript (ES6+)

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v18.0 or higher)
- npm or yarn
- A Google account for Gemini API access

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/yuktra.git
cd yuktra
```

### 2. Install dependencies

```bash
npm install
```

### 3. Get your Gemini API Key

1. Visit [Google AI Studio](https://aistudio.google.com/app/apikey)
2. Sign in with your Google account
3. Click "Create API Key"
4. Copy your API key

### 4. Set up environment variables

Create a `.env.local` file in the root directory:

```env
GEMINI_API_KEY=your_api_key_here
```

⚠️ **Important**: Never commit your `.env.local` file to version control!

### 5. Run the development server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see Yuktra in action!

## 📁 Project Structure

```
yuktra/
├── app/
│   ├── api/
│   │   └── chat/
│   │       └── route.js          # Backend API endpoint
│   ├── page.js                    # Main chatbot UI
│   ├── layout.js                  # Root layout
│   └── globals.css                # Global styles
├── public/                        # Static assets
├── .env.local                     # Environment variables (not in repo)
├── next.config.js                 # Next.js configuration
├── tailwind.config.js             # Tailwind CSS configuration
├── package.json                   # Dependencies
└── README.md                      # Project documentation
```

## 🎯 Key Components

### Frontend (`app/page.js`)
- Manages chat state and user interactions
- Handles message sending and receiving
- Renders chat interface with messages
- Implements loading states and error handling

### Backend API (`app/api/chat/route.js`)
- Securely stores and uses Gemini API key
- Processes incoming messages
- Communicates with Gemini API
- Returns AI-generated responses
- Handles errors gracefully

## 🔧 Configuration

### Changing the AI Model

Edit `app/api/chat/route.js` to use a different Gemini model:

```javascript
// Current model
gemini-2.0-flash

// Other available models
gemini-1.5-pro
gemini-1.5-flash
```

### Customizing the UI

Colors and styling can be modified in:
- `app/page.js` - Tailwind classes
- `tailwind.config.js` - Theme configuration
- `app/globals.css` - Global CSS variables







## 📈 Future Enhancements

- [ ] Chat history persistence with database
- [ ] User authentication and profiles
- [ ] Multiple chat sessions
- [ ] Markdown rendering for bot responses
- [ ] Code syntax highlighting
- [ ] Image upload support (Gemini Vision)
- [ ] Voice input/output
- [ ] Dark mode toggle
- [ ] Export chat functionality
- [ ] Rate limiting for API calls

