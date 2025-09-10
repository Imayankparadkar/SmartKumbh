# SmartKumbh: The Sentient & Resilient Pilgrim Ecosystem
**Team ID:** TH1309

---

## 1. Overview
SmartKumbh is a **full-stack web platform** designed to enhance **safety, navigation, and spiritual experience** for pilgrims during the Kumbh Mela.

**Key Features:**
- Real-time **crowd monitoring & safety alerts**
- **Lost & Found services** with QR-based identification
- **AI-powered multilingual chatbot** (supports 12 Indian languages)
- Step-by-step **spiritual journey navigation & event updates**
- **Role-based admin controls** for security officers and event managers
- **Interactive maps** for smooth navigation

SmartKumbh ensures **safety, accessibility, and a seamless experience** for millions of visitors.

---

## 2. Problem & Solution

**Problem Statement:**  
Massive crowds at Kumbh Mela create challenges such as:
- Overcrowding & safety risks
- Missing persons
- Lack of real-time information
- Difficulty navigating spiritual sites

**Our Solution:**  
SmartKumbh leverages **AI, real-time data, and mapping systems** to provide:
- **Live crowd density monitoring & safety alerts**
- **Lost & Found assistance** with QR-based identification
- **AI multilingual chatbot** (Google Gemini AI)
- Step-by-step **spiritual journey guidance & event updates**
- **Role-based admin controls** for police, medical, and event managers

---

## 3. System Architecture & Workflow

### User Side:
- Live navigation & safety alerts
- Spiritual journey guidance
- QR-based ID for emergency contacts
- AI Chatbot support in multiple languages

### Admin Side:
- Real-time monitoring of crowd density, bathing zones, parking, and facilities
- Manage safety alerts, lost & found reports, event schedules, and cleanliness reports

### Data Flow:
- **Data Collection:** Cameras, sensors, user reports, admin inputs, event schedules, lost & found cases
- **Processing:**
  - PostgreSQL via **Drizzle ORM** for structured data
  - **Firestore** for real-time sync
  - **AI chatbot (Google Gemini)** for queries
  - **Zod validation** ensures secure and clean data
- **Output:** Interactive maps, alerts, event schedules, facility details, and chatbot responses

---

## 4. Tech Stack

**Frontend:** React 18 + TypeScript, Tailwind CSS, Radix UI, shadcn/ui, Wouter  
**Backend:** Node.js + Express.js  
**Database:** PostgreSQL (Neon) + Firestore  
**AI:** Google Gemini AI (multilingual chatbot)  
**Maps:** Leaflet + OpenStreetMap  
**Auth & Storage:** Firebase Authentication + Firestore  
**Other Tools:** QRCode.js, TanStack Query, Zod, React Hook Form

---

## 5. Interactive Features
- Leaflet-based maps with dynamic markers
- QR code generation for pilgrim identification
- Multilingual chatbot (KumbhBot) powered by Google Gemini AI
- Elderly-friendly mode with high contrast & larger fonts
- Real-time updates for crowd density, alerts, and events
- Mobile-first responsive design

---

## 6. Future Scope
- Mobile app integration (Android/iOS) with offline support
- AI predictive crowd control & personalized guidance
- Integration with **government safety & tourism systems**
- IoT sensor-based crowd density monitoring
- Multi-user dashboards for admin, police, and medical teams

---

## 7. Getting Started

### 7.1 Clone the Repository
```bash
git clone https://github.com/Imayankparadkar/SmartKumbh.git
cd SmartKumbh
7.2 Install Dependencies
bash
Copy code
npm install
7.3 Create .env File
Create a .env file in the root directory and add:

env
Copy code
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

Firebase: Get variables from Firebase project settings → SDK snippet

Google Gemini AI: Get key from Google Cloud / Gemini AI console

EmailJS: Set up a service, template, and public key

PostgreSQL: Use database credentials

7.4 Run the Website
bash
Copy code
npm run dev
Open http://localhost:5000 to view your site.

8. Notes
Ensure Firebase Auth, Firestore, and EmailJS are properly configured

PostgreSQL must be running and accessible

Google Gemini API must be enabled

Keep .env secret; do not commit to GitHub
