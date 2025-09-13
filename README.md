AI Notes App
An intelligent, modern note-taking application powered by Google's Gemini API and Firebase. This app goes beyond simple text storage, offering a suite of AI-powered tools to make your notes smarter, more organized, and easier to study from.

✨ Features
This application is built as a single-file web app, demonstrating the power of modern web technologies and cloud services.

📝 Real-time Note Taking: A clean, intuitive interface for creating and editing notes.

☁️ Cloud-Synced with Firebase: All notes are saved instantly and securely to Firestore, available in real-time across sessions.

🤖 AI-Powered Content Tools (Gemini API):

Summarize: Condense long notes into concise summaries.

Expand: Elaborate on brief points to create more detailed content.

Fix Grammar: Correct spelling and grammatical errors with a single click.

🎓 Study Mode: A distraction-free view that focuses solely on your note content.

AI Highlighting: Automatically identifies and highlights the key points in your notes for efficient studying.

💬 AI Q&A: Chat directly with your notes! Ask questions in plain English and get answers based on the note's content.

🃏 AI Flashcard Generation: Instantly turn any note into a set of interactive flashcards for active learning.

🛠️ Tech Stack
Frontend: HTML5, Tailwind CSS, Vanilla JavaScript (ES Modules)

Backend: Firebase (Firestore Database, Anonymous Authentication)

AI Model: Google Gemini API

🚀 Getting Started (How to Run Locally)
To run this project on your own machine, follow these steps:

Clone the Repository:

git clone [https://github.com/your-username/ai-notes-app.git](https://github.com/your-username/ai-notes-app.git)
cd ai-notes-app

Firebase Setup:

Create a new project at the Firebase Console.

Enable Firestore Database and start it in Test Mode.

Enable Authentication and add Anonymous as a sign-in provider.

Copy your project's Firebase configuration keys.

Google AI Studio Setup:

Go to Google AI Studio.

Create a new API key.

Configure the App:

Open the index.html file.

Find the firebaseConfig object and replace the placeholder values with your own Firebase keys.

Find the callGeminiAPI function and replace "YOUR_GEMINI_API_KEY_HERE" with your Google AI Studio key.

Run the App:

If you're using VS Code, install the "Live Server" extension and click "Go Live" to run the index.html file.

🔗 Live Project Link
You can try out the live version of the app here: [your-live-project-link-goes-here]

This project was created for the Buildathon.


### ✅ 2. A Live Project Link

This is the most important step for letting the judges (and others) easily try your application. We will use **Firebase Hosting** to deploy your app, which is the perfect tool since you're already using Firebase.

Here is a step-by-step guide to get your live link:

#### Step 1: Install Node.js
If you don't have it, install Node.js from [the official website](https://nodejs.org/). This will also install `npm` (Node Package Manager), which you'll need.

#### Step 2: Install the Firebase CLI
Open your computer's terminal (or the terminal inside VS Code) and run this command:
```bash
npm install -g firebase-tools

Step 3: Log in to Firebase
In the same terminal, run this command. It will open a browser window for you to log in to your Google account.

firebase login

Step 4: Initialize Your Project for Hosting
In your terminal, navigate to your project folder (the one with index.html).

Run the initialization command:

firebase init

The tool will ask you a series of questions. Here’s how to answer them:

"Are you ready to proceed?" -> Yes

"Which Firebase features do you want to set up?" -> Use the arrow keys and spacebar to select Hosting, then press Enter.

"Please select an option:" -> Use an existing project

Select your ai-notes-app-471dd project from the list.

"What do you want to use as your public directory?" -> Type . (a single dot) and press Enter. This tells Firebase that your index.html is in the main folder.

"Configure as a single-page app?" -> Yes

"Set up automatic builds and deploys with GitHub?" -> No (for simplicity).

Step 5: Deploy Your App
This is the final step! In your terminal, run:

firebase deploy
