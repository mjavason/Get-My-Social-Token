# Get My Social Token

A simple frontend web application that implements Firebase Google authentication and returns auth tokens for development and testing purposes.

## Features

- **Google Sign-In**: Authenticate users with their Google accounts using Firebase Auth
- **Token Display**: Shows a shortened version of the Firebase ID token for security
- **Token Copy**: Copy the full token to clipboard with one click
- **Clean UI**: Simple, responsive interface for easy use
- **Auto State Management**: Automatically handles user authentication state

## How It Works

1. Click "Sign In with Google" to authenticate with Firebase
2. Upon successful authentication, the app retrieves the Firebase ID token
3. The token is displayed (shortened for security) with an option to copy the full token

## Setup

1. Clone or download this repository
2. Open `index.html` in your web browser
3. Make sure you have an active internet connection for Firebase services

## Configuration

The app is pre-configured with a Firebase project. If you want to use your own Firebase project:

1. Update the `firebaseConfig` object in `index.html` with your Firebase project credentials:

   ```javascript
   const firebaseConfig = {
     apiKey: 'your-api-key',
     authDomain: 'your-project.firebaseapp.com',
     projectId: 'your-project-id',
     appId: 'your-app-id',
   };
   ```

2. Enable Google authentication in your Firebase Console:
   - Go to Authentication > Sign-in method
   - Enable Google as a sign-in provider

## Technologies Used

- **Firebase Authentication**: For Google OAuth integration
- **HTML5/CSS3**: For the user interface
- **Vanilla JavaScript**: For application logic
- **Firebase SDK**: Version 9.6.11 (compat mode)

## Browser Compatibility

This application works in all modern browsers that support:

- ES6+ JavaScript features
- Firebase SDK
- Clipboard API (for token copying)

## Security Notes

- Tokens are only displayed in shortened form by default
- Full tokens are only copied to clipboard when explicitly requested
- All authentication is handled securely through Firebase
