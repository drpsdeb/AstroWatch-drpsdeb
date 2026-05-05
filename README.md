# AstroWatch (v4.9.9)

A lightweight, local, AI-powered Vedic Astrology system built with React and Google's Gemini AI. Designed for both beginners looking for simple guidance and expert astrologers tracking precise astronomical movements, traditional vargas, and planetary strengths.

## What is New in v4.9.9

* Exact Sripati Shadbala: A mathematically rigorous calculation of planetary strength (Sthana, Dik, Kaala, Chesta) using exact angular distances. Viewable as a beautiful horizontal bar chart.

* Functional Dignities (Maraka/Badhaka): Automatically calculates Benefics, Malefics, Marakas (Disease inflictors), and Badhakas (Obstruction creators) based on your exact Lagna (Ascendant), strictly following BPHS rules.

* Advanced Vargas Suite: Seamlessly toggle your secondary chart between Navamsha (D9 - Marriage), Dashamsha (D10 - Career), Shashthamsha (D6 - Health/Debts), and Vimshamsha (D20 - Spirituality). Available in both North and South Indian styles.

* Interactive AI Panchang: Toggle between your Natal (Birth) Panchang and the Transit (Current) Panchang. Click it to have the AI interpret how the 5 Limbs of Time are affecting your destiny.

* Supercharged AI Context: The Gemini AI now silently processes your Shadbala scores, Maraka/Badhaka status, and Life Context notes before answering. It knows not just where a planet is, but how powerful and functional it is for you.

* Aspect of planet is included for AI interpretation 

## Core Features

* Local & Private: Runs entirely in your browser. Your Gemini API key and profiles are saved locally, not on a server.

* Cosmic Orrery Mode: A breathtaking geocentric mechanical model of the solar system showing real-time planetary orbits.

* Traditional D1 Charts: Interactive South Indian (Grid) or North Indian (Diamond) natal charts.

* Retrograde (Vakri) Engine: Mathematically calculates planetary rate-of-change to detect retrograde motion in real-time, tagging them with "R".

* Time Machine Controls: Fast-forward or rewind the cosmos with +1 Day, +1 Month, and +1 Year buttons to watch transits unfold and Dashas change dynamically.

* Astronomical Sunclock: Dynamic Day/Night diurnal band with precise Sunrise, Sunset, and Tithi (Lunar Phase) tracking.

* Smart Conjunctions (Yuti): If multiple planets occupy the same sign, clicking one will automatically reveal a button to analyze the combined energy of the conjunction.

* Life Context Module: Input your actual life details (marital status, career phase, health notes) during setup so the AI gives highly specific, reality-based predictions.

* Multilingual AI: Natively generates readings in English, Hindi, Bengali, Tamil, Telugu, Malayalam, and Assamese.

 ## How to Install and Run

1. Ensure you have Node.js installed on your computer.

2. Download or clone this repository to your computer.

3. Open a Command Prompt/Terminal in the downloaded folder and install the requirements:
npm install

4. Start the app:
npm run dev

* Note: To use the Parashari AI features, the app will ask you to paste a free Google Gemini API key during setup. You can generate one instantly at https://aistudio.google.com/app/apikey.
   
Created by Dr. P.S. Deb | Bridging ancient Vedic wisdom with modern computational technology.
