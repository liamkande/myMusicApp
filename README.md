My Music App

An streaming Music-like mobile app built with React Native and Expo, designed for a smooth and responsive UI with animations. The app uses GraphQL for data handling, Firebase for backend services, and MobX for global state management. Built for a streamlined music browsing and playback experience.

Features

	•	Responsive and Animated UI: Smooth transitions and UI animations to enhance user experience.
	•	GraphQL API Integration: Efficient data fetching and mutations via Apollo Client.
	•	Firebase Backend: Firebase for authentication, database (Firestore), and cloud functions.
	•	MobX for State Management: Manage global state (e.g., current track, playlists) with MobX.
	•	Custom Hooks: Reusable custom hooks for handling authentication, player controls, and more.

Directory Structure

src/
├── components/          # Reusable UI components like buttons, sliders, etc.
├── screens/             # Major screens like Home, Library, Search, etc.
├── stores/              # MobX stores for global state
├── navigation/          # Navigation setup
├── assets/              # Fonts, icons, images, etc.
├── utils/               # Utility functions and helpers
├── graphql/             # GraphQL setup
│   ├── schema/          # Local GraphQL schemas
│   ├── queries.tsx       # GraphQL queries
│   ├── mutations.tsx     # GraphQL mutations
│   ├── ApolloClient.tsx  # Apollo client configuration
├── firebase/            # Firebase configuration and functions
│   ├── config.tsx        # Firebase initialization and config
│   ├── auth.tsx          # Firebase authentication helper functions
│   ├── firestore/       # Firestore-specific queries and helper functions
└── hooks/               # Custom React hooks for app logic
├── useAuth.tsx       # Authentication-related hooks
├── useTrackPlayer.tsx # Custom hook for audio player controls and state

Tech Stack

	•	React Native & Expo: For building the mobile app and rapid prototyping.
	•	GraphQL & Apollo Client: For efficient data fetching and management.
	•	Firebase: For authentication, Firestore database, and cloud functions.
	•	MobX: For global state management.
	•	Custom Hooks: To encapsulate specific functionalities, making the codebase cleaner and more modular.

Setup Instructions

Prerequisites

	•	Node.js and Yarn
	•	Expo CLI
	•	Firebase account

Getting Started

	1.	Clone the repository:

git clone https://github.com/liamkande/myMusicApp.git
cd myMusicApp


	2.	Install dependencies:

yarn install


	3.	Firebase Setup:
	•	Create a Firebase project in the Firebase Console.
	•	Enable Firestore and set up authentication.
	•	Download the Firebase configuration and add it to firebase/config.ts.
	4.	Environment Variables:
	•	Set up any environment variables, like Firebase keys, as needed.
	5.	Start the Expo server:

expo start


	6.	Install Expo Go (optional):
	•	For iOS or Android, use the Expo Go app to scan the QR code and test on a physical device.

Usage

Running the App

	1.	Run the app using Expo:

expo start


	2.	Scan the QR code in the Expo Go app or open in a simulator.

Available Scripts

	•	expo start: Start the Expo development server.
	•	yarn build: Build the app for production (requires Expo account).
	•	firebase deploy --only functions: Deploy Firebase Cloud Functions.

Key Components

	•	Apollo Client: Configured in src/graphql/ApolloClient.ts.
	•	MobX Stores: Found in src/stores/, with MusicStore.tsx handling global music state.
	•	Firebase Functions: Cloud functions reside in firebase/functions/ (optional if testing locally).

Contributing

Feel free to contribute to this project! Open a pull request for any bug fixes, feature requests, or improvements.

License

This project is licensed under the MIT License.

This setup should guide you through setting up, running, and understanding the project structure. Happy coding!