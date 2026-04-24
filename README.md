🌌 AstroWatch v2.4.1A 
mathematically rigorous, offline-first Progressive Web App (PWA) for real-time Vedic Astrology, Ephemeris Tracking, and Vimshottari Dasa calculations.

📖 OverviewAstroWatch is a highly advanced, self-contained astronomical watch face that combines a classic analog interface with precise Vedic astrological data. It eliminates the need for expensive, rate-limited external APIs by utilizing an internal mathematical engine capable of calculating planetary degrees, transits (Gochara), and Dasa timelines with extreme precision, right in your browser.

✨ Key Features🕰️ 

The Cosmic Watch Face: A multi-layered visual dial displaying:
Outer Rings: Current Time, 27 Nakshatras, and 12 Zodiac Signs (Rashis).
Middle Rings: Astrological Houses (H1-H12) dynamically based on Ascendant (Lagna).
Inner Rings: Real-time planetary transits (Gochara) overlapping the static Natal Chart.

🪐 High-Precision Offline Engine (v2.4.1): 

Calculates Ephemeris entirely offline using JavaScript.
Atomic Time Calibration: Automatically adjusts for historical Delta T ($\Delta$T) to sync Universal Time with Terrestrial Time.
True Lahiri Ayanamsa: Baseline matched accurately to the Swiss Ephemeris.
24-Term Meeus Lunar Array: Computes top complex lunar perturbations (Evection, Variation, Annual Equation) for an ultra-precise Moon degree.

📜 Vimshottari Dasa Timeline: Calculates precise Mahadasha, Antardasha, and Pratyantardasha down to the exact day, fueled by the offline Moon engine.

☁️ Cloud Sync & PWA: Built-in Firebase support for securely saving profiles across devices. Operates as a Progressive Web App (PWA) for 100% offline mobile use.

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

🔬 The Mathematics (Why v2.4.1?)

Earlier versions of AstroWatch exhibited a slight drift (up to 16-20 days) in Vimshottari Dasa calculations when compared to the massive Swiss Ephemeris database.
This was solved in Version 2.4.1 by implementing:

1. Delta T Interpolation: A 31-second discrepancy between human clock time and atomic time in the 1950s shifts the Moon by ~0.0047°. The engine now interpolates historical Delta T tables to eliminate this error.
2. Jean Meeus Polynomials: The lunar engine now applies the top 24 trigonometric perturbation terms, tightening the offline longitudinal error margin to less than 0.01°.

   Developed and maintained by Dr. PS Deb. For educational and astrological research purposes.
