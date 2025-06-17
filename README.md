# 📰 NewsBreeze - AI-Powered News Reader

NewsBreeze is a modern news aggregation app that brings you the latest headlines with AI-powered summaries and text-to-speech capabilities.

## ✨ Features

- 📰 Latest news headlines from NewsAPI
- 🤖 AI-powered article summaries
- 🔊 Text-to-speech for audio reading
- 🎨 Modern, responsive UI
- 🔄 Real-time news updates

## 🛠️ Tech Stack

### Frontend
- React with TypeScript
- Vite for build tooling
- Modern CSS with animations

### Backend
- Node.js with Express
- NewsAPI integration
- Hugging Face AI integration
- Axios for HTTP requests

## 🚀 Quick Start

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- API keys for:
  - [NewsAPI](https://newsapi.org/)
  - [Hugging Face](https://huggingface.co/)

### Setup Steps

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd NewsBreeze
   ```

2. **Backend Setup**
   ```bash
   cd backend
   npm install
   ```

   Create `.env` file in backend directory:
   ```env
   NEWS_API_KEY=your_newsapi_key_here
   HUGGINGFACE_API_KEY=your_huggingface_api_key_here
   PORT=5000
   ```

3. **Frontend Setup**
   ```bash
   cd ../frontend
   npm install
   ```

4. **Start the Application**

   Start backend server:
   ```bash
   cd backend
   npm run dev
   ```

   In a new terminal, start frontend:
   ```bash
   cd frontend
   npm run dev
   ```

   Access the application:
   - Frontend: http://localhost:5173
   - Backend API: http://localhost:5000

## 📡 API Endpoints

### GET /api/news
Fetches latest news with AI summaries
```json
{
  "articles": [
    {
      "id": "unique_id",
      "title": "Article Title",
      "description": "Article description",
      "summary": "AI-generated summary",
      "url": "article_url",
      "urlToImage": "image_url",
      "publishedAt": "2024-01-01T00:00:00Z"
    }
  ]
}
```

### POST /api/audio
Generates audio from text
```json
{
  "text": "Text to convert to speech"
}
```

## 🎯 How to Use

1. **View News**: Latest headlines load automatically
2. **Read Summaries**: Each article shows AI-generated summary
3. **Listen**: Click "🎵 Listen" for audio playback
4. **Refresh**: Use "🔄 Refresh News" for latest updates
5. **Read Full**: Click article titles for complete stories

## 🔧 Configuration

### Environment Variables
- `NEWS_API_KEY`: NewsAPI key
- `HUGGINGFACE_API_KEY`: Hugging Face API key
- `PORT`: Backend port (default: 5000)

## 🚨 Troubleshooting

### Common Issues
1. **CORS Errors**: Ensure backend runs on port 5000
2. **API Key Issues**: Verify API keys and permissions
3. **Audio Playback**: Check browser audio permissions
4. **Slow Loading**: Initial model loading may take time

### Error Messages
- "Failed to fetch news": Check NewsAPI key and connection
- "Audio generation failed": Verify Hugging Face API key
- "Server connection failed": Ensure backend is running

## 📝 License
MIT License

## 🤝 Contributing
1. Fork the repository
2. Create feature branch
3. Make changes
4. Test thoroughly
5. Submit pull request

## 📞 Support
Open an issue on GitHub for questions or problems.

---

**Built with ❤️ for the AI-powered news experience**
