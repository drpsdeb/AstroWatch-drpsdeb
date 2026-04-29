AstroWatch 🌌 (v4.8.0)

A beautifully designed, completely serverless, AI-powered Vedic Astrology (Parashari) web application. AstroWatch combines high-precision offline ephemeris calculations with Google's Gemini AI to deliver deeply personalized, context-aware astrological insights in real-time.

✨ What's New in Version 4.8.0

1. Adaptive AI Knowledge Levels: Choose between "Beginner/Layperson" (translates astrology into plain English life advice) or "Expert" (uses strict classical Vedic terminology like Lagna, Gochara, and Bhava).

2. Lucky Elements Finder: A dedicated AI tool to generate your auspicious colors, gemstones, and directions based strictly on your Lagna and current Mahadasha.

3. Streamlined Onboarding: Added a direct, 1-click link to Google AI Studio to help non-technical users easily get their free Gemini API key.

4. Mobile Touch Enhancements: Disabled native browser text-selection and image-saving popups on the Watch Face so mobile users can tap elements without triggering contextual menus.

5. Responsive UI Overhaul: The cosmic dial now scales beautifully on mobile and tablet devices, sitting perfectly centered with the live clock relocated above the dial.

6. Vimshottari Dasa Redesign: A clean, single-line display of the currently active Mahadasha ➔ Antardasha ➔ Pratyantardasha, with a dropdown containing the complete upcoming timeline.

7. Fortified Memory Loader: Added aggressive data-validation to local storage to completely prevent app crashes caused by corrupted or incomplete saved profiles.

🚀 Core Features

⏱️ Realtime Cosmic Dial

   Visually tracks current planetary transits (Gochara) overlaid perfectly onto your static Natal Birth Chart.

   Hover Tooltips: Hover over any planet, zodiac sign (Rashi), house (Bhava), or Nakshatra to instantly see its classical BPHS significance.

   Time Travel UI: Switch from "Live Realtime Tracking" to a custom Date/Time picker to freeze the clock and investigate transits in the past or future.

🤖 Parashari AI (Powered by Gemini 2.5 Flash)

   Click on any astrological element on the dial to get a highly personalized, 3-4 sentence AI prediction analyzing that specific natal placement or transit against your current Dasha.
   
   Ask the Astrologer: Ask specific questions (e.g., "Tell me about my career prospects") and the AI will analyze your chart, transits, and Dashas to answer you.
   
   Astro-Dream Decoder: Input your recent dreams and the AI will decode them spiritually and astrologically based on the current transiting planets.
   
   Daily Cosmic Mantra & Upaya: Generate a daily prediction, personalized Vedic remedy, and practical precautions for the day.

☁️ Cloud Sync & Local Privacy

   Multi-profile management allowing you to save charts for friends and family.
   
   Secure API Keys: Your Gemini API key is stored securely in your browser's local storage and is never sent to a database.
   
   Firebase Integration: Profiles are synced seamlessly to the cloud across your devices.
   
   Auto-Geocoding: Type a city name, and AstroWatch automatically fetches the precise Latitude, Longitude, and UTC Timezone.


🛠️ Technical Stack

   Frontend: React, Tailwind CSS, Lucide React (Icons)

   Astrology Engine: Custom offline Javascript Ephemeris (Calculates Julian Dates, Ayanamsa, True Lagna, and planetary longitudes).

   AI Integration: Google Generative AI (Gemini v1beta API).

   Backend/Storage: Firebase (Auth & Firestore).

   APIs: Nominatim (OpenStreetMap) for Geocoding, Open-Meteo for Timezone offsets.

📦 Installation & Setup

   1. Clone the repository:
      git clone [https://github.com/yourusername/astrowatch.git](https://github.com/yourusername/astrowatch.git)
cd astrowatch

   2.Install dependencies: npm install

   3.Configure Firebase (Optional for Local Dev): AstroWatch expects __firebase_config and __app_id to be injected globally. If you are running locally without a cloud build    environment, you can define these inside your index.html or at the top of App.jsx:

   window.__firebase_config = '{"apiKey": "...", "authDomain": "...", "projectId": "..."}';
   window.__app_id = "astrowatch-local";


   4. Start the development server: npm run dev

   
🔐 Privacy & API Keys

   To use the AI features, users must provide their own Google Gemini API Key.

   Keys are free to obtain from Google AI Studio.

   The key is stored purely in the client's localStorage. No server has access to it.

📜 License

   This project is open-source and available under the MIT License.
   
Created by Dr. P.S. Deb | Bridging ancient Vedic wisdom with modern computational technology.
