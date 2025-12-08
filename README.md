# 🌱 AI-Based Mobile App for Durian Leaf Disease Detection

A comprehensive Flutter mobile application that leverages artificial intelligence to detect plant diseases (durian) through image analysis, providing farmers and gardeners with instant diagnosis and treatment recommendations.
## ✨ Core Features

### 🔍 **AI-Powered Disease Detection**
- **Real-time Camera Analysis**: Capture plant images using the device camera
- **Advanced ML Models**: TensorFlow Lite integration for on-device inference
- **High Accuracy**: Trained models for detecting various plant diseases
- **Instant Results**: Get disease diagnosis within seconds

### 📚 **Comprehensive Plant Library**
- **Extensive Database**: Browse detailed information about various crops
- **Disease Catalog**: Complete database of plant diseases with symptoms
- **Scientific Information**: Scientific names, families, and origins
- **Growing Guides**: Seasonal information and growing conditions

### 🩺 **Detailed Disease Information**
- **Expandable Sections**: Collapsible causes and treatment information
- **Database Integration**: Real disease data from Supabase backend
- **Treatment Recommendations**: Specific treatment plans for each disease
- **Prevention Tips**: Proactive measures to prevent disease occurrence

### 🌤️ **Weather Integration**
- **Location-based Weather**: Current weather conditions for your area
- **Agricultural Insights**: Weather impact on plant health
- **Smart Recommendations**: Weather-based care suggestions

### 👤 **User Authentication**
- **Secure Login**: Supabase authentication integration
- **User Profiles**: Personalized experience and history
- **Data Sync**: Cross-device synchronization of user data

### 🎨 **Modern UI/UX**
- **Material Design**: Clean, intuitive interface
- **Responsive Layout**: Optimized for various screen sizes
- **Smooth Animations**: Enhanced user experience with fluid transitions
- **Accessibility**: Built with accessibility best practices

## 🛠️ Technical Stack
### **Frontend**
- **Framework**: Flutter 3.24.5
- **Language**: Dart 3.5.4
- **State Management**: Provider pattern
- **Navigation**: GoRouter for declarative routing
- **UI Components**: Material Design 3

### **Backend & Database**
- **Backend**: Supabase (PostgreSQL)
- **Authentication**: Supabase Auth
- **Real-time Data**: Supabase Realtime
- **File Storage**: Supabase Storage

### **AI & Machine Learning**
- **ML Framework**: TensorFlow Lite
- **Image Processing**: Camera plugin with ML integration
- **Model Format**: .tflite models for on-device inference

### **External Services**
- **Weather API**: OpenWeatherMap integration
- **Location Services**: Geolocator for GPS functionality
- **Permissions**: Camera, location, and storage permissions


## 🚀 Installation & Setup

### **1. Clone the Repository**
```bash
git clone <repository-url>
cd plant_ai_disease_flutter
```

### **2. Install Flutter Dependencies**
```bash
flutter pub get
```

### **3. Environment Configuration**
Create a `.env` file in the root directory based on `.env.example`:
```bash
cp .env.example .env
```

Edit the `.env` file with your configuration:
```env
# Supabase Configuration
SUPABASE_URL=your_supabase_project_url
SUPABASE_ANON_KEY=your_supabase_anon_key

# Weather API Configuration
OPENWEATHER_API_KEY=your_openweather_api_key

# App Configuration
APP_NAME=Plant AI Disease Detection
DEBUG_MODE=true
```

### **4. TensorFlow Lite Models Setup**
Place your trained `.tflite` model files in the `assets/models/` directory:
```
assets/
  models/
    plant_disease_model.tflite
    labels.txt
```

### **5. Database Setup (Supabase)**
1. Create a new Supabase project
2. Run the SQL setup script: `supabase_setup.sql`
3. Configure Row Level Security (RLS) policies
4. Update your `.env` file with Supabase credentials

### **6. Verify Installation**
Check that Flutter is properly configured:
```bash
flutter doctor
```

## 📁 Project Structure

```
plant_ai_disease_flutter/
├── lib/
│   ├── core/                          # Core functionality
│   │   ├── config/                    # Configuration files
│   │   ├── providers/                 # State management
│   │   ├── services/                  # Business logic services
│   │   ├── theme/                     # App theming
│   │   └── utils/                     # Utility functions
│   ├── features/                      # Feature modules
│   │   ├── ai_scan/                   # AI disease detection
│   │   ├── auth/                      # Authentication
│   │   └── home/                      # Home & plant library
│   ├── navigation/                    # App routing
│   ├── shared/                        # Shared components
│   │   └── widgets/                   # Reusable widgets
│   └── main.dart                      # App entry point
├── assets/                            # Static assets
│   ├── images/                        # Image assets
│   ├── models/                        # ML models
│   └── icons/                         # App icons
├── android/                           # Android-specific code
├── ios/                               # iOS-specific code
├── test/                              # Unit and widget tests
├── .env.example                       # Environment template
├── pubspec.yaml                       # Dependencies
└── README.md                          # This file
```


**Made with ❤️ for farmers and gardeners worldwide** 🌱
