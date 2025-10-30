# 🌿 Puff Club

A comprehensive React Native mobile application for cannabis enthusiasts to discover dispensaries, rate strains, connect with friends, and share experiences.

## 📱 Features

### 🔐 Authentication
- User registration and login
- Owner/Dispensary account management
- Password recovery
- Secure Firebase authentication

### 🏪 Dispensary Features
- Browse nearby dispensaries with map integration
- View trending and top-rated dispensaries
- Search dispensaries with location services
- Dispensary profiles with photos and details
- Owner portal for dispensary management

### 🌱 Strain Management
- Create and rate cannabis strains
- Browse strain profiles with detailed information
- Top-rated strains discovery
- Trending strains feed
- Personal strain collection (My Strains)
- Location-based strain availability
- Wishlist functionality

### 👥 Social Features
- Add and manage friends
- View friend activities
- Pending friend requests
- Friend profile details
- Global activity feed
- Comments and interactions
- Real-time notifications

### 📍 Location Services
- Interactive maps for dispensary locations
- Nearby dispensaries based on GPS
- Location-based strain availability
- Google Places integration

### 👤 User Profile
- Customizable user profiles
- Photo galleries
- Activity history
- Settings management
- Password changes
- Membership management

### 📸 Media
- Photo uploads for dispensaries
- Strain photos
- Profile pictures
- Gallery views

## 🛠 Tech Stack

- **Framework**: React Native 0.63.4 with Expo 42
- **Navigation**: React Navigation 5
- **State Management**: Redux with Redux Persist
- **Backend**: Firebase (Authentication & Firestore)
- **UI Components**: Native Base 2.15.2
- **Maps**: React Native Maps 0.28.0
- **Location**: Expo Location & Google Places API
- **Image Handling**: Expo Image Picker

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v12 or higher)
- npm or yarn
- Expo CLI: `npm install -g expo-cli`
- For iOS: Xcode (macOS only)
- For Android: Android Studio with Android SDK

## 🚀 Getting Started

### Installation

1. Clone the repository:
```bash
git clone https://github.com/superdev947/puff-club.git
cd puff-club
```

2. Install dependencies:
```bash
npm install
```

3. Configure Firebase:
   - Create a Firebase project at [Firebase Console](https://console.firebase.google.com/)
   - Enable Authentication and Firestore
   - Update `src/constants/firebase.js` with your Firebase configuration

4. Configure Google Maps API:
   - Get an API key from [Google Cloud Console](https://console.cloud.google.com/)
   - Enable Maps SDK for Android/iOS and Places API
   - Update the API key in `app.json` under `android.config.googleMaps.apiKey`

### Running the App

#### Start Metro Bundler:
```bash
npm start
```

#### Run on Android:
```bash
npm run android
```

#### Run on iOS:
```bash
npm run ios
```

#### Run on Web:
```bash
npm run web
```

## 📁 Project Structure

```
puff-club/
├── src/
│   ├── assets/          # Images, fonts, and static data
│   ├── components/      # Reusable UI components
│   ├── constants/       # App constants (colors, images, Firebase config)
│   ├── navigation/      # Navigation configuration (Guest/Logged routes)
│   ├── redux/           # State management (actions, reducers, store)
│   ├── scenes/          # App screens/pages
│   │   ├── Auth/        # Authentication screens
│   │   ├── Dispensary/  # Dispensary-related screens
│   │   ├── Friend/      # Friend management screens
│   │   ├── Home/        # Home feed and discovery
│   │   ├── Profile/     # User profile screens
│   │   ├── Strains/     # Strain management screens
│   │   └── ...
│   └── theme/           # Custom theme and styled components
├── App.js               # Root component
├── app.json             # Expo configuration
├── package.json         # Dependencies and scripts
└── README.md            # Project documentation
```

## 🔧 Configuration

### Firebase Setup

Update `src/constants/firebase.js` with your Firebase credentials:

```javascript
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};
```

### Environment Variables

Key configurations to update:
- Firebase config in `src/constants/firebase.js`
- Google Maps API key in `app.json`
- Bundle identifiers in `app.json` (iOS: `com.happy.puffclub`, Android: `com.happy.puffclub`)

## 🏗 Building for Production

### Android:
```bash
npm run build
```

### iOS:
```bash
npm run build:ios
```

## 📦 Key Dependencies

| Package | Purpose |
|---------|---------|
| `react-navigation` | App navigation |
| `redux` & `react-redux` | State management |
| `firebase` | Backend services |
| `native-base` | UI components |
| `react-native-maps` | Map integration |
| `expo-location` | Location services |
| `expo-image-picker` | Image uploads |
| `axios` | HTTP requests |
| `moment` | Date/time handling |
| `geolib` | Geolocation utilities |

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is private and proprietary.

## 👨‍💻 Developer

**superdev947**

## 🐛 Known Issues & Troubleshooting

- **Firebase Auth Issues**: Ensure Firebase is properly configured and enabled in your Firebase Console
- **Google Maps Not Loading**: Verify your Google Maps API key is valid and has the necessary APIs enabled
- **Location Services**: Make sure location permissions are granted on the device
- **Build Failures**: Clear cache with `expo start -c` or `npm start -- --reset-cache`

## 📱 App Version

Current Version: **1.0.0**

## 🎯 Future Enhancements

- [ ] Push notifications for friend activities
- [ ] Advanced strain filtering and search
- [ ] Social sharing integration
- [ ] In-app messaging
- [ ] Dispensary deals and promotions
- [ ] User reviews and ratings system
- [ ] Dark mode support
- [ ] Multi-language support

---

Made with 💚 for the cannabis community
