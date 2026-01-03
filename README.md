# 🏢 RealtyLingo

**Your AI Co-Founder for Startup Success**

RealtyLingo is an intelligent platform that empowers solo entrepreneurs and early-stage founders with AI-driven business strategy, validation, and fundraising support. Built with cutting-edge technology, it serves as your virtual co-founder, providing actionable insights and automation to accelerate your startup journey.

---

## ✨ Features

### 🤖 AI-Powered Business Assistant
- **Intelligent Chat Interface**: Get instant answers to your business questions powered by Google's Gemini AI
- **24/7 Availability**: Access expert-level business advice anytime, anywhere

### 💡 Idea Validation
- **Market Feasibility Analysis**: Validate your business ideas with comprehensive market research
- **Competition Assessment**: Understand your competitive landscape
- **Demand Forecasting**: Get insights on potential market demand

### 📊 Pitch Deck Support
- **Auto-Generation**: Create compelling pitch decks tailored to your business
- **Expert Review**: Receive detailed feedback and recommendations
- **Structured Approach**: Covers problem statement, solution, market opportunity, business model, and financials

### 💰 Investor Matching
- **Smart Recommendations**: Get matched with investors based on your pitch
- **Industry Focus Analysis**: Understand which investors align with your sector
- **Investment Stage Matching**: Find investors suited to your startup stage

### 📈 Strategic Growth
- **Growth Hacking Strategies**: Actionable insights for rapid growth
- **Scaling Plans**: Detailed roadmaps for business expansion
- **Workflow Optimization**: Automation recommendations to enhance efficiency

---

## 🛠️ Tech Stack

### Backend
- **FastAPI**: High-performance Python web framework
- **Google Gemini AI**: Advanced AI model for business intelligence
- **Supabase**: Authentication and database management
- **Firecrawl**: Web scraping and data extraction
- **FAISS**: Vector similarity search for intelligent matching
- **Uvicorn**: ASGI server for production deployment

### Frontend
- **React**: Modern UI library
- **Vite**: Next-generation frontend tooling
- **ESLint**: Code quality and consistency
- **Responsive Design**: Mobile-first approach

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Node.js 16+
- npm or yarn
- Google API Key (for Gemini)
- Supabase Account
- Firecrawl API Key

### Backend Setup

1. **Navigate to the Backend directory**
   ```bash
   cd Backend
   ```

2. **Install Python dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure environment variables**
   
   Create a `.env` file in the Backend directory:
   ```env
   GEMINI_KEY=your_gemini_api_key
   SUPABASE_URL=your_supabase_url
   SUPABASE_ANON_KEY=your_supabase_anon_key
   FIRECRAWL_KEY=your_firecrawl_api_key
   ```

4. **Run the backend server**
   ```bash
   python backend.py
   ```
   
   The API will be available at `http://localhost:8000`

### Frontend Setup

1. **Navigate to the Frontend directory**
   ```bash
   cd Frontend
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```
   
   The application will be available at `http://localhost:5173`

---

## 📖 API Documentation

Once the backend is running, visit `http://localhost:8000/docs` for interactive API documentation powered by FastAPI's built-in Swagger UI.

### Key Endpoints

- `GET /status/` - Health check
- `POST /ai/` - General AI chat queries
- `POST /login/` - User authentication
- `POST /validate_idea/` - Business idea validation
- `POST /pitch/generate/` - Generate pitch deck
- `POST /pitch/review/` - Review existing pitch
- `POST /match_investors/` - Get investor recommendations
- `POST /strategic_advice/` - Receive strategic guidance
- `POST /scaling/` - Get scaling strategies

---

## 🎯 Usage Examples

### Validate a Business Idea
```javascript
const response = await fetch('http://localhost:8000/validate_idea/', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify({
    idea: 'A SaaS platform for managing remote teams'
  })
});
```

### Generate a Pitch Deck
```javascript
const response = await fetch('http://localhost:8000/pitch/generate/', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify({
    business_info: 'Your business description here'
  })
});
```

---

## 🏗️ Project Structure

```
RealtyLingo/
├── Backend/
│   ├── backend.py          # Main FastAPI application
│   ├── requirements.txt    # Python dependencies
│   └── README.md          # Backend documentation
├── Frontend/
│   ├── src/
│   │   ├── components/    # React components
│   │   ├── pages/        # Application pages
│   │   └── styles/       # CSS stylesheets
│   ├── package.json      # Frontend dependencies
│   └── README.md         # Frontend documentation
├── LICENSE               # Project license
└── README.md            # This file
```

---

## 🔒 Security

- All API endpoints use CORS protection
- User authentication handled via Supabase
- Google OAuth integration for secure login
- Environment variables for sensitive data
- Input validation on all endpoints

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the terms specified in the [LICENSE](LICENSE) file.

---

## 🙏 Acknowledgments

- **Google Gemini AI** for powering the intelligent assistant
- **Supabase** for authentication and database services
- **FastAPI** for the robust backend framework
- **React** for the dynamic frontend experience

---

## 📧 Contact & Support

For questions, feedback, or support, please open an issue in the repository.

---

**Built with ❤️ for entrepreneurs worldwide**
