# Exam-prep
# CNIP Master Portal - Liquid Glass Edition

A modern, interactive quiz application for Computer Networks and Internet Protocols (CNIP) exam preparation featuring liquid glass morphism UI, 3D interactions, and adaptive learning modes.

![Version](https://img.shields.io/badge/version-2.0-blue)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## ✨ Features

### Core Functionality
- **11 Week Coverage**: Complete curriculum from Week 1 (TCP/IP basics) to Week 11 (DHCP/ARP)
- **110 Questions**: Comprehensive question bank with detailed explanations
- **Session Tracking**: Real-time score calculation and progress monitoring
- **Review System**: Post-quiz analysis with correct answers and explanations

### New: Randomization Mode 🎲
- **Shuffle Questions**: Questions appear in random order after selecting a week
- **Fair Distribution**: Ensures all questions from selected week are covered exactly once
- **Anti-Cheating**: Prevents pattern recognition for repeated attempts
- **Persistent Logic**: Maintains correct answer mapping regardless of shuffle

### UI/UX Features
- **Liquid Glass Design**: Frosted glass panels with backdrop blur and ambient lighting
- **3D Tilt Cards**: Mouse-tracking parallax effects on week selection cards
- **Animated Transitions**: Smooth view switching with fade and blur effects
- **Confetti Celebration**: Particle effects for high scores (≥80%)
- **Dark Mode**: Premium dark theme with neon accents
- **Responsive Design**: Optimized for desktop, tablet, and mobile

## 🚀 Getting Started

### Installation
1. Download `cnip-portal.html` to your local machine
2. Open directly in any modern browser (Chrome, Firefox, Safari, Edge)
3. No server or internet connection required after download

### Usage

#### Starting a Quiz
1. **Select Week**: Click on any week card (Week 1-11) from the dashboard
2. **Question Randomization**: Questions automatically shuffle when the quiz starts
3. **Answer Selection**: Click on options A, B, C, or D
   - Green glow = Correct answer
   - Red shake = Wrong answer (correct option highlighted)
4. **Navigation**: Click "Next Question" to proceed
5. **Completion**: View score, percentage, and detailed review

#### Scoring System
- **Outstanding (80-100%)**: Confetti celebration + "Outstanding!" badge
- **Good (60-79%)**: "Good job!" encouragement
- **Practice Needed (&lt;60%)**: "Keep practicing!" motivation with review suggestions

## 🛠️ Technical Details

### File Structure
cnip-portal/
├── cnip-portal.html      # Single-file application (HTML+CSS+JS)
└── README.md             # This documentation file


### Browser Compatibility
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- Mobile browsers (iOS Safari, Chrome Mobile)

### Performance Specs
- **Load Time**: <500ms (local file)
- **Animations**: 60fps CSS transforms
- **Memory Usage**: ~15MB (question bank loaded in memory)
- **Offline Capable**: 100% functional without internet

## 🎨 Customization

### Adding New Questions
Edit the `database` object in the `<script>` section:

```javascript
"Week 12": [
    {
        q: "Your question here?",
        a: ["Option A", "Option B", "Option C", "Option D"],
        c: 0,  // Index of correct answer (0-based)
        s: "Explanation text here"
    }
]

| Key     | Action                          |
| ------- | ------------------------------- |
| `1-4`   | Select answer option (A-D)      |
| `Enter` | Next question / Submit          |
| `R`     | Reload page (back to dashboard) |
| `Space` | Pause timer (if implemented)    |



