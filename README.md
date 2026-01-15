# Career Guide (Path Forge) 🚀

**Career Guide** is a smart, AI-driven career assistance platform built to support job seekers throughout their professional journey. By combining modern AI capabilities with practical career tools, it helps users improve their resumes, prepare for interviews, and follow clear, personalised career paths toward their target roles.

![Career Guide Dashboard](https://images.unsplash.com/photo-1486312338219-ce68d2c6f44d?w=1200&h=400&fit=crop&q=80)

## ✨ Key Features

- **📄 Smart Resume Evaluation**: Upload your resume along with a job description to receive a compatibility score, skill gap insights, and clear recommendations for improvement.
- **🎙️ AI-Powered Mock Interviews**: Practice technical and behavioural interviews with an AI interviewer that mimics real hiring scenarios and provides instant feedback with suggested answers.
- **🧭 Personalised Career Roadmaps**: Interactive and visually structured learning paths based on your current skill set and long-term career goals.
- **💬 AI Career Assistant**: A round-the-clock chat assistant to answer career-related questions, guide job applications, and help users navigate the platform.
- **📈 Progress & Performance Tracking**: Monitor your resume match scores, interview performance, and growth through analytics and a gamified XP-based motivation system.
- **🔐 Secure User Profiles**: Safely store your reports, interview history, and progress while managing your professional data with confidence.

## 🛠️ Tech Stack

### Frontend

- **Framework**: React 19 (Vite)
- **Styling**: Tailwind CSS 4, Framer Motion
- **Charts**: Recharts
- **Icons**: Lucide React

### Backend

- **Runtime**: Node.js & Express.js 5
- **Database**: MongoDB (Mongoose 9)
- **AI Integration**: Groq API (Llama-3.3-70b-versatile)
- **File Processing**: PDF-Parse, Mammoth, Puppeteer (PDF Generation)
- **Authentication**: JWT & Bcrypt

## 🚀 Getting Started

Follow the steps below to run the project on your local system.

### Prerequisites

- **Node.js**: v18 or higher
- **MongoDB**: Installed locally or a cloud URI (MongoDB Atlas)
- **Groq API Key**: Get a free key from [console.groq.com](https://console.groq.com)

### Installation

1.  **Clone the Repository**

    ```bash
    git clone https://github.com/yourusername/career-guide.git
    cd career-guide
    ```

2.  **Install Dependencies**
    You need to install dependencies for both the frontend and backend.

    ```bash
    # Install Backend Dependencies
    cd backend
    npm install

    # Install Frontend Dependencies
    cd ../frontend
    npm install
    ```

### ⚙️ Environment Configuration

Create a `.env` file in the **`backend`** directory (`backend/.env`) with the following variables:

```env
# backend/.env

PORT=5000
MONGODB_URI=mongodb://localhost:27017/career_guide
# OR your MongoDB Atlas URI

JWT_SECRET=your_secure_jwt_secret_key
GROQ_API_KEY=gsk_your_groq_api_key_here
```

> **Note:** The frontend runs on Vite and typically does not need environment variables unless additional client-side configuration is required.

### ▶️ Running the Application

You need to run both the backend server and the frontend client.

1.  **Start Backend** (Terminal 1)

    ```bash
    cd backend
    npm start
    ```

    _Output should say: "Server is running on port 5000" and "MongoDB Connected"_

2.  **Start Frontend** (Terminal 2)

    ```bash
    cd frontend
    npm run dev
    ```

    _This will launch the app at `http://localhost:5173`_

3.  **Open in Browser**
    Visit `http://localhost:5173` to start using Career Guide!

## 🧪 Troubleshooting

- **"Invalid API Key" Error:**
  Ensure your `GROQ_API_KEY` in `backend/.env` is correct. If you changed it, strictly restart the backend server (`Ctrl+C` -> `npm start`).

- **Port 5000 Already in Use:**
  If you see `EADDRINUSE`, an old server process might be running. Kill it using Task Manger or `taskkill /F /IM node.exe` (Windows).

- **Database Connection Fail:**
  Ensure your local MongoDB service is running (`mongod`) or your Atlas URI is whitelisted.

## 🤝 Contributing

Contributions, improvements, and suggestions are welcome. Feel free to fork the repository and submit a Pull Request..

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
