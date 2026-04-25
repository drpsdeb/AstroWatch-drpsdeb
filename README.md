🌟 AstroWatch 3.1 - AI Automated Astrologer

AstroWatch is a high-precision, real-time Vedic Astrology dashboard. It combines a zero-latency offline spherical trigonometry ephemeris engine with an integrated Parashari AI Astrologer (powered by Google's Gemini AI) to provide deeply personalized astrological insights, natal charts, and current transits (Gochara).

🚀 What's New in Version 3.1

Integrated Parashari AI (Gemini 2.5 Flash): Click on any planetary placement, house, rashi, or nakshatra to instantly generate a personalized 3-sentence prediction adhering strictly to the classical principles of the Brihat Parashara Hora Shastra (BPHS).

Smart API Automation: End-users no longer need to configure API keys! The app securely embeds a domain-locked API key for seamless use on GitHub Pages, while gracefully handling local development testing.

Custom Branding: Updated UI featuring customized application logos and a refined color palette.

Enhanced Cloud Sync: Auto-syncs unlimited client profiles across devices using Firebase.

✨ Key Features

1. Offline Ephemeris Engine: * Calculates planetary positions, Lagna (Ascendant), and True Moon degree mathematically without relying on external astrology APIs.

Uses atomic time adjustments (Delta T) and real-time ayanamsa calculations.

2. Interactive Cosmic Watch Face:

A beautiful 5-ring concentric dial displaying:

   1. Time/Nakshatras

   2. Rashis (Zodiac Signs)

   3. Houses (Bhavas)

   4. Current Transits (Gochara)

   5. Natal Placements (Birth Chart)

3. Vimshottari Dasa Calculator:

Automatically calculates current Mahadasha, Antardasha, and Pratyantardasha based on the exact natal Moon degree.

Generates a timeline of upcoming Dasha changes.

4. Time-Travel Mode:

Manually fast-forward or rewind time by hours, days, months, or years to observe how transits and Dashas shift in real-time.

5. Classical Vedic Lore:

Built-in classical interpretations for all 9 Grahas, 12 Rashis, 12 Bhavas, and 27 Nakshatras.

🛠️ Technical Stack

   Frontend: React (Vite)
   
   Styling: Tailwind CSS, Lucide React (Icons)
   
   AI Engine: Google Gemini API (gemini-2.5-flash)
   
   Backend/Storage: Firebase (Auth & Firestore)
   
   Hosting: GitHub Pages

📱 How to Install on Your PhoneAstroWatch is a fully certified Progressive Web App. You do not need the Google Play Store or Apple App Store to install it.

1. Open Google Chrome (Android) or Safari (iOS) on your mobile device.
2. Navigate to the live link: https://drpsdeb.github.io/AstroWatch-drpsdeb/
3. Wait for the page to load.
4. Tap your browser's menu (the three dots in Chrome, or the Share square in Safari).
5. Tap "Install App" or "Add to Home Screen".
6. AstroWatch will now appear alongside your native apps and will run 100% offline!
   
🛠️ Local Development SetupIf you want to download the code and run the app locally on your computer:

Prerequisites

Node.js installed on your machine.

Installation
1. Clone this repository: git clone [https://github.com/drpsdeb/AstroWatch-drpsdeb.git](https://github.com/drpsdeb/AstroWatch-drpsdeb.git)
2. Navigate into the folder:cd AstroWatch-drpsdeb
3. Install dependencies:npm install
4. Start the local development server: npm run dev
   
Building for Production (GitHub Pages)If you make changes to the code and want to deploy them:

1. Run the Vite build command:npm run build
2. The compiled application will be generated in the dist folder.
3. Commit and push the contents of the dist folder to your live branch.

💻 Local Development Setup

If you wish to clone and run this project locally on your machine:

1. Clone the repository:

git clone [https://github.com/drpsdeb/AstroWatch-drpsdeb.git](https://github.com/drpsdeb/AstroWatch-drpsdeb.git)
cd AstroWatch-drpsdeb


2. Install Dependencies:

npm install


3. Configure the AI API Key for Local Testing:

AstroWatch uses a "Smart Environment Detector" for its AI features.

Open src/App.jsx and locate the callGemini function.

Replace "PASTE_YOUR_LOCKED_KEY_HERE" with your Google Gemini API Key.

Note: Ensure your Google Cloud API key restrictions allow requests from http://localhost:5173/* if you wish to test locally.

4. Run the Local Server:

npm run dev

Hold Ctrl and click the http://localhost:5173 link in your terminal to open it.

   🚀 Deployment to GitHub Pages

To compile the latest code and push it to the live site:

Stop the local dev server (Ctrl + C).

Run the build command to package the code into the dist folder:

npm run build

Upload the contents of the newly updated dist folder to your GitHub repository.

Created by Dr. P.S. Deb | Bridging ancient Vedic wisdom with modern computational technology.
