SmartKumbh: The Sentient & Resilient Pilgrim Ecosystem

Team ID: TH1309

1. Overview

SmartKumbh is a full-stack web platform designed to enhance the safety, navigation, and spiritual experience of pilgrims during the Kumbh Mela. The platform provides:

Real-time crowd monitoring & safety alerts

Lost & found services with QR-based identification

AI-powered multilingual chatbot (supports 12 Indian languages)

Step-by-step spiritual journey navigation & event updates

Role-based admin controls for security officers and event managers

With interactive maps, QR-based identification, and role-based access, SmartKumbh ensures safety, smooth navigation, and accessibility for millions of visitors.

2. Problem & Solution

Problem Statement:
Massive crowds at Kumbh Mela lead to challenges like overcrowding, safety risks, missing persons, lack of real-time information, and difficulty navigating spiritual sites.

Solution:
SmartKumbh integrates AI, mapping, and real-time data systems to provide:

Live crowd density monitoring & safety alerts

Lost & found assistance with QR-based identification

AI-powered multilingual chatbot (Google Gemini AI)

Step-by-step spiritual journey guidance & event updates

Role-based admin controls for police, medical, and event managers

3. System Architecture & Workflow

User Side:

Live navigation and safety alerts

Spiritual journey guidance

QR-based ID for emergency contacts

AI Chatbot support in multiple languages

Admin Side:

Real-time monitoring of crowd density, bathing zones, parking, and facilities

Manage safety alerts, lost & found reports, event schedules, and cleanliness reports

Data Flow:

Data Collection: Cameras/sensors, user reports, admin inputs, event schedules, lost & found cases.

Processing:

PostgreSQL via Drizzle ORM for structured data

Firestore for real-time sync

AI chatbot (Google Gemini) for queries

Zod validation ensures clean and secure data

Output: Interactive map, alerts, event schedules, facility details, and chatbot responses

4. Tech Stack

Frontend: React 18 + TypeScript, Tailwind CSS, Radix UI, shadcn/ui, Wouter

Backend: Node.js + Express.js

Database: PostgreSQL (Neon) + Firestore

AI: Google Gemini AI (multilingual chatbot)

Maps: Leaflet + OpenStreetMap

Auth & Storage: Firebase Authentication + Firestore

Other Tools: QRCode.js, TanStack Query, Zod, React Hook Form

5. Interactive Features

Leaflet-based maps with dynamic markers

QR code generation for pilgrim identification

Multilingual chatbot (KumbhBot) powered by Google Gemini AI

Elderly-friendly mode with high contrast and larger fonts

Real-time updates for crowd density, alerts, and events

Mobile-first responsive design

6. Future Scope

Mobile app integration (Android/iOS) with offline support

AI predictive crowd control and personalized guidance

Integration with government safety and tourism systems

IoT sensor-based crowd density monitoring

Multi-user dashboards for admin, police, and medical teams

7. Getting Started
7.1 Clone the Repository
git clone https://github.com/Imayankparadkar/SmartKumbh.git
cd SmartKumbh

7.2 Install Dependencies
npm install

7.3 Create .env File

Create a .env file in the root of your project (same level as package.json) and add the following variables:

# Firebase
VITE_FIREBASE_API_KEY=
VITE_FIREBASE_APP_ID=
VITE_FIREBASE_AUTH_DOMAIN=
VITE_FIREBASE_MESSAGING_SENDER_ID=
VITE_FIREBASE_PROJECT_ID=
VITE_FIREBASE_STORAGE_BUCKET=

# Google Gemini AI
VITE_GEMINI_API_KEY=
VITE_GOOGLE_GEMINI_API_KEY=

# EmailJS
EMAILJS_PUBLIC_KEY=
EMAILJS_SERVICE_ID=
EMAILJS_TEMPLATE_ID=

# PostgreSQL / Neon Database
DATABASE_URL=
PGDATABASE=
PGHOST=
PGPORT=
PGUSER=
PGPASSWORD=


Instructions:

Firebase variables: Get these from your Firebase project settings under “Project Settings → General → Your apps → Firebase SDK snippet.”

Google Gemini API key: Get from Google Cloud or Gemini AI console.

EmailJS variables: Create an EmailJS account and set up a service, template, and public key.

Database variables: Use your PostgreSQL/Neon database credentials. DATABASE_URL is optional if you use separate PG variables.

7.4 Run the Website
# Start Full Website
npm run dev


Open http://localhost:5000 (Vite default port) to see your website.

8. Notes

Ensure Firebase Authentication, Firestore, and EmailJS services are enabled and configured properly.

PostgreSQL database must be running and accessible via .env credentials.

Google Gemini API should be enabled for your project in Google Cloud.

Keep .env file secret; do not commit it to GitHub.
