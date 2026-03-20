# GigShield AI – Predictive Income Protection for Gig Workers

## Problem Statement
Gig workers such as Swiggy and Zomato delivery partners lose income due to external disruptions like heavy rain, pollution, and extreme heat. Currently, there is no system to protect their daily earnings.

## Solution
GigShield AI is an AI-powered parametric insurance platform that predicts disruptions and automatically compensates workers for income loss.

## Workflow
1. Worker registers with location and income details  
2. AI calculates weekly insurance premium  
3. Worker purchases insurance  
4. System monitors weather and environmental data  
5. If disruption occurs, claim is automatically triggered  
6. Worker receives payout  

## AI Strategy
We use:
- Weather data
- Pollution data
- Historical disruption data  

Models:
- Random Forest → risk prediction & premium calculation  
- Isolation Forest → fraud detection  

## Weekly Pricing Model
- Low risk → ₹10/week  
- Medium risk → ₹15/week  
- High risk → ₹25/week  

## Parametric Triggers
- Rainfall > 70mm  
- Temperature > 42°C  
- AQI > 350  

## Tech Stack
- Frontend: React  
- Backend: FastAPI  
- Database: PostgreSQL  
- AI: Python (Scikit-learn)  
- APIs: OpenWeather, OpenAQ  

## Adversarial Defense & Anti-Spoofing Strategy
To prevent fraud, we use:
- GPS and movement tracking  
- Weather API cross-check  
- AI-based anomaly detection  
- Detection of repeated or unusual claims  
- Device and IP tracking  

This ensures fake claims are blocked while genuine workers are protected.
