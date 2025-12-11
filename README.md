# GaliBot UI

Frontend interface for GaliBot - Statistics Assistant for Students.

## Features

- **Streaming Responses**: Real-time token-by-token responses using Server-Sent Events (SSE)
- **MathJax Integration**: Beautiful LaTeX formula rendering
- **RAG Support**: Displays sources from the RAG database
- **Modern UI**: Clean and user-friendly chat interface

## Setup

1. Clone the repository:
```bash
git clone https://github.com/shayuk/galibot-ui.git
cd galibot-ui
```

2. Deploy to Firebase Hosting (or any static hosting):
```bash
firebase deploy
```

Or simply upload the `public/` folder to your hosting service.

## Configuration

Update the API URL in `public/index.html`:
```javascript
const API_URL = "https://lecturers-gpt-server.onrender.com/api/ask/stream";
```

## Structure

```
galibot-ui/
├── public/
│   ├── index.html      # Main chat interface
│   ├── dashboard.html  # Dashboard (if exists)
│   └── upload.html     # Upload interface (if exists)
├── firebase.json       # Firebase Hosting configuration
└── README.md
```

## Features Details

### Streaming API
The UI connects to `/api/ask/stream` endpoint and displays responses token-by-token in real-time.

### MathJax Support
LaTeX formulas are automatically detected and rendered beautifully using MathJax 3.x.

### Loading Indicators
Animated loading spinner shows during RAG queries and response generation.

## Deployment

### Firebase Hosting
```bash
firebase deploy --only hosting
```

### Other Hosting Services
Simply upload the `public/` folder to your hosting service (Netlify, Vercel, etc.).

## License

MIT

