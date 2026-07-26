# 👋 Hi, I'm Batmagnai

🇯🇵 Based in Tokyo, Japan | Bilingual (English & Intermediate Japanese)

Front-end and full-stack developer building practical web apps and AI-powered tools. Open to developer and IT support roles in Japan and remote.

Clean UI - Practical tools - Usability first.

---

## 🔍 What I Do

🎯 Building full-stack web apps with React, Next.js, and TypeScript

🤖 Engineering AI applications with Claude API, Groq API, RAG pipelines, and LLM prompt design

✨ Crafting polished UI with Framer Motion animations, custom theming systems, and responsive layouts

📌 Documenting my learning and code with clear READMEs

---

## 🚀 Projects

### 🎌 BJT Trainer - Offline-First Japanese Vocabulary Trainer

A study tool for the Business Japanese Proficiency Test (BJT) that works entirely offline - I use it daily on the commute where there is no signal.

- Built with Next.js 16 (static export), TypeScript, and Tailwind CSS
- **Audio-first recall** via the browser's native SpeechSynthesis API - speaks Japanese with zero network, no audio files
- **Leitner spaced repetition** - weak cards resurface first, and units unlock by mastery rather than on a fixed calendar
- **Two progress goals** - a unit unlock ring on the study screen and a course mastery bar tracking every card from box 1 to box 5
- **Shadowing mode** plus an installable PWA with a hand-written service worker for cache-first offline loading
- Backed by **136 unit tests** over a pure, deterministic scheduling core

💻 GitHub: https://github.com/chemicalwolf1836/bjt-trainer

---

### ✈️ Wander - AI Travel Discovery App

An AI-powered travel app that helps you find your perfect destination through natural conversation or guided prompts.

- Built with Next.js 16, TypeScript, Tailwind CSS, and Framer Motion
- **AI chat** powered by Claude - describe your trip in natural language or tap through guided choice chips
- **3 destination results** shown on an interactive Mapbox world map with animated pins and per-destination colour theming
- **3D card tilt + image parallax** - cards tilt in perspective on hover; the background photo shifts opposite for a depth illusion
- **Cinematic reveal** - cards materialise from a blur/scale stagger animation on load
- **Aurora home background** - soft animated glowing orbs react subtly to mouse position
- **Planning tools** - AI packing list, AI day-by-day itinerary, and similar destination suggestions per destination
- **Comparison mode** - view two destinations side by side
- **Show more** - load 3 fresh destinations without leaving the page
- **Saved destinations** with undo remove, trip notes, and one-tap Explore
- **Share card** - styled travel-poster modal with copy/share options
- **Personalise panel** - 5 theme presets, accent colour picker, font size, map style
- Deployed on Vercel with Supabase (PostgreSQL) for destination data and result caching

🔗 Live Demo: https://wander-travel-app-jade.vercel.app

💻 GitHub: https://github.com/chemicalwolf1836/wander-travel-app

---

### 💰 RetireAI - AI Retirement Planner

A full-stack SaaS web app that helps anyone plan their retirement with AI-powered projections and personalised recommendations.

- Built with Next.js 16 (App Router), TypeScript, Tailwind CSS v4, and shadcn/ui
- Interactive savings projection chart using Recharts - projected vs target growth over time
- Readiness breakdown across 4 key retirement indicators with progress bars
- AI recommendations panel powered by the Claude API (Anthropic)
- Scenario comparison - conservative (4%), moderate (7%), and aggressive (10%) return projections
- Supabase authentication (email/password) and PostgreSQL database with Row Level Security
- 5-theme colour picker with CSS variable injection and localStorage persistence
- Dark mode toggle persisted across sessions

🔗 Live Demo: https://retirement-planner-chi.vercel.app

💻 GitHub: https://github.com/chemicalwolf1836/retirement-planner

---

### 🌆 Neon Kissa V2 - Bilingual Cocktail Bar Redesign

A fully separate V2 of the Tokyo Neon Kissa concept, rebuilt in Next.js 16 and React 19 with a stronger design system and more interactive features.

- Four switchable neon palettes (Ruby, Cyber, Amber, Jade) controlled by CSS custom properties - one attribute swap changes the whole site
- Mood and sweetness-based cocktail finder that scores and ranks all menu items in real time as the user types
- Bilingual virtual host Hana with rule-based responses in English and Japanese, reading the active language state
- Reservation form with a confirmation state and bilingual plan-your-visit summary
- Atmosphere mosaic using CSS Grid with tiles spanning multiple columns and rows
- Daily hero image rotation from seven Unsplash photos chosen by day of the week
- Built with Next.js 16, React 19, TypeScript, and Tailwind CSS v4

🔗 Live Demo: https://neon-kissa-v2.vercel.app

💻 GitHub: https://github.com/chemicalwolf1836/neon-kissa-v2

---

### 🍸 Tokyo Neon Kissa - AI-Powered Cocktail Bar Website

A cyberpunk-style bilingual cocktail bar website for Tokyo nightlife venues, featuring an AI virtual host.

- Built with Next.js, TypeScript, and Tailwind CSS
- **AI virtual host "Hana"** powered by Claude - answers questions about the menu, hours, and reservations; responds in English or Japanese automatically
- Persistent bilingual interface (EN/JP) - language preference saved to localStorage
- Cocktail finder with mood and sweetness scoring algorithm
- Reservation form with email notifications via Resend API
- Atmosphere gallery with fullscreen lightbox and keyboard navigation
- 6-theme colour palette picker with CSS variables and localStorage persistence
- CSS neon tube flicker animation on the brand using keyframes

🔗 Live Demo: https://tokyo-neon-bar.vercel.app

💻 GitHub: https://github.com/chemicalwolf1836/tokyo-neon-bar

---

### 🤖 AI Handbook Generator

Upload PDFs (or just name a topic) and generate a structured, multi-section handbook - planned, written section by section, and streamed live. Now running fully serverless inside my portfolio, rebuilt from my original Python/Gradio version.

- Rebuilt from Python/Gradio into vanilla JavaScript with a Vercel Edge Function backend
- Architected a two-mode API - one fast outline call, then one streamed call per section - so the browser orchestrates a multi-minute generation within serverless time limits
- Implemented client-side PDF text extraction with pdf.js, processed in the visitor's browser
- Streams each ~1,200-word section live using Llama 3.3 70B via the Groq API
- Keeps the API key server-side behind the edge function, with Markdown export of the finished handbook

🔗 Live Demo: https://batmagnai-ganbaatar-portfolio.vercel.app/handbook-generator-app.html

💻 GitHub: https://github.com/chemicalwolf1836/Batmagnai-Ganbaatar---Portfolio- (original Python version: https://github.com/chemicalwolf1836/handbook-generator)

---

### 💼 AI Job Application Assistant

Upload a CV and paste a job description - get a tailored cover letter, CV suggestions, skills-gap analysis, interview questions, and a salary estimate. Now running fully serverless inside my portfolio, rebuilt from my original Python/Gradio version.

- Rebuilt from Python/Gradio into vanilla JavaScript with a Vercel Edge Function backend
- Streams Llama 3.3 70B responses token by token via the Groq API for a live-typing result panel
- Implemented client-side CV parsing with pdf.js, so PDF text extraction happens in the browser
- Designed five focused system prompts (cover letter, CV review, skills gap, interview prep, salary) selectable from one interface
- Keeps the API key server-side behind the edge function, with copy and Markdown download for every result

🔗 Live Demo: https://batmagnai-ganbaatar-portfolio.vercel.app/job-assistant-app.html

💻 GitHub: https://github.com/chemicalwolf1836/Batmagnai-Ganbaatar---Portfolio- (original Python version: https://github.com/chemicalwolf1836/job-assistant-)

---

### ⭐ PromptKit (v2)

A front-end workflow tool that transforms rough project notes into structured, reusable outputs for portfolio documentation and AI workflows.

- Structured input system (Problem / Actions / Result / Tools)
- Live preview that updates in real time
- Autosave and draft persistence using localStorage
- Save, reload, export, import, search, and filter saved prompts as reusable cards

🔗 Live Demo: https://batmagnai-ganbaatar-portfolio.vercel.app/promptkit.html

💻 GitHub: https://github.com/chemicalwolf1836/Batmagnai-Ganbaatar---Portfolio-

---

### 🍋 Little Lemon Menu

A responsive restaurant menu interface built with HTML/CSS/JS.

💻 GitHub: https://github.com/chemicalwolf1836/little-lemon-website

---

## 🧰 Skills

**Frontend**
- HTML, CSS, JavaScript
- TypeScript
- React, Next.js
- Tailwind CSS
- Framer Motion

**Backend**
- Node.js
- Next.js API Routes
- Vercel Edge Functions
- Supabase (PostgreSQL)
- Email APIs (Resend)
- Python

**AI & ML**
- Anthropic Claude API
- Groq API
- LLM Engineering & Prompt Design
- RAG (Retrieval-Augmented Generation)
- sentence-transformers, numpy
- Gradio

**Tools**
- Git / GitHub
- Vercel, Hugging Face Spaces
- VS Code
- Mapbox

**Certifications**
- CompTIA A+ (Core 1 - Passed)
- CompTIA A+ Core 2 - In Progress

---

## 💬 Let's Connect

🔗 Portfolio: https://batmagnai-ganbaatar-portfolio.vercel.app

🔗 LinkedIn: https://linkedin.com/in/batmagnai-ganbaatar-025a94211

📫 Email: batmagnai.ganbaatar@gmail.com
