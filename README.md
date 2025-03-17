# Real Estate Price Predictor

A machine learning-powered web application that predicts real estate prices based on property features and market data. Built with Flask, SQLAlchemy, and scikit-learn.

## Features

- Property price prediction using machine learning
- User authentication system
- Interactive data visualizations
- Mortgage calculator
- Save and manage predictions
- Mobile-responsive design

## Tech Stack

- Backend: Python, Flask
- Database: SQLAlchemy (SQLite in development, PostgreSQL in production)
- ML: scikit-learn, pandas, numpy
- Frontend: HTML, CSS, JavaScript, Bootstrap
- Visualization: Chart.js

## Getting Started

1. Clone the repository:
```bash
git clone <your-repo-url>
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
Required environment variables:
- SESSION_SECRET: Secret key for Flask sessions
- DATABASE_URL: Database connection URL (optional, defaults to SQLite)

4. Run the application:
```bash
python main.py
```
The application will be available at `http://localhost:5000`

## Project Structure

- `app.py`: Main Flask application setup and routes
- `model.py`: Machine learning model training and prediction logic
- `models.py`: Database models (User, SavedPrediction)
- `data/`: Housing dataset and data processing
- `templates/`: HTML templates
- `static/`: CSS, JavaScript, and other static assets

## Features in Detail

### Price Prediction
- Input property features (square footage, bedrooms, location, etc.)
- Get instant price predictions with confidence intervals
- View feature importance analysis
- Interactive data visualizations

### User System
- User registration and authentication
- Password reset functionality
- Save and manage predictions
- User dashboard

### Mortgage Calculator
- Calculate monthly payments
- Factor in down payment, interest rates, and terms
- Include property tax and insurance estimates

## Deployment

The application is configured to run on Replit with the following specifications:
- Gunicorn web server
- PostgreSQL database support
- Automatic HTTPS
- Environment variable management

## Model Information

The price prediction model:
- Uses Random Forest Regressor
- Features both numerical and categorical data
- Includes confidence interval estimation
- Regular retraining with new data
