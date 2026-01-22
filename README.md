# DetectraCare 🏥

Hey! This is DetectraCare – a health risk assessment tool I built to help people understand their health better before problems arise.

# Url-https://detectracare.netlify.app/

## What it does

- **Health Check** – Fill in your vitals, lifestyle habits, and symptoms. The app calculates your risk for diabetes, heart disease, hypertension, and mental health issues using evidence-based scoring.
- **AI Diet Planner** – Ask for personalized meal suggestions based on your dietary needs (low-carb, high-protein, etc.). Returns structured meal plans with breakfast, lunch, dinner, and snack recommendations.
- **HealthBuddy Chatbot** – Chat with an AI about health questions. You can also upload a prescription PDF and it'll analyze the contents for you.
- **User Accounts** – Sign up to save your health assessments to the cloud. View your history in the dashboard to track progress over time.
- **Responsive Design** – Works on desktop, tablet, and mobile. The chatbot even has a close button for mobile users.

## Tech Stack & Credits

### Core
- Plain HTML5, CSS3, and JavaScript – no frameworks, everything in one file for easy deployment

### Fonts
- [Inter](https://fonts.google.com/specimen/Inter) – for body text
- [Outfit](https://fonts.google.com/specimen/Outfit) – for headings

### AI & Backend Services
- [Google Gemini API](https://ai.google.dev/) – powers the chatbot and nutrition planner
- [Firebase Authentication](https://firebase.google.com/docs/auth) – handles user login/signup
- [Firebase Realtime Database](https://firebase.google.com/docs/database) – stores user profiles and health reports

### Libraries
- [PDF.js by Mozilla](https://mozilla.github.io/pdf.js/) – extracts text from uploaded PDFs client-side

## Health Data Sources

The rotating facts on the homepage come from these sources:

| Fact | Source |
|------|--------|
| "80% of premature heart disease and strokes are preventable" | [WHO - Cardiovascular Diseases](https://www.who.int/health-topics/cardiovascular-diseases) |
| "Physical activity reduces depression risk by 30%" | [NIH - Physical Activity Guidelines](https://www.niddk.nih.gov/health-information/weight-management/physical-activity) |
| "Type 2 diabetes is largely preventable" | [CDC - Diabetes Prevention](https://www.cdc.gov/diabetes/prevention/index.html) |
| "Early cancer detection = 90%+ survival rates" | [American Cancer Society - Early Detection](https://www.cancer.org/cancer/screening.html) |
| "Less than 6 hours sleep increases inflammation" | [Sleep Research Society](https://sleepresearchsociety.org/) |

### Risk Calculation Logic

The health scoring is based on established medical guidelines:

- **Diabetes Risk** – Uses factors from [American Diabetes Association guidelines](https://diabetes.org/about-diabetes/type-2/risk-test) (BMI, age, family history, activity level, sugar intake)
- **Blood Pressure Classification** – Based on [American Heart Association BP categories](https://www.heart.org/en/health-topics/high-blood-pressure/understanding-blood-pressure-readings)
- **Cardiovascular Risk** – Inspired by the [Framingham Heart Study](https://framinghamheartstudy.org/) risk factor model
- **Mental Health Indicators** – References [WHO Mental Health guidelines](https://www.who.int/news-room/fact-sheets/detail/mental-health-strengthening-our-response)
- **BMI Formula** – Standard [WHO BMI classification](https://www.who.int/europe/news-room/fact-sheets/item/body-mass-index---bmi)

## How to Run

Just open `index.html` in any browser. Done.

For live reload during development:
```bash
npx live-server
```

## Project Structure

```
index.html  – the entire app (HTML + CSS + JS all-in-one)
logo.png      – site icon/logo
README.md     – this file
```

## Setting Up Your Own

If you want to use your own Firebase/Gemini:

1. Create a [Firebase project](https://console.firebase.google.com/)
2. Enable Authentication and Realtime Database
3. Get a [Gemini API key](https://ai.google.dev/)
4. Replace the config values in `index.html`

## Important Disclaimer ⚠️

This is an educational project. The health scores are rough estimates based on general guidelines – **they are NOT medical diagnoses**. For real health concerns, please consult an actual healthcare professional.

---

Built as a learning project. Thanks to WHO, AHA, CDC, and ADA for making health data publicly accessible!

---

## 🤝 Collaborative Project

This is a collaborative project – feel free to share feedback, suggest improvements, or contribute! Your input helps make DetectraCare better for everyone.
