# 🌍 SI-KLOP: Neon Encyclopedia - Interactive Learning Platform

<div align="center">

![Neon Encyclopedia](https://images.unsplash.com/photo-1451187580459-43490279c0fa?w=1200&h=400&fit=crop)

**A vibrant, gamified encyclopedia app designed for Indonesian students (SD-SMA)**

[Features](#-features) • [Tech Stack](#-tech-stack) • [Getting Started](#-getting-started) • [Documentation](#-documentation) • [Contributing](#-contributing)

[![Next.js](https://img.shields.io/badge/Next.js-14-black?style=flat-square&logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?style=flat-square&logo=typescript)](https://www.typescriptlang.org/)
[![TailwindCSS](https://img.shields.io/badge/Tailwind-3-38bdf8?style=flat-square&logo=tailwindcss)](https://tailwindcss.com/)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)

</div>

---

## 📖 About

**SI KLOP** is an interactive, gamified learning platform that combines education with engagement. Built specifically for Indonesian students from primary to high school (SD-SMA), it features a stunning neon-cyber aesthetic with comprehensive content about world geography, Indonesian culture, vocabulary building, and AI-powered learning assistance.

### 🎯 Mission

To make learning fun, engaging, and accessible through gamification, visual content, and interactive features that keep students motivated and coming back daily.

---

## ✨ Features

### 🌏 Core Content

- **🗺️ World Explorer**
  - 100+ countries across all continents
  - Cultural information, cuisine, landmarks
  - Language, currency, and interesting facts
  - Search and filter by continent
  - Beautiful imagery for each country

- **🇮🇩 Indonesia Deep Dive**
  - All 38 provinces with complete details
  - Traditional clothing (pakaian adat)
  - Traditional houses (rumah adat)
  - Local cuisine and cultural facts
  - Regional filtering system

- **📚 Academic Vocabulary**
  - 150+ words for SD-SMA levels
  - Etymology and word history
  - Example sentences and synonyms
  - Pronunciation guides (EN/ID)
  - Categorized by subject areas

- **💡 Fun Facts**
  - 45+ fascinating facts
  - Categories: World, Indonesia, Geography
  - Scientific explanations
  - Educational and entertaining

### 🎮 Gamification System

- **⭐ Level & XP System**
  - 15 progressive levels (Beginner Explorer → Legendary Scholar)
  - Earn XP from every activity
  - Visual progress tracking
  - Level-based achievements

- **🏅 Badge Collection**
  - 30+ unique badges to unlock
  - Multiple rarity tiers (Common → Legendary)
  - Categories: Exploration, Learning, Quiz, Streak, Special
  - Real-time achievement notifications

- **🔥 Daily Streaks**
  - Track consecutive learning days
  - Streak bonuses and multipliers
  - Motivational milestone badges
  - Auto-reset at midnight

- **🎯 Daily Challenges**
  - 3 fresh challenges every day
  - Quiz, Exploration, and Vocabulary tasks
  - Bonus XP rewards
  - Countdown timers

### 💾 Retention Features

- **❤️ Bookmarks System**
  - Save favorite countries, provinces, facts, vocabulary
  - Quick access to saved content
  - Organized by category
  - One-click bookmark management

- **📊 Progress Tracker**
  - Comprehensive learning analytics
  - Countries visited & provinces explored
  - Quiz history with scores and dates
  - Total learning time tracking
  - Visual progress bars

- **📜 Learning History**
  - Complete activity log
  - Timestamped entries
  - Filter by activity type
  - Export capabilities

### 🏆 Social & Competition

- **🥇 Global Leaderboard**
  - Top 100 rankings by XP
  - User avatars and titles
  - Achievement counts display
  - Real-time rank updates

- **🤝 Share Progress**
  - Share achievements to social media
  - Copy progress summary to clipboard
  - Shareable rank cards
  - Motivate friends to join

### 🤖 AI-Powered Learning

- **💬 AI Assistant**
  - Powered by Perplexity AI
  - Deep learning conversations
  - Context-aware responses
  - Clean, markdown-free formatting
  - Credit-based usage system

### 🎲 Interactive Learning

- **📝 Quiz System**
  - 10 random questions per quiz
  - Multiple choice format
  - Instant scoring and feedback
  - XP rewards for performance
  - Quiz history tracking

---

## 🛠️ Tech Stack

### Frontend
- **Framework**: [Next.js 14](https://nextjs.org/) (App Router)
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/)
- **UI Components**: [shadcn/ui](https://ui.shadcn.com/)
- **Icons**: [Lucide React](https://lucide.dev/)
- **Animations**: CSS Transitions & Tailwind

### Backend & APIs
- **AI**: [Perplexity API](https://www.perplexity.ai/)
- **Images**: [Unsplash](https://unsplash.com/)
- **Avatars**: [DiceBear API](https://www.dicebear.com/)
- **API Proxy**: Custom Next.js API Route

### Data & State
- **Storage**: LocalStorage (browser-based)
- **State Management**: React Hooks (useState, useEffect)
- **Data Persistence**: Custom storage utilities

### Design System
- **Theme**: Neon Cyber Aesthetic
- **Colors**: Vibrant neons (cyan, purple, green, pink)
- **Typography**: System fonts optimized for readability
- **Responsive**: Mobile-first design

---

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ installed
- npm or yarn package manager
- Perplexity API key (for AI Assistant feature)

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/neon-encyclopedia.git
cd neon-encyclopedia
```

2. **Install dependencies**
```bash
npm install
# or
yarn install
```

3. **Configure API Keys**

The Perplexity API key is hardcoded in `src/components/AIAssistant.tsx`. To use your own key:

Open `src/components/AIAssistant.tsx` and update the API key:
```typescript
const apiKey = 'YOUR_PERPLEXITY_API_KEY_HERE';
```

4. **Run development server**
```bash
npm run dev
# or
yarn dev
```

5. **Open your browser**
```
http://localhost:3000
```

### Build for Production

```bash
npm run build
npm start
# or
yarn build
yarn start
```

---

## 📂 Project Structure

```
neon-encyclopedia/
├── src/
│   ├── app/
│   │   ├── api/
│   │   │   └── proxy/
│   │   │       └── route.ts          # API proxy for external requests
│   │   ├── layout.tsx                # Root layout with metadata
│   │   └── page.tsx                  # Main app with routing logic
│   │
│   ├── components/
│   │   ├── ui/                       # shadcn/ui components
│   │   │   ├── button.tsx
│   │   │   ├── card.tsx
│   │   │   ├── input.tsx
│   │   │   └── ...
│   │   │
│   │   ├── AIAssistant.tsx           # Perplexity AI chat interface
│   │   ├── Bookmarks.tsx             # Saved content manager
│   │   ├── DailyChallenges.tsx       # Daily tasks system
│   │   ├── Dashboard.tsx             # Main navigation hub
│   │   ├── FunFacts.tsx              # Interesting facts display
│   │   ├── Gamification.tsx          # Badges & achievements UI
│   │   ├── IndonesiaExplorer.tsx     # 38 provinces explorer
│   │   ├── Leaderboard.tsx           # Global rankings
│   │   ├── ProgressTracker.tsx       # Learning analytics
│   │   ├── Quiz.tsx                  # Interactive quiz system
│   │   ├── Vocabulary.tsx            # Academic word learning
│   │   └── WorldCountries.tsx        # 100+ countries explorer
│   │
│   └── lib/
│       ├── gamification.ts           # XP, levels, badges logic
│       ├── imageData.ts              # Image URLs for countries/provinces
│       ├── storage.ts                # LocalStorage utilities
│       └── utils.ts                  # Helper functions
│
├── public/                           # Static assets
├── README.md                         # This file
├── package.json                      # Dependencies
├── tsconfig.json                     # TypeScript config
└── tailwind.config.ts                # Tailwind CSS config
```

---

## 📚 Documentation

### Gamification System

#### XP Rewards
- **Explore Country**: +25 XP
- **Explore Province**: +25 XP
- **Bookmark Item**: +10 XP
- **Complete Quiz (60%+)**: +50 XP
- **Complete Quiz (80%+)**: +100 XP
- **Daily Challenge**: +200 XP
- **Daily Streak Bonus**: +50 XP per day

#### Level Progression
| Level | Title | XP Required |
|-------|-------|-------------|
| 1 | Beginner Explorer | 0 |
| 2 | Curious Learner | 100 |
| 3 | Knowledge Seeker | 250 |
| 5 | Quiz Master | 750 |
| 10 | Geography Expert | 3000 |
| 15 | Legendary Scholar | 10000 |

#### Badge Categories
- **Exploration**: World Tourist, Continental Explorer, Geography Legend
- **Learning**: Word Collector, Vocab Master, Polyglot
- **Quiz**: Quiz Novice, Quiz Champion, Quiz Legend
- **Streak**: Dedicated Learner, Committed Student, Unstoppable Force
- **Special**: Early Bird, Night Owl, Speed Demon, Completionist

### Storage System

All user data is stored in browser localStorage:

```typescript
// Key structure
{
  "userProgress": {
    "level": 1,
    "xp": 0,
    "streak": 0,
    "lastVisit": "2025-01-15T12:00:00Z",
    "visitedCountries": [],
    "exploredProvinces": [],
    "learnedVocabulary": [],
    "quizHistory": [],
    "totalLearningTime": 0
  },
  "bookmarks": {
    "countries": [],
    "provinces": [],
    "facts": [],
    "vocabulary": []
  },
  "achievements": [],
  "credits": 1000
}
```

### API Integration

#### Perplexity AI
```typescript
// Request format
POST /api/proxy
{
  "protocol": "https",
  "origin": "api.perplexity.ai",
  "path": "/chat/completions",
  "method": "POST",
  "headers": {
    "Authorization": "Bearer YOUR_API_KEY",
    "Content-Type": "application/json"
  },
  "body": {
    "model": "llama-3.1-sonar-small-128k-online",
    "messages": [...]
  }
}
```

### Component Usage

#### WorldCountries
```tsx
import { WorldCountries } from '@/components/WorldCountries';

<WorldCountries onBack={() => setCurrentView('dashboard')} />
```

#### Gamification
```tsx
import { Gamification } from '@/components/Gamification';

<Gamification onBack={() => setCurrentView('dashboard')} />
```

---

## 🎨 Design Guidelines

### Color Palette

```css
/* Primary Neon Colors */
--neon-cyan: #00ffff
--neon-purple: #bf00ff
--neon-green: #39ff14
--neon-pink: #ff006e
--neon-blue: #00d9ff

/* Background */
--bg-dark: #0a0a0f
--bg-darker: #050508

/* Text */
--text-light: #ffffff
--text-muted: #94a3b8
```

### Typography Scale

- **Hero**: 4xl - 5xl (36px - 48px)
- **Heading**: 2xl - 3xl (24px - 30px)
- **Subheading**: xl (20px)
- **Body**: base (16px)
- **Small**: sm (14px)

### Spacing System

Following Tailwind's spacing scale:
- **Tight**: 2, 4 (0.5rem, 1rem)
- **Normal**: 6, 8 (1.5rem, 2rem)
- **Loose**: 12, 16 (3rem, 4rem)

---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Reporting Bugs
1. Check existing issues first
2. Create detailed bug report with steps to reproduce
3. Include screenshots if applicable

### Suggesting Features
1. Open an issue with `[FEATURE]` prefix
2. Describe the feature and its benefits
3. Discuss implementation approach

### Pull Requests
1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

### Development Guidelines
- Follow TypeScript strict mode
- Use Tailwind CSS for styling
- Write clear commit messages
- Test on mobile and desktop
- Maintain neon-cyber aesthetic

---

## 🐛 Known Issues

- **LocalStorage Limitations**: Data is device-specific and will be lost if browser cache is cleared
- **Leaderboard**: Currently uses mock data, needs backend for real global rankings
- **Images**: Dependent on Unsplash CDN availability
- **AI Assistant**: Requires valid Perplexity API key with sufficient credits

---

## 🗺️ Roadmap

### Version 2.0 (Q1 2025)
- [ ] Backend database integration
- [ ] User authentication system
- [ ] Real global leaderboard
- [ ] Friend system & social features
- [ ] More quiz categories and difficulties

### Version 2.5 (Q2 2025)
- [ ] Mobile app (React Native)
- [ ] Offline mode with sync
- [ ] Audio pronunciation feature
- [ ] Video content integration
- [ ] Teacher dashboard for schools

### Version 3.0 (Q3 2025)
- [ ] Multiplayer quiz battles
- [ ] Study groups and collaboration
- [ ] Advanced analytics & AI recommendations
- [ ] Content creator platform
- [ ] Marketplace for user-generated content

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👥 Credits

### Development
- **Creator**: Built with ❤️ by [Your Name]
- **Framework**: [Next.js](https://nextjs.org/) by Vercel
- **UI Components**: [shadcn/ui](https://ui.shadcn.com/)

### APIs & Services
- **AI**: [Perplexity AI](https://www.perplexity.ai/)
- **Images**: [Unsplash](https://unsplash.com/)
- **Avatars**: [DiceBear](https://www.dicebear.com/)

### Content Sources
- Country data: Various open-source geographical databases
- Indonesia data: Curated from reliable Indonesian sources
- Fun facts: Verified educational content

### Special Thanks
- Indonesian students for inspiration
- Open-source community for amazing tools
- All contributors and supporters

---

## 📞 Contact & Support

- **GitHub**: [Repository Issues](https://github.com/mrbrightsides/si-klop/issues)
- **Email**: your.email@example.com
- **Website**: https://neon-encyclopedia.vercel.app

---

## 🌟 Star History

If you find this project useful, please consider giving it a star! ⭐

[![Star History Chart](https://api.star-history.com/svg?repos=mrbrightsides/si-klop&type=Date)](https://star-history.com/#mrbrightsides/si-klop&Date)

---

<div align="center">

**Made with 💜 for Indonesian Students**

*Learn • Play • Grow*

[⬆ Back to Top](#-neon-encyclopedia---interactive-learning-platform)

</div>

