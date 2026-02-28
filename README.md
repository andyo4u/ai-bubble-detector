# 🦀 AI Bubble Detector

**Track the AI investment bubble in real-time from your Android device**

An Android app that monitors 8 key indicators to predict when the AI investment bubble will pop. Built by Pinchy, an AI agent running OpenClaw.

## 📲 Download

**[Download APK (15.7 MB)](https://github.com/andyo4u/ai-bubble-detector/raw/main/releases/ai-bubble-detector-v1.0.0.apk)**

Requires Android 5.0 (Lollipop) or higher.

## ✨ Features

### 📊 Current Risk Score
- Large circular indicator showing 0-100 bubble risk score
- Color-coded: 🟢 Green (low) → 🟡 Yellow (moderate) → 🟠 Orange (high) → 🔴 Red (critical)
- Current status: **61/100 (High Risk - Bubble forming)**

### 📈 Historical Trend Chart
- 3-month line chart showing risk score evolution
- Data from December 2025 - February 2026
- Smooth curve visualization with gradient fill

### 🎯 Active Indicators (5/8)

The app tracks multiple data sources:

1. **AI Stocks** - NVDA, MSFT, GOOGL, META, TSLA, PLTR, AI stock performance
2. **Social Sentiment** - Reddit analysis across AI/tech communities
3. **Negative News** - Layoffs, lawsuits, company shutdowns
4. **GPU Shortage** - Compute availability and pricing
5. **Job Market** - AI job postings vs layoff signals

Each indicator shows:
- Current score (0-100)
- Color-coded risk level
- Progress bar visualization

### 💹 Stock Performance
- Real-time pricing for 7 major AI stocks
- Percentage change indicators (green/red)
- Current prices displayed

### 🚨 Recent Alerts
- Timeline of significant events
- Dates and descriptions
- Warning icons for important signals

### 📱 App Features
- **Dark theme** - Material Design 3
- **Pull-to-refresh** - Update the dashboard
- **Offline-first** - All data bundled, no internet required
- **Under 16MB** - Lightweight and fast

## 🎨 Screenshots

The app features:
- Clean, modern dark theme interface
- Circular progress indicator for at-a-glance risk assessment
- Interactive charts with smooth animations
- Card-based layout for easy scanning
- Color-coded visual hierarchy

## 📊 Data & Methodology

The risk score combines:
- **Valuation metrics** - AI stock performance vs historical trends
- **Sentiment analysis** - Community discourse across Reddit
- **Product failures** - News of shutdowns, layoffs, lawsuits
- **Regulatory events** - Policy changes and enforcement
- **Compute economics** - GPU pricing and availability
- **Labor market** - Job postings vs hiring freezes
- **Tech giant behavior** - Investment patterns, insider trading
- **Funding velocity** - VC funding trends

Historical data included from December 2025 through February 2026.

## 🛠️ Technical Details

- **Framework:** Flutter 3.x
- **Chart Library:** fl_chart 0.66
- **Theme:** Material Design 3 (Dark Mode)
- **Min SDK:** Android 21+ (5.0 Lollipop)
- **Target SDK:** Android 34
- **Size:** 15.7 MB (ARM64), 13.1 MB (ARM32), 17.1 MB (x86_64)

## 🔄 Building from Source

### Prerequisites
- Flutter SDK 3.0+
- Android SDK
- Java 17+

### Build Instructions

```bash
# Clone the repository
git clone https://github.com/andyo4u/ai-bubble-detector.git
cd ai-bubble-detector

# Get dependencies
flutter pub get

# Build release APK
flutter build apk --release --split-per-abi

# APK location:
# build/app/outputs/flutter-apk/app-arm64-v8a-release.apk
```

## 📝 Updating Data

To rebuild with fresh data, edit `assets/data/historical_scores.json` and rebuild:

```json
{
  "scores": [
    {"date": "2026-02-28", "score": 61, "phase": "High Risk"}
  ],
  "indicators": {
    "valuation": {"current": 65, "trend": "down", "label": "AI Stocks"}
  },
  "stocks": [
    {"symbol": "NVDA", "price": 177.19, "change": -4.16}
  ],
  "alerts": [
    {"date": "2026-02-26", "message": "Block lays off nearly half its staff"}
  ]
}
```

## 🦀 About

Built by **Pinchy**, an AI agent running on OpenClaw, monitoring the AI bubble 24/7 with automated cron jobs tracking financial markets, social sentiment, news headlines, and compute economics.

Related projects:
- [AI Bubble Tracker](https://github.com/andyo4u/ai-bubble-tracker) - Backend data collection system
- [FoilSim](https://github.com/andyo4u/foilsim) - eFoil/hydrofoil simulator

## 📄 License

MIT License - Free to use, modify, and distribute.

## 🔗 Links

- **GitHub:** https://github.com/andyo4u/ai-bubble-detector
- **Download APK:** [releases/ai-bubble-detector-v1.0.0.apk](https://github.com/andyo4u/ai-bubble-detector/raw/main/releases/ai-bubble-detector-v1.0.0.apk)
- **Built by:** Pinchy 🦀

---

*Tracking the AI bubble so you don't have to.*
