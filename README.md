# SoilMinds - Sustainable Agriculture Assistant (SDG 15)

<p align="center">
  <img src="public/icon.png" alt="SoilMinds Logo" width="150">
</p>

<p align="center">
  <strong>Nurturing Tomorrow's Harvest Today</strong>
</p>

## Table of Contents
- [About the Project](#-about-the-project)
- [Key Features](#-key-features)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Usage](#-usage)
- [Future Scope](#-future-scope)

---

## About the Project

**SoilMinds** is a web application developed to assist farmers in making informed agricultural decisions.  
By blending technology with the art of cultivation, this project aims to address the challenges farmers face in selecting suitable crops and identifying the right fertilizers for their specific soil conditions.

The project aligns with **SDG 15** (Life on Land) by promoting sustainable agriculture and optimizing resource usage.

## Key Features

* **Precision Crop Recommendation:** Develops a predictive model that analyzes soil properties including Nitrogen (N), Phosphorus (P), Potassium (K), Temperature, Humidity, pH, and Rainfall to recommend the most suitable crop.
* **Fertilizer Insights:** Creates a model that suggests appropriate pesticides/fertilizers based on the identified crops and prevailing environmental conditions.
* **Interactive 3D Elements:** Includes 3D model integration for an engaging user experience, utilizing GLTF assets.
* **User-Friendly Interface:** Boasts an intuitive interface designed for every farmer, allowing effortless navigation regardless of technical expertise.

## Technologies Used

* **Frontend:** React.js, JavaScript, CSS.  
  * *React Router* for navigation.
* **Build Tool:** Vite (configured via `vite.config.ts`).
* **Runtime:** Node.js (Runtime environment for executing JavaScript).
* **Algorithm:** Decision Tree Logic (Used for crop recommendation based on input parameters).
* **Assets:** GLTF 3D Models, SVG Icons.

## Project Structure

Based on the project files and source organization:

```text
Soil-Minds/
├── public/
│   ├── images/
│   │   ├── crops/       # Images for Apple, Rice, Maize, etc.
│   │   └── fertilizers/ # Images for DAP, Urea, etc.
│   ├── Model/           # 3D Assets (scene.gltf, textures)
│   ├── icon.png
│   └── icon.svg
├── src/
│   ├── components/
│   │   ├── crop/        # Crop Prediction Logic & UI
│   │   ├── fertilizer/  # Fertilizer Prediction Logic & UI
│   │   ├── header/      # Navigation Bar
│   │   ├── home/        # Landing Page
│   │   └── result/      # Output Display
│   ├── App.jsx
│   ├── App.css
│   ├── index.jsx
│   └── index.css
├── package.json
└── vite.config.ts
```

## Getting Started

Follow these steps to set up the project locally.

### Prerequisites

* **Node.js** installed on your machine.

### Installation & Setup

1. **Open your terminal.**

2. **Navigate to the project directory:**

    ```bash
    cd project_folder
    ```

3. **Install dependencies:**

    ```bash
    npm install
    ```

4. **Run the development server:**

    ```bash
    npm start
    ```

5. **Access the application:**

    Open your browser and navigate to:

    ```
    http://localhost:5173/
    ```

## Usage

1. **Home:** Click "Get Started Now" to enter the application.  
2. **Crop Prediction:** Enter the soil nutrient ratios (N, P, K), environmental factors (Temperature, Humidity, Rainfall), and pH level.  
   Click **PREDICT** to see which crop is best for your land.  
3. **Fertilizer Prediction:** Navigate to the "Fertilizer Recommendation" tab.  
   Input soil details and the crop type to receive specific fertilizer advice.

## Future Scope

* **Machine Learning Integration:** Implementing Random Forest or Gradient Boosting algorithms for higher accuracy and adaptability.
* **Mobile Application:** Developing a native mobile app for easier access in rural areas using smartphones.
* **Real-time Weather:** Integrating weather forecast data to enhance the precision of recommendations.
* **Multilingual Support:** Localizing the app for diverse linguistic and cultural backgrounds.
