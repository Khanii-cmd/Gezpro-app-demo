# 🎓 GenZPro — Flutter App

A complete Flutter student portal app for GenZPro Tech Institute.

## 📱 Screens
| Screen | Route | Description |
|--------|-------|-------------|
| Splash | `/` | Animated logo, auto-navigates to Home |
| Home | `/home` | Landing page with features & courses |
| Login | `/login` | Email + password login |
| Signup | `/signup` | 2-step registration form |
| Welcome | `/welcome` | Dashboard after login |
| Profile | `/profile` | View & edit profile |

## 🚀 Setup in VS Code

### Step 1 — Install Flutter SDK
Download from https://docs.flutter.dev/get-started/install  
Make sure `flutter` is in your PATH. Verify:
```
flutter doctor
```

### Step 2 — Open Project in VS Code
```
code genzpro
```
Or: **File → Open Folder → select `genzpro` folder**

### Step 3 — Install Extensions
Install these VS Code extensions:
- **Flutter** (by Dart Code)
- **Dart** (by Dart Code)

### Step 4 — Get Dependencies
Open VS Code terminal (Ctrl+`) and run:
```
flutter pub get
```

### Step 5 — Run the App

**On an Emulator:**
- Open Android Studio → AVD Manager → Start an emulator
- In VS Code, press **F5** or run:
```
flutter run
```

**On a Physical Device:**
- Enable USB Debugging on your Android phone
- Connect via USB
- Run: `flutter run`

**On Chrome (Web):**
```
flutter run -d chrome
```

---

## 📁 Project Structure

```
genzpro/
├── lib/
│   ├── main.dart                 ← App entry point & routing
│   ├── theme/
│   │   └── app_theme.dart        ← Colors, fonts, theme
│   ├── models/
│   │   └── user_model.dart       ← User data model
│   ├── services/
│   │   └── api_service.dart      ← All API calls
│   ├── widgets/
│   │   └── app_widgets.dart      ← Reusable widgets
│   └── screens/
│       ├── splash_screen.dart
│       ├── home_screen.dart
│       ├── login_screen.dart
│       ├── signup_screen.dart
│       ├── welcome_screen.dart
│       └── profile_screen.dart
└── pubspec.yaml                  ← Dependencies
```

## 🔌 API Endpoints Used
- `POST /signup.php` — Register new user
- `POST /login.php` — Login
- `POST /get_profile.php` — Fetch profile
- `POST /update_profile.php` — Update profile

Base URL: `https://api.genzpro.pk`

## 🎨 Design
- **Colors:** Dark theme (#0A0E1A) + Purple (#6C63FF) + Teal (#00C9A7)
- **Font:** Sora (Google Fonts)
- **Animations:** flutter_animate package
