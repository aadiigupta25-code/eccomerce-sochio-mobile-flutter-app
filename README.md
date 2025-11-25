# Era Shop - Sochio E-commerce Mobile App

A Flutter-based e-commerce mobile application with live selling features, integrated with Node.js backend.

## 🚀 Features

- **E-commerce Platform**: Complete shopping experience
- **Live Selling**: Real-time product selling with video streaming
- **User Authentication**: Login/Register with OTP verification
- **Product Management**: Browse, search, and filter products
- **Shopping Cart**: Add/remove items, checkout process
- **Order Management**: Track orders, order history
- **Payment Integration**: Multiple payment gateways (Razorpay, Stripe, Flutterwave)
- **Real-time Chat**: Socket.io integration for live communication
- **Push Notifications**: Firebase messaging
- **Social Login**: Google Sign-in, Apple Sign-in

## 🛠️ Tech Stack

- **Frontend**: Flutter (Dart)
- **State Management**: GetX
- **Backend**: Node.js + Express
- **Database**: MongoDB Atlas
- **Authentication**: Firebase Auth + JWT
- **Payment**: Razorpay, Stripe, Flutterwave
- **Real-time**: Socket.io
- **Video**: Zego Express Engine
- **Notifications**: Firebase Cloud Messaging

## 📱 Dependencies

```yaml
dependencies:
  flutter:
    sdk: flutter
  get: ^4.6.6
  http: ^1.1.0
  firebase_core: ^3.2.0
  firebase_auth: ^5.1.2
  flutter_stripe: ^10.0.0
  razorpay_flutter: ^1.3.6
  flutterwave_standard: ^1.0.8
  image_picker: ^1.0.4
  video_player: ^2.8.6
  zego_express_engine: ^3.15.1+2
  socket_io_client: ^2.0.3+1
  # ... and 20+ more dependencies
```

## 🔧 Setup Instructions

### Prerequisites
- Flutter SDK (>=2.18.6 <3.0.0)
- Android Studio / VS Code
- Node.js (for backend)
- Firebase account
- MongoDB Atlas account

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/aadiigupta25-code/eccomerce-sochio-mobile-flutter-app.git
   cd eccomerce-sochio-mobile-flutter-app
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Configure API URL**
   
   Edit `lib/utiles/api_url.dart`:
   ```dart
   // For production
   static const BASE_URL = "https://sochio-backend.onrender.com/";
   
   // For local development
   // static const BASE_URL = "http://localhost:5000/";
   ```

4. **Run the app**
   ```bash
   flutter run
   ```

## 🌐 Backend Integration

The app is fully integrated with a Node.js backend deployed on Render.com:

- **Production URL**: https://sochio-backend.onrender.com/
- **API Endpoints**: 50+ configured endpoints
- **Authentication**: JWT + OTP verification
- **Database**: MongoDB Atlas
- **File Storage**: Configured for images/videos

### API Categories
- ✅ Authentication APIs (login, OTP, password management)
- ✅ User Management APIs (profile, settings)
- ✅ Product APIs (CRUD, search, filters)
- ✅ Cart & Checkout APIs
- ✅ Order Management APIs
- ✅ Payment Gateway APIs
- ✅ Live Selling APIs
- ✅ Real-time Chat APIs
- ✅ Notification APIs

## 📁 Project Structure

```
lib/
├── ApiModel/          # Data models
├── ApiService/        # API service classes
├── Controller/        # GetX controllers
├── View/             # UI screens
│   └── MyApp/        # App screens
├── utiles/           # Utilities
│   └── api_url.dart  # API configuration
└── main.dart         # App entry point
```

## 🔐 Configuration

### API Keys Setup
Create `lib/utiles/api_keys.dart` (not tracked in git):
```dart
class ApiKeys {
  static const String razorpayKey = "your_razorpay_key";
  static const String stripeKey = "your_stripe_key";
  static const String zegoAppId = "your_zego_app_id";
  static const String zegoAppSign = "your_zego_app_sign";
}
```

### Firebase Setup
1. Add `google-services.json` to `android/app/`
2. Add `GoogleService-Info.plist` to `ios/Runner/`
3. Configure Firebase in `lib/main.dart`

## 🚀 Deployment

### Android APK
```bash
flutter build apk --release
```

### iOS IPA
```bash
flutter build ios --release
```

## 📊 Backend Status

- **Status**: ✅ Live and Running
- **Deployment**: Render.com
- **Database**: MongoDB Atlas
- **API Health**: All endpoints operational
- **Integration**: Complete

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Support

For support, email: aadiigupta25@gmail.com

## 🔗 Links

- **Backend Repository**: [Sochio Backend](https://github.com/aadiigupta25-code/sochio-backend)
- **Live Backend**: https://sochio-backend.onrender.com/
- **Documentation**: See `BACKEND_INTEGRATION_GUIDE.md`

---

**Built with ❤️ using Flutter & Node.js**