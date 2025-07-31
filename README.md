# Ori-Sage
Emotionally grounded AI persona interface and behavior engine
# Ori Sage - Emotionally Grounded AI Guidance

A compassionate AI support application built with Flask that provides empathetic, personalized responses based on emotional state analysis. Features the official trademarked Ori Sage AI persona.

## Features

- **Emotional Intelligence**: Advanced sentiment analysis and emotional tone detection
- **Trademarked AI Persona**: Official Ori Sage identity with authentic voice and behavioral alignment
- **Personality Profiles**: 5 pre-defined personalities plus custom personality creation
- **Database Integration**: PostgreSQL storage for conversations, users, and analytics
- **Calming UI**: Sage green design system optimized for mental wellness
- **Real-time Chat**: Responsive conversation interface with message history
- **Help System**: In-app help panel with guidance information

## Technology Stack

### Backend
- **Flask** - Python web framework
- **PostgreSQL** - Database with full persistence
- **TextBlob** - Sentiment analysis and NLP
- **SQLAlchemy** - Database ORM
- **Gunicorn** - WSGI server

### Frontend
- **Bootstrap 5** - Responsive CSS framework
- **Vanilla JavaScript** - Client-side interactions
- **Feather Icons** - Icon library
- **Custom CSS** - Ori Sage design system

## Installation

1. Clone the repository:
```bash
git clone https://github.com/bernibot/ori-sage.git
cd ori-sage
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
```bash
export DATABASE_URL="your_postgresql_connection_string"
export SESSION_SECRET="your_secret_key"
```

4. Run the application:
```bash
gunicorn --bind 0.0.0.0:5000 main:app
```

## Project Structure

```
ori-sage/
├── static/
│   ├── css/
│   │   └── style.css          # Ori Sage design system
│   └── js/
│       └── main.js            # Client-side functionality
├── templates/
│   ├── base.html              # Base template
│   ├── index.html             # Main conversation interface
│   └── personality.html       # Personality settings
├── app.py                     # Flask application setup
├── main.py                    # Application entry point
├── models.py                  # Database models
├── routes.py                  # Application routes
├── database_service.py        # Database operations
├── personality_api.py         # Personality management
├── sentiment_analyzer.py      # Emotion analysis
├── ori_identity_system.py     # Official Ori persona
├── ori_identity.json          # Persona specification
├── ori_responses.json         # Response database
└── requirements.txt           # Python dependencies
```

## Key Components

### Ori Identity System
The application features the official trademarked Ori Sage AI persona with:
- Authentic voice and tone guidelines
- Signature responses and grounding techniques
- Behavioral alignment for emotional safety
- Contextual response generation

### Emotional Intelligence
- Real-time sentiment analysis using TextBlob
- Emotional tone detection (anxiety, sadness, joy, etc.)
- Contextual response matching
- Grounding elements for high-stress emotions

### Personality Profiles
- **Compassionate Sage**: Warm, deeply empathetic
- **Mindful Guide**: Present-moment awareness
- **Gentle Counselor**: Professional therapeutic approach
- **Caring Friend**: Casual, supportive companion
- **Wise Elder**: Philosophical, experienced perspective
- **Custom Profiles**: User-created personalities

### Database Schema
- **Users**: Session-based user tracking
- **Conversations**: Persistent conversation management
- **Messages**: Complete message history with metadata
- **PersonalityProfiles**: Custom personality storage
- **AnalyticsEvents**: User interaction tracking
- **ResponseFeedback**: Response quality metrics

## API Endpoints

### Core Application
- `GET /` - Main conversation interface
- `POST /send_message` - Process user messages
- `POST /clear_conversation` - Clear conversation history

### Personality API
- `GET /api/personality/profiles` - List all profiles
- `GET /api/personality/current` - Get current profile
- `POST /api/personality/set/<name>` - Set active profile
- `POST /api/personality/custom` - Create custom profile

### Ori Identity API
- `GET /api/ori/identity` - Get Ori's identity info
- `GET /api/ori/signature` - Get signature response
- `GET /api/ori/grounding` - Get grounding response
- `GET /api/ori/tone_guidelines` - Get tone guidelines

## Configuration

### Environment Variables
- `DATABASE_URL` - PostgreSQL connection string
- `SESSION_SECRET` - Flask session secret key
- `FLASK_ENV` - Application environment (development/production)

### Database Setup
The application automatically creates all required tables on startup. For production deployment, ensure PostgreSQL is properly configured.

## Deployment

### Replit Deployment
The application is optimized for Replit deployment with:
- Automatic dependency management
- Environment variable configuration
- PostgreSQL integration
- Gunicorn WSGI server

### Manual Deployment
1. Set up PostgreSQL database
2. Configure environment variables
3. Install dependencies
4. Run database migrations
5. Start with Gunicorn

## Development

### Local Development
1. Install dependencies: `pip install -r requirements.txt`
2. Set up local PostgreSQL
3. Configure environment variables
4. Run: `python main.py`

### Adding New Features
- Models: Add to `models.py`
- Routes: Add to `routes.py`
- Database operations: Use `database_service.py`
- Frontend: Update templates and `main.js`

## License

This project contains the trademarked Ori Sage AI persona. The persona specification and identity are proprietary. The underlying application framework is available for educational and development purposes.

## Support

For issues and questions:
1. Check the in-app help panel
2. Review the personality settings
3. Verify database connection
4. Check application logs

---

**Ori Sage** - Emotionally grounded guidance with clarity and calm.
