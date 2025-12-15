# Social Media Content Scheduler 📅

Multi-platform social media scheduling tool with AI-powered content suggestions, hashtag recommendations, and comprehensive analytics.

## 🌟 Features

- **Multi-Platform Support** - Schedule posts for Twitter, LinkedIn, Instagram, Facebook
- **AI Content Suggestions** - Get AI-generated content ideas and captions
- **Smart Hashtag Recommendations** - AI suggests trending and relevant hashtags
- **Post Scheduling** - Schedule posts for optimal engagement times
- **Media Library** - Manage images, videos, and documents
- **Analytics Dashboard** - Track post performance and engagement
- **Calendar View** - Visual content calendar
- **Bulk Scheduling** - Schedule multiple posts at once

## 🛠️ Tech Stack

**Frontend:**
- React.js
- FullCalendar
- Material-UI
- Axios

**Backend:**
- Python Django
- Django REST Framework
- Celery (Task Queue)
- Redis (Message Broker)

**AI/ML:**
- OpenAI GPT (Content generation)
- NLP for hashtag analysis
- Sentiment analysis

**Database:**
- PostgreSQL

## 📋 Prerequisites

- Python 3.8+
- Node.js 14+
- PostgreSQL
- Redis
- npm/yarn

## 🚀 Installation

### Backend Setup

```bash
cd backend
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

### Celery Worker

```bash
celery -A scheduler worker -l info
```

### Frontend Setup

```bash
cd frontend
npm install
npm start
```

## 📁 Project Structure

```
social-media-content-scheduler/
├── backend/
│   ├── scheduler/
│   │   ├── models.py
│   │   ├── views.py
│   │   ├── serializers.py
│   │   ├── tasks.py
│   │   └── ai_helper.py
│   ├── manage.py
│   └── requirements.txt
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   └── App.js
│   └── package.json
└── README.md
```

## 🎯 Key Features

### 1. AI Content Generation
Generate engaging captions and content ideas using AI.

### 2. Smart Scheduling
AI suggests best times to post based on audience engagement patterns.

### 3. Hashtag Intelligence
Analyzes trending hashtags and suggests relevant ones for your content.

## 📊 API Endpoints

- `POST /api/posts/create` - Create scheduled post
- `GET /api/posts/` - Get all scheduled posts
- `PUT /api/posts/{id}` - Update post
- `DELETE /api/posts/{id}` - Delete post
- `POST /api/ai/generate-content` - Generate AI content
- `POST /api/ai/suggest-hashtags` - Get hashtag suggestions
- `GET /api/analytics/` - Get analytics data

## 👨‍💻 Author

**Keshav Jadam**
- GitHub: [@Keshavja29](https://github.com/Keshavja29)
- LinkedIn: [Keshav Jadam](https://linkedin.com/in/keshav-jadam)
