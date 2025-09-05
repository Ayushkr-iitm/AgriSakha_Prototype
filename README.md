AgriSakha AI - A Voice-First AI Ecosystem for Indian Farmers
AgriSakha is a groundbreaking AI-powered solution designed to empower India's 120 million smallholder farmers by democratizing access to financial services, agricultural knowledge, and fair markets through a voice-first interface that works on any phone.

Table of Contents
The Challenge

Our Solution

Key Features

System Architecture

Technology Stack

Project Structure

Getting Started

Demonstration

Scalability & Impact

Contributing

License

The Challenge
Indian smallholder farmers face a triple crisis that hinders their growth and sustainability:

Financial Exclusion: 70% lack access to formal credit, making them vulnerable to predatory lending.

Market Exploitation: An estimated 30% of their income is lost to middlemen due to a lack of direct market access.

Information Gap: 40% of crop yield is wasted due to poor and untimely agricultural advisories.

Existing digital solutions often fail to reach over 80% of this demographic due to dependencies on smartphones, reliable internet, and digital literacy. AgriSakha bridges this critical gap.

Our Solution
AgriSakha is an offline-first, voice-powered ecosystem that requires no app and no digital literacy. By integrating multilingual AI, blockchain, and satellite technology, we provide a robust toolkit that runs on basic feature phones, ensuring no farmer is left behind.

Our platform uniquely combines:

Multilingual Voice AI: Supporting over 12 Indian languages and dialects for natural, intuitive interaction.

Blockchain-Powered Credit Scoring: A transparent and automated "TrustWeb" that uses satellite and on-ground data for fair credit assessment.

Satellite-Enabled Hyperlocal Advisories: Leveraging ISRO's Bhuvan satellite data to provide precise, context-aware farming advice.

Key Features
✅ Voice AI for Zero-Literacy Users: Works on basic phones via USSD/SMS/Voice. Farmers can ask for pest/disease diagnosis, get localized advice, and access market information simply by speaking in their native dialect.

✅ Financial Inclusion: An alternative credit scoring model that uses satellite crop health data, UPI transaction history, and peer-validated reputation to provide credit to unbanked farmers.

✅ Decentralized Marketplace: A voice-based commerce protocol where farmers can connect directly with buyers, get fair prices negotiated by AI, and view transparent transaction logs on a blockchain.

✅ Offline-First Capability: An edge computing layer powered by Raspberry Pi allows the system to remain operational in low-connectivity areas, syncing data when a connection becomes available.

✅ Hyperlocal Alerts & Advisories: Provides real-time mandi prices, 72-hour advance weather warnings, and crowdsourced, cost-effective remedies for crop issues.

System Architecture
Our solution is built on a resilient, hybrid cloud/edge architecture designed for low-connectivity environments.

Farmer-Facing Layer:

Input: Interacts with farmers via USSD menus, voice calls (using IndicWhisper ASR), and IoT soil sensors.

Output: Delivers responses via synthesized voice (Mozilla TTS) and structured SMS alerts (e.g., credit score, market prices).

Edge Computing Layer (Offline Operation):

Hardware: Local hubs with Raspberry Pi 4 clusters are deployed at FPO (Farmer Producer Organization) offices.

Function: Runs TensorFlow Lite models for on-device pest classification and yield prediction. It stores up to 7 days of interactions locally and batch-uploads data when connectivity is restored.

Core AI Processing Layer:

A suite of modular microservices for handling core logic:

CreditAI: Performs dynamic credit scoring using satellite data.

AgriBot: A Q&A engine powered by IndicBERT.

Market Matcher: Manages voice-based commerce and negotiations.

Blockchain & Data Layer:

Network: A private Hyperledger Fabric network with nodes managed by banks, FPOs, and government agencies.

Smart Contracts: Manage peer reputation (Vouch.sol) and update credit scores (CreditScore.sol).

Data Sources: Integrates with public datasets from ISRO Bhuvan, e-NAM, and Soil Health Cards, alongside private, encrypted farmer transaction data.

Technology Stack
Category

Technologies

Core AI/ML

IndicTrans (AI4Bharat), TensorFlow Lite, Dalex.ai, LightGBM, PyTorch

Voice Processing

Mozilla TTS, IndicWhisper (Fine-tuned Whisper), Vosk ASR

Data Infrastructure

Hyperledger Fabric, Apache Kafka

Edge Computing

Raspberry Pi OS, TensorFlow.js, OpenCV

Agricultural ML

GeoPy, AgriML (Custom Fork)

Gateways

KooKoo SMS Gateway, Asterisk PBX

Project Structure
AgriSakha-Prototype/
│
├── voice_ai/               # Voice interaction system
│   ├── core.py             # Main voice processing logic
│   └── requirements.txt    # Python dependencies for voice AI
│
├── credit_scoring/         # Financial services module
│   ├── engine.py           # Credit scoring algorithms
│   └── blockchain.py       # Hyperledger Fabric integration mock
│
├── edge_computing/         # Field data processing
│   ├── soil.py             # Soil analysis algorithms
│   └── requirements.txt    # Edge computing dependencies
│
├── data/                   # Storage for datasets (currently empty)
│
├── docs/                   # Documentation
│   ├── INSTALL.md          # Setup and installation guide
│   └── DEMO.md             # Demonstration scenarios
│
└── README.md               # Project overview (this file)

Getting Started
Follow the instructions in docs/INSTALL.md to set up the project environment. A brief overview is provided below.

Prerequisites
Python 3.8+

Raspberry Pi 4 (for edge computing module)

Basic knowledge of Docker (for Hyperledger)

Installation
Clone the repository:

git clone [https://github.com/Ayushkr-iitm/AgriSakha_Prototype.git](https://github.com/Ayushkr-iitm/AgriSakha_Prototype.git)
cd AgriSakha_Prototype

Install dependencies for each module separately. For the voice AI module:

cd voice_ai
pip install -r requirements.txt

Repeat the installation process for credit_scoring and edge_computing modules.

Demonstration
For a complete guide on running demonstration scenarios, please refer to the docs/DEMO.md file.

You can also watch a video demonstration of the prototype here:
Demo Video Link

Scalability & Impact
Our model is designed for massive, low-cost scalability, with a vision to onboard millions of farmers across India.

Challenge

Our Solution

Projected Improvement

Credit Access

Alternative Scoring

▼ 65% in loan rejections

Middlemen Exploitation

Direct Negotiations

▲ 30% in farmer income

Crop Losses

Precision Advisories

▼ 50% in crop waste

Input Costs

Localized Recs

▼ 40% in farm expenses

The system leverages government synergy by building on IndiaStack (Aadhaar, UPI) and is designed for community ownership where FPOs manage local nodes.

Contributing
We welcome contributions! Please feel free to submit a pull request or open an issue to discuss your ideas.
