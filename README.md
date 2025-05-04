# AgriSakha AI - Farmer Assistance System

AgriSakha-Prototype/
├── voice_ai/
│   ├── core.py                 # Main voice processing
│   └── requirements.txt        # voice_ai specific deps
├── credit_scoring/
│   ├── engine.py               # Credit scoring logic
│   └── blockchain.py           # Hyperledger mock
├── edge_computing/
│   ├── soil.py                 # Soil analysis
│   └── requirements.txt        # Edge deps
├── data/                       # (Empty - for your datasets)
├── docs/
│   ├── INSTALL.md              # Setup instructions
│   └── DEMO.md                 # How to test
└── README.md                   # Project overview

An AI-powered solution for Indian farmers providing:
- Voice-based agricultural advisory in 12+ Indian languages
- Blockchain-based credit scoring using satellite data
- Edge-computing enabled soil health analysis

## Key Features
✅ **Voice AI** - Works on basic phones via USSD/SMS/Voice  
✅ **Financial Inclusion** - Alternative credit scoring for unbanked farmers  
✅ **Localized Advice** - Crop/location-specific recommendations  
✅ **Offline Capable** - Raspberry Pi integration for low-connectivity areas  

## Technology Stack
- **Voice Processing**: Mozilla TTS + Vosk ASR
- **AI/ML**: TensorFlow Lite, IndicWhisper
- **Blockchain**: Hyperledger Fabric (mock)
- **Edge Computing**: Raspberry Pi + IoT sensors

[Demo Video](https://example.com/demo) | [Technical Documentation](docs/ARCHITECTURE.md)
