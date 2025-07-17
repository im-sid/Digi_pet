# Digital Pet Project

![Digital Pet Project Banner](https://placehold.co/1200x400/6366f1/ffffff?text=Digital+Pet+Project&font=lato)

A web-based application where you can adopt, raise, and breed your own unique virtual pet. This prototype explores a full lifecycle for digital companions, from birth and growth to an unpredictable end, all powered by modern web technologies and a touch of AI.

---

## 📜 Table of Contents

- [Project Overview](#-project-overview)
- [✨ Key Features](#-key-features)
- [🤖 How It Works](#-how-it-works)
- [🛠️ Tech Stack](#️-tech-stack)
- [🚀 Getting Started](#-getting-started)
- [⚠️ Prototype Limitations](#️-prototype-limitations)
- [🔮 Future Enhancements](#-future-enhancements)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## 📖 Project Overview

The **Digital Pet Project** offers a unique take on the virtual pet experience. Each user account is home to a single pet, fostering a one-on-one bond. Pets evolve through three life stages—**Kid, Young, and Mature**—based on your interactions. Feeding and playing with your pet awards Experience Points (XP), driving its growth. A special **Emotional Bond Meter** tracks your connection, and once a certain threshold is reached, you can chat with your pet, with its personality and responses powered by AI.

![A happy pixel art pet on a screen](https://placehold.co/600x400/34d399/1f2937?text=A+happy+pixel+art+pet+wagging+its+tail&font=lato)

Pets have unique genetic traits that influence their appearance. When mature pets breed, an AI determines the offspring's characteristics based on its parents' genes. After a long and happy life (Level 60+), pets will face an unpredictable death, allowing the user to adopt a new companion and start a new journey. This prototype is built entirely on free-tier services to demonstrate the concept without incurring costs.

---

## ✨ Key Features

- **One Pet Per Account**: Fosters a strong, singular bond between the user and their digital companion.
- **Level-Based Evolution**: Pets progress through **Kid (Lv 1-15)**, **Young (Lv 16-30)**, and **Mature (Lv 31+)** stages by gaining XP from interactions.
- **Emotional Bond Meter**: Unlock an **AI-powered chat** with your pet by building a strong bond through care and play.
- **Genetic System**: Pets possess unique genes (color, ears, patterns) that define their appearance.
- **AI-Driven Breeding**: Mature pets (Lv 31+) can breed. **Gemini AI** determines the offspring's traits by combining parental genes.
- **Unpredictable Lifecycle**: Pets reaching Level 60+ face a random, unpredictable death, creating a realistic and meaningful lifecycle.
- **Social Interaction**: Visit other users' pets and engage in joint activities.
- **Customization**: Personalize your pet's environment with different backgrounds and equip them with fun accessories.

---

## 🤖 How It Works

1.  **Adoption**: New users sign up via Google OAuth. You can take an optional personality quiz to get a pet recommendation (Cat, Dog, Bird, or Turtle) or choose one directly. A breed is then randomly assigned.
2.  **Care & Growth**: You raise your pet by **feeding** it and **playing** with toys. Each action grants XP and Bond Points.
    - **XP** levels up your pet, advancing it through life stages.
    - **Bond Points** increase your connection. At 50 points, the AI chat feature unlocks.
    - **Neglect** (24 hours of no interaction) will result in a small loss of XP and Bond Points.
3.  **Breeding**: Once your pet reaches the **Mature** stage (Level 31+), you can list it in a public breeding pool or select a partner from the pool. The AI then generates a unique offspring based on the parents' genetic traits.
4.  **End of Life**: After reaching Level 60, your pet has a small, random chance of passing away each day. You'll be notified when this happens, and its data will be archived, allowing you to adopt a new pet and begin again.

---

## 🛠️ Tech Stack

-   **Frontend**: React (via CDN) & Tailwind CSS
-   **Backend**: Node.js & Express
-   **Database**: MongoDB
-   **Authentication**: Firebase Authentication (Google OAuth)
-   **AI Integration**: Google Gemini AI
-   **Deployment**: Vercel (Frontend) & Render (Backend)
-   **Design Tools**: Aseprite / Krita (for sprites)

---

## 🚀 Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

-   Node.js and npm installed.
-   A Google Firebase project for authentication.
-   A MongoDB Atlas account for the database.
-   A Google AI Studio API key for Gemini.

### Installation

1.  **Clone the repo**
    ```sh
    git clone [https://github.com/your-username/digital-pet-project.git](https://github.com/your-username/digital-pet-project.git)
    ```
2.  **Install NPM packages** for the backend
    ```sh
    cd digital-pet-project/backend
    npm install
    ```
3.  **Create a `.env` file** in the `backend` directory and add the following environment variables:
    ```env
    MONGO_URI=your_mongodb_connection_string
    FIREBASE_API_KEY=your_firebase_api_key
    GEMINI_API_KEY=your_gemini_api_key
    ```
4.  **Start the backend server**
    ```sh
    npm start
    ```
5.  **Open the frontend `index.html`** file in your browser to view the application.

---

## ⚠️ Prototype Limitations

This project is a prototype and operates under the constraints of free-tier services:
-   **Backend Hosting**: The Render free tier may cause the server to spin down after a period of inactivity, leading to a slow initial load time.
-   **Database & Storage**: MongoDB (512 MB) and Vercel (100 MB) have limited storage.
-   **AI API Calls**: The use of Gemini AI is limited to 1,500 requests per day.
-   **Scalability**: The current setup is designed for a small user base (~10-20 concurrent users) for testing and demonstration.
-   **Simulated Payments**: Premium features are for demonstration only and do not involve real transactions.

---

## 🔮 Future Enhancements

-   **Monetization**: Implement a real payment system for premium items and cosmetics.
-   **Scalability**: Upgrade to paid service tiers to support a larger user base.
-   **Enhanced AI**: Utilize more advanced AI models for richer pet personalities, dynamic interactions, and more complex genetic inheritance.
-   **More Pet Types**: Introduce new species and breeds for users to adopt.

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
