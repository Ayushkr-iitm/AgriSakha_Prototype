# AgriSakha AI - Farmer Assistance System

## Project Structure

```bash
AgriSakha-Prototype/
├── voice_ai/                   # Voice interaction system
│   ├── core.py                 # Main voice processing logic
│   └── requirements.txt        # Python dependencies for voice AI
├── credit_scoring/             # Financial services module
│   ├── engine.py               # Credit scoring algorithms
│   └── blockchain.py           # Hyperledger Fabric integration mock
├── edge_computing/             # Field data processing
│   ├── soil.py                 # Soil analysis algorithms
│   └── requirements.txt        # Edge computing dependencies
├── data/                       # Storage for datasets (currently empty)
├── docs/                       # Documentation
│   ├── INSTALL.md              # Setup and installation guide
│   └── DEMO.md                 # Demonstration scenarios
└── README.md                   # Project overview (this file)

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
