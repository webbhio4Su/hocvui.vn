# Project Description: AZFClip Code Generator & Scanner Web App

## Overview
This project aims to build a web-based application inspired by the **AZFClip** infographic. The core functionality combines NFC-like interaction triggers, custom visual QR code generation (reminiscent of Apple App Clip codes), and swift content redirection. The application must be cross-platform, supporting iOS, Android, and Web environments.

## Core Technical Requirements

### 1. Frontend & UI/UX Design
* **Aesthetic:** Modern, futuristic, dark mode default. 
* **Color Palette:** Deep blacks/grays for the background, with neon blue and purple gradients for accents, borders, and branding elements.
* **Layout:** A clean, responsive dashboard featuring:
  * An interactive display area for the custom circular/scannable code.
  * A sidebar or section detailing "How to Use" and "Applications" (Smart Business Cards, Check-in, Payments).
  * Input fields for alphanumeric IDs (e.g., `AZF-8A7X-K2L9`) and target URLs.

### 2. Functional Features to Implement

#### A. Code Generation Engine
* Create a component that generates a stylized, scannable code. 
* The design should feature concentric circular tracks/dashes enclosing a central logo placeholder, flanked by three distinct corner positioning squares (similar to the reference image).
* The generator should bind a unique alphanumeric asset string (e.g., `AZF-8A7X-K2L9`) to a URL payload (`azfclip.com/target`).

#### B. Scanning & Redirection Simulation
* Implement a camera-based scanner interface using web APIs (like `html5-qrcode` or WebRTC) capable of detecting and decoding the generated identifier.
* Include a simulated "NFC Touch" trigger action (e.g., a button or Web NFC API stub for compatible Android devices) that instantly parses the content.

#### C. Data Management
* A lightweight backend or local storage solution to map the unique AZFClip IDs to their respective user actions (e.g., opening a smart business card, checking into an event, or processing an offer).

---

## Instructions for Gemini Code Generation

Please generate the complete codebase or a modular prototype for this application based on the following stack preference:
* **Frontend:** [Insert your preferred framework here, e.g., React, Vue, or Vanilla HTML/CSS/JS]
* **Styling:** [Insert preference, e.g., Tailwind CSS, CSS Modules]
* **Key Libraries:** Suggest or implement appropriate libraries for QR/circular code rendering and camera scanning.

### Please provide:
1. `index.html` / Component architecture.
2. The CSS/Tailwind configuration for the neon blue/purple dark-mode aesthetic.
3. The JavaScript logic handling the generation of the unique circular layout and camera scanning parsing.
