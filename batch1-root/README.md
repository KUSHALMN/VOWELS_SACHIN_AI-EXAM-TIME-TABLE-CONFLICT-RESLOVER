# 🎓 AI Exam Timetable Conflict Resolver

**Hackathon Project**: AI-powered system to detect and automatically resolve exam scheduling conflicts with smart optimization algorithms.

## 🚀 Live Demo URLs

- **Frontend**: http://localhost:5173
- **Backend**: http://localhost:3001

## ⚡ Quick Setup (2 Minutes)

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn

### 1. Clone Repository
```bash
git clone https://github.com/YOUR_USERNAME/ai-exam-timetable-conflict-resolver.git
cd ai-exam-timetable-conflict-resolver
```

### 2. Install Dependencies
```bash
# Install backend dependencies
npm install

# Install frontend dependencies
cd client
npm install
cd ..
```

### 3. Start the Application
```bash
# Terminal 1 - Start Backend Server
npm run dev

# Terminal 2 - Start Frontend (in new terminal)
cd client
npm run dev
```

### 4. Access Application
- Open browser: http://localhost:5173
- Backend API: http://localhost:3001

## 🎯 Instant Testing for Judges

### No Manual Setup Required!
1. **Click "Quick Test Scenarios"** in any section
2. **Select any demo scenario** (No Conflicts, Room Conflicts, etc.)
3. **Click "CLICK ME TO GET DATA"** buttons
4. **Run analysis** instantly

### Test Flow:
```
Upload Timetable → Load Demo Data → Detect Conflicts → Auto-Resolve → Download CSV
```

## ✨ Key Features

- ✅ **AI Conflict Detection**: 10+ conflict types (Room, Faculty, Time, Capacity)
- 🤖 **Auto-Resolution**: Greedy algorithm optimization
- 📊 **Multi-Branch Analysis**: Cross-department conflict detection  
- 🎨 **Modern UI**: React + Tailwind with animations
- 📥 **CSV Import/Export**: Upload and download timetables
- ⚡ **Instant Demo Data**: Built-in test scenarios
- 🔄 **Real-time Updates**: Live conflict detection

## 🛠️ Tech Stack

| Component | Technology |
|-----------|------------|
| Frontend | React 18, Vite, Tailwind CSS |
| Backend | Node.js, Express |
| File Processing | Multer, CSV Parser |
| AI Integration | Gemini API |
| Animations | CSS Animations, Tailwind |

## 📁 Project Structure

```
├── client/                 # React Frontend
│   ├── src/
│   │   ├── components/     # UI Components
│   │   ├── data/          # Demo data & cache
│   │   ├── pages/         # Login & Dashboard
│   │   └── utils/         # Helper functions
├── server.js              # Node.js Backend
├── utils/                 # Conflict detection logic
├── sample-data/           # Test CSV files
└── package.json           # Dependencies
```

## 🎪 Demo Scenarios Available

| Scenario | Description | Expected Conflicts |
|----------|-------------|-------------------|
| ✅ No Conflicts | Clean timetable | 0 conflicts |
| ⚠️ Room Conflicts | Same room overlaps | 2 conflicts |
| 🔥 Multi Conflicts | Room + Faculty issues | 3 conflicts |
| 🎯 Perfect Schedule | Optimized timetable | 0 conflicts |

## 🔧 Available Scripts

### Backend
```bash
npm run dev          # Start development server
npm start           # Start production server
```

### Frontend
```bash
cd client
npm run dev         # Start development server
npm run build       # Build for production
npm run preview     # Preview production build
```

## 📋 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/upload` | Upload CSV timetable |
| POST | `/detect-conflicts` | Analyze conflicts |
| POST | `/resolve` | Auto-resolve conflicts |
| POST | `/detect-multibranch-conflicts` | Cross-branch analysis |

## 🎯 Usage Guide

### 1. Upload Timetable
- Use "Upload Timetable" section
- Click demo scenarios or upload CSV
- Required columns: `subject_name, department, date, start_time, end_time, room_no, faculty_id, student_group`

### 2. Detect Conflicts
- Go to "AI Conflict Detection"
- Load demo data or use uploaded timetable
- Click "Run AI Conflict Check"

### 3. Multi-Branch Analysis
- Use "Multi-Branch Analyzer"
- Compare multiple department timetables
- Detect cross-department conflicts

### 4. Auto-Resolution
- Use "AI Auto-Resolution"
- Automatically fix detected conflicts
- Download optimized timetable

## 🏆 Hackathon Highlights

- **2-minute setup** with instant demo data
- **No manual CSV creation** required
- **Full AI pipeline** demonstration
- **Professional UI** with animations
- **Cross-platform** compatibility
- **Judge-friendly** with clear instructions

## 🐛 Troubleshooting

### Port Already in Use
```bash
# Kill processes on ports
npx kill-port 3001 5173
```

### Dependencies Issues
```bash
# Clear cache and reinstall
rm -rf node_modules package-lock.json
npm install
```

### Demo Data Not Loading
- Refresh the page
- Check browser console for errors
- Ensure both servers are running



---

**Made for Hackathon Judges** 🏆 | **Ready to Test in 2 Minutes** ⚡

**Quick Start**: Clone → `npm install` → `npm run dev` → Open http://localhost:5173 → Click "Quick Test Scenarios"