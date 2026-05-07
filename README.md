<div align="center">

# 🤖 AIVA — AI Financial Advisor

### _Artificial Intelligence Value Assistant for Indian Personal Finance_

[![Live Demo](https://img.shields.io/badge/Live%20Demo-aiva--36.lovable.app-blueviolet?style=for-the-badge&logo=vercel)](https://aiva-36.lovable.app/)
[![CI/CD](https://img.shields.io/github/actions/workflow/status/shaawtymaker/AIVA-FINTECH/ci.yml?branch=master&style=for-the-badge&logo=githubactions&logoColor=white&label=CI%2FCD)](https://github.com/shaawtymaker/AIVA-FINTECH/actions)
[![Docker Hub](https://img.shields.io/badge/Docker%20Hub-Published-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://hub.docker.com/r/shaawtymaker/aiva-fintech)
[![Vercel](https://img.shields.io/badge/Vercel-Deployed-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://vercel.com/)

[![React](https://img.shields.io/badge/React-18.3-61DAFB?style=for-the-badge&logo=react)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.5-3178C6?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-5.4-646CFF?style=for-the-badge&logo=vite)](https://vitejs.dev/)
[![Supabase](https://img.shields.io/badge/Supabase-Auth%20%26%20DB-3ECF8E?style=for-the-badge&logo=supabase)](https://supabase.com/)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.4-06B6D4?style=for-the-badge&logo=tailwindcss)](https://tailwindcss.com/)
[![LM Studio](https://img.shields.io/badge/LLM-LM%20Studio-FF6B35?style=for-the-badge&logo=ai)](https://lmstudio.ai/)

> **AIVA** is an AI-powered personal finance web application tailored for the **Indian market**. It delivers intelligent financial advice through an **LM Studio**-powered local LLM chat interface, interactive financial calculators, curated learning resources, and investment education — all within a stunning, animated glassmorphism UI.

</div>

---

## 📸 Preview

| Homepage | AI Chat | Financial Calculators |
|---|---|---|
| Hero with animated background, parallax effects, and feature cards | India-specific AI advisor powered by Hermes-3-Llama-3.1-8b | Six interactive calculators for compound interest, debt, retirement, budget, mortgage & investments |

---

## ✨ Features

### 🤖 AI Financial Assistant (AIVA Chat)
- Powered by **[LM Studio](https://lmstudio.ai/)** running **Hermes-3-Llama-3.1-8b** locally
- Specialized system prompt for **Indian financial context** — references PPF, ELSS, NSE, BSE, RBI policies, Indian tax laws
- **Quick topic selectors**: Tax Saving, SIPs, Mutual Funds, Real Estate, PPF & EPF, Credit Score, Stock Market, Insurance, Gold, Fixed Deposits
- **Suggested questions** pre-built for common Indian finance queries
- Real-time **typing indicators** with animated bounce dots
- Full **conversation history** maintained per session

### 📊 Investment Tracking
- Consolidated portfolio overview with visual analytics
- Real-time performance tracking across stocks, bonds, mutual funds, and ETFs
- Customizable price alerts and portfolio change notifications
- Detailed reports on gains, losses, and dividend income

### 💰 Smart Saving
- AI-driven analysis of income and spending patterns
- Multiple customizable saving goals with milestones
- Round-up feature for micro-savings from daily purchases
- Predictive analytics on when goals will be reached

### 💳 Debt Management
- Debt repayment strategies: **Avalanche Method** and **Snowball Method**
- Visual debt reduction progress charts
- Payment reminders and refinancing opportunity alerts
- Interest savings calculations for extra payment scenarios

### 🎯 Goal Planning
- Detailed financial roadmaps for any goal (home, retirement, education)
- Scenario modeling and milestone tracking
- Automatic plan adjustments when circumstances change
- Tailored investment and saving recommendations per goal

### 📚 Financial Education Center
- **6 in-depth financial articles** covering:
  - Emergency Funds
  - 50/30/20 Budgeting Rule
  - Stocks, Bonds & ETFs explained
  - The Power of Compound Interest
  - Debt Payoff Strategies
  - How to Improve Your Credit Score
- Downloadable **Beginner's Investment Guide** (PDF)
- Links to investing guides and calculator resources

### 🧮 Financial Calculators (6 Tools)
All calculators output results in **Indian Rupees (₹)** using `en-IN` locale formatting:

| Calculator | Inputs |
|---|---|
| **Compound Interest** | Principal, Rate, Time Period |
| **Debt Payoff** | Debt Amount, Interest Rate, Monthly Payment |
| **Retirement Savings** | Current Age, Retirement Age, Current Savings, Monthly Contribution |
| **Budget (50/30/20)** | Monthly Income → auto-splits into Needs / Wants / Savings |
| **Mortgage / Home Loan** | House Price, Down Payment, Interest Rate, Loan Term |
| **Investment Returns** | Initial Investment, Rate, Duration, Monthly Contribution |

### 🧩 Investing Fundamentals Page
- Why start investing: Beat Inflation, Build Wealth, Passive Income
- Step-by-step getting started guide
- **4 common investment types** compared side-by-side (Stocks, ETFs, Bonds, Real Estate) with risk level, time horizon, and expected return

### 👤 User Profile & Settings
- **General Tab**: Name, phone number (email read-only from Supabase auth)
- **Preferences Tab**: Currency (INR/USD/EUR), Language (English/Hindi), Dark Mode toggle, Push Notifications, Email Newsletter
- **Security Tab**: Two-Factor Authentication toggle, Change Password, Delete Account (danger zone)
- All settings persisted to Supabase `profiles` table

---

## 🏗️ Tech Stack

| Layer | Technology |
|---|---|
| **Frontend Framework** | React 18 + TypeScript |
| **Build Tool** | Vite 5 |
| **Styling** | Tailwind CSS 3 + `tailwindcss-animate` |
| **UI Components** | shadcn/ui (Radix UI primitives) |
| **State Management** | React Context API + TanStack Query v5 |
| **Routing** | React Router DOM v6 |
| **Forms & Validation** | React Hook Form + Zod |
| **Backend / Auth / DB** | Supabase (PostgreSQL + Auth) |
| **AI / LLM** | LM Studio (Hermes-3-Llama-3.1-8b, local inference) |
| **Charts** | Recharts |
| **PDF Generation** | jsPDF |
| **Animations** | CSS animations + `next-themes` dark mode |
| **Icons** | Lucide React |
| **Toast Notifications** | Sonner + Radix Toast |
| **Date Utilities** | date-fns |
| **Package Manager** | npm / bun |

---

## 🔧 DevOps & Tooling

| Category | Tool | Purpose |
|---|---|---|
| **Version Control** | Git | Source code versioning |
| **Repository** | GitHub | Code hosting, issues, pull requests |
| **CI/CD** | GitHub Actions | Automated lint, build, Docker push, and Vercel deploy |
| **Containerization** | Docker | Multi-stage build with Node 20 Alpine + nginx Alpine |
| **Container Registry** | Docker Hub | Published images at `shaawtymaker/aiva-fintech` |
| **Deployment** | Vercel | Production hosting with edge CDN, SPA rewrites, and security headers |
| **Linting** | ESLint 9 + TypeScript ESLint | Code quality enforcement with zero errors |
| **Type Checking** | TypeScript `tsc --noEmit` | Compile-time type safety |

### CI/CD Pipeline

Every push to `master` triggers the following fully automated pipeline:

```
┌─────────────────────┐     ┌──────────┐     ┌────────────────────────┐
│ 🔍 Lint & Type Check│────▶│ 🏗️ Build │──┬──▶│ 🐳 Docker Hub Push     │
│   ESLint + tsc      │     │ Vite prod │  │  │   shaawtymaker/        │
│   0 errors ✅        │     │ bundle    │  │  │   aiva-fintech:latest  │
└─────────────────────┘     └──────────┘  │  └────────────────────────┘
                                          │  ┌────────────────────────┐
                                          └──▶│ ▲ Vercel Production    │
                                              │   Edge CDN deploy     │
                                              └────────────────────────┘
```

| Job | Trigger | Description |
|---|---|---|
| **🔍 Lint & Type Check** | Push + PRs | Runs ESLint (0 errors) and `tsc --noEmit` for type safety |
| **🏗️ Build** | After lint passes | Produces optimized production bundle (~1.6 MB), uploads as artifact |
| **🐳 Docker Build & Push** | Push to master | Builds multi-stage Docker image & pushes to Docker Hub with SHA + `latest` tags |
| **▲ Vercel Deploy** | Push to master | Deploys production build to Vercel edge network with security headers |

### Docker

The project uses a **multi-stage Dockerfile** for an optimized production image:

- **Stage 1 (Builder)** — Node 20 Alpine installs dependencies and builds the Vite production bundle
- **Stage 2 (Production)** — nginx Alpine serves the static files with gzip compression, SPA routing, and aggressive asset caching
- **Final image size**: ~25 MB

### Pull from Docker Hub

```sh
# Pull the latest image
docker pull shaawtymaker/aiva-fintech:latest

# Run it
docker run -d -p 3000:80 shaawtymaker/aiva-fintech:latest
```

---

## 🗂️ Project Structure

```
AIVA-FINTECH/
├── .github/
│   └── workflows/
│       └── ci.yml                 # GitHub Actions CI/CD pipeline
├── public/                        # Static assets
├── src/
│   ├── App.tsx                    # Root app with routing
│   ├── main.tsx                   # React entry point
│   ├── index.css                  # Global styles & Tailwind base
│   ├── pages/
│   │   ├── Index.tsx              # Landing page (Hero + Features + CTA)
│   │   ├── Chat.tsx               # Dedicated AI chat page
│   │   ├── Investing.tsx          # Investment fundamentals
│   │   ├── Learn.tsx              # Financial education center
│   │   ├── Resources.tsx          # Financial calculators hub
│   │   ├── FeatureDetailed.tsx    # Detailed feature subpages
│   │   ├── Auth.tsx               # Login / Signup page
│   │   └── NotFound.tsx           # 404 page
│   ├── components/
│   │   ├── ChatInterface.tsx      # AI chat UI with LLM integration
│   │   ├── ChatMessage.tsx        # Individual chat message bubble
│   │   ├── FinancialCalculator.tsx # Multi-type calculator component
│   │   ├── ProfileSettings.tsx    # User profile settings (tabbed)
│   │   ├── AnimatedBackground.tsx # Animated gradient background
│   │   ├── Navbar.tsx             # Top navigation bar
│   │   ├── FeatureCard.tsx        # Feature grid card with gradient
│   │   ├── FinancialArticle.tsx   # Expandable article component
│   │   ├── DownloadGuide.tsx      # PDF guide download button
│   │   ├── ThemeToggle.tsx        # Dark/Light mode toggle
│   │   ├── UserMenu.tsx           # Auth-aware user dropdown
│   │   ├── auth/                  # Auth form components
│   │   └── ui/                    # shadcn/ui component library (49 components)
│   ├── contexts/
│   │   └── AuthContext.tsx        # Supabase session + profile context
│   ├── hooks/
│   │   └── use-toast.ts           # Toast notification hook
│   ├── integrations/
│   │   └── supabase/              # Supabase client + type definitions
│   ├── lib/
│   │   └── utils.ts               # Tailwind merge utility
│   └── providers/
│       └── ThemeProvider.tsx       # next-themes dark mode provider
├── supabase/                      # Supabase config & migrations
├── .dockerignore                  # Files excluded from Docker build context
├── Dockerfile                     # Multi-stage Docker build (Node → nginx)
├── nginx.conf                     # nginx config for SPA routing & gzip
├── vercel.json                    # Vercel deployment config & SPA rewrites
├── tailwind.config.ts             # Tailwind theme (finance color palette)
├── vite.config.ts                 # Vite build config
└── package.json
```

---

## 🎨 Design System

AIVA uses a custom color palette defined in `tailwind.config.ts`:

| Token | Color | Usage |
|---|---|---|
| `finance-purple` | `#8B5CF6` | Primary CTAs, AI bot icon, highlights |
| `finance-blue` | `#3B82F6` | Accents, feature cards |
| `finance-teal` | `#14B8A6` | Supporting accents |
| `finance-lavender` | `#C4B5FD` | Soft highlights |

Additional UI patterns:
- **Glassmorphism cards** (`.glass-card`) with backdrop blur
- **Animated background** with floating gradient blobs
- **Parallax Hero** — scroll-driven `translateY` on hero card
- **Fade-in animations** with staggered delays on feature cards
- Full **Dark / Light** theme support via `next-themes`

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** `>= 18` and **npm** (or **bun**)
- A **Supabase** project (for Auth & DB)
- **[LM Studio](https://lmstudio.ai/)** installed and running with the `hermes-3-llama-3.1-8b` model loaded  
  (any model available in LM Studio that supports chat completions will work)
- **Docker** (optional, for containerized deployment)

### Installation

```sh
# 1. Clone the repository
git clone https://github.com/shaawtymaker/AIVA-FINTECH.git

# 2. Navigate to the project directory
cd AIVA-FINTECH

# 3. Install dependencies
npm install
# or with bun
bun install
```

### Environment Setup

Create a `.env` file in the root directory:

```env
VITE_SUPABASE_URL=your_supabase_project_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

> The Supabase credentials are already pre-configured in `src/integrations/supabase/client.ts` if you are using the default Lovable project setup.

### LM Studio Setup

AIVA uses **LM Studio** as its local AI backend. Follow these steps:

1. Download and install **[LM Studio](https://lmstudio.ai/)**
2. Search for and download the `hermes-3-llama-3.1-8b` model (or any chat-compatible model)
3. In LM Studio, go to **Local Server** tab and click **Start Server**
4. The server runs by default at `http://localhost:8080`

Then update the endpoint in `src/components/ChatInterface.tsx` to match your LM Studio server IP:

```ts
const response = await fetch('http://<YOUR-LM-STUDIO-IP>:8080/v1/chat/completions', {
  // ...
  body: JSON.stringify({
    model: 'hermes-3-llama-3.1-8b',  // Match the model loaded in LM Studio
    // ...
  })
});
```

> 💡 **Tip:** If running LM Studio on the same machine, use `http://localhost:8080`. For LAN access from another device, use your machine's local IP address.

### Running Locally

```sh
# Start the development server
npm run dev
```

The app will be available at `http://localhost:5173`

### Build for Production

```sh
npm run build
```

Output is generated in the `dist/` folder.

---

## 🐳 Docker Deployment

Build and run the production Docker image locally:

```sh
# Build the image
docker build -t aiva-fintech .

# Run the container
docker run -d -p 3000:80 --name aiva-fintech aiva-fintech
```

The app will be available at `http://localhost:3000`

#### Docker Commands Reference

| Command | Description |
|---|---|
| `docker build -t aiva-fintech .` | Build the production image |
| `docker run -d -p 3000:80 --name aiva-fintech aiva-fintech` | Run in detached mode on port 3000 |
| `docker stop aiva-fintech` | Stop the running container |
| `docker start aiva-fintech` | Restart a stopped container |
| `docker rm aiva-fintech` | Remove the container |
| `docker logs aiva-fintech` | View nginx access/error logs |
| `docker images aiva-fintech` | Check image size |

---

## ▲ Vercel Deployment

### One-Click Deploy

Deploy directly from the command line:

```sh
# Install Vercel CLI
npm install -g vercel

# Deploy to production
vercel --prod
```

### Auto-Deploy via GitHub

1. Go to [vercel.com](https://vercel.com) and import your GitHub repository
2. Vercel auto-detects the Vite framework from `vercel.json`
3. Every push to `master` triggers an automatic production deployment
4. Pull requests get preview deployments with unique URLs

The `vercel.json` configuration handles:
- SPA route rewrites (all routes → `index.html`)
- Static asset caching (1 year, immutable)
- Security headers (`X-Content-Type-Options`, `X-Frame-Options`, `Referrer-Policy`)

---

## ⚙️ CI/CD Setup (GitHub Actions)

The CI/CD pipeline at `.github/workflows/ci.yml` runs automatically on every push to `master` and on pull requests.

### Required GitHub Secrets

Add these secrets at **GitHub → Settings → Secrets and variables → Actions → New repository secret**:

| Secret | How to Get It | Required For |
|---|---|---|
| `DOCKERHUB_USERNAME` | Your Docker Hub username | 🐳 Docker Push |
| `DOCKERHUB_TOKEN` | Docker Hub → Account Settings → Security → [New Access Token](https://hub.docker.com/settings/security) | 🐳 Docker Push |
| `VERCEL_TOKEN` | Vercel → Account Settings → [Tokens → Create](https://vercel.com/account/tokens) | ▲ Vercel Deploy |

### Environment Variables

These should be set in your hosting environment (Vercel dashboard / `.env` locally):

| Variable | Description |
|---|---|
| `VITE_SUPABASE_URL` | Supabase project URL |
| `VITE_SUPABASE_ANON_KEY` | Supabase anonymous key |

> **Note:** The lint and build jobs run without any secrets. Only the Docker push and Vercel deploy steps require the secrets above.

### Pipeline Status

All 4 jobs are currently ✅ **passing**:
- 🔍 Lint & Type Check — 0 errors, 8 non-blocking warnings
- 🏗️ Build — 2200 modules, ~21s build time
- 🐳 Docker Build & Push — Pushes `shaawtymaker/aiva-fintech:latest`
- ▲ Vercel Deploy — Production edge deployment

---

## 🗃️ Database Schema (Supabase)

The app uses a `profiles` table in Supabase PostgreSQL:

| Column | Type | Description |
|---|---|---|
| `id` | `uuid` (FK → `auth.users`) | User ID |
| `name` | `text` | Full name |
| `phone` | `text` | Phone number |
| `currency` | `text` | Preferred currency (default: `INR`) |
| `language` | `text` | UI language (`en` / `hi`) |
| `dark_mode` | `boolean` | Dark mode preference |
| `notifications` | `boolean` | Push notification preference |
| `newsletter` | `boolean` | Email newsletter opt-in |
| `two_factor_auth` | `boolean` | 2FA toggle |
| `updated_at` | `timestamptz` | Last updated timestamp |

---

## 🛣️ App Routes

| Route | Page | Description |
|---|---|---|
| `/` | Index | Landing page with hero, features, and AI chat preview |
| `/chat` | Chat | Dedicated full-page AI chat interface |
| `/investing` | Investing | Investment fundamentals and asset types |
| `/learn` | Learn | Financial education articles and guides |
| `/resources` | Resources | Six interactive financial calculators |
| `/feature/:id` | FeatureDetailed | Deep-dive pages for each feature |
| `/auth` | Auth | Login and Sign Up |
| `/profile` | ProfileSettings | User account settings |
| `*` | NotFound | 404 page |

---

## 🌐 Live Demo

🔗 **[https://aiva-36.lovable.app/](https://aiva-36.lovable.app/)**

> **Note:** The AI chat feature requires **LM Studio** running locally with a model loaded. In the hosted demo, chat responses may be unavailable without a connected LM Studio instance.

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m 'Add: your feature description'`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Open a Pull Request

The CI/CD pipeline will automatically run lint and build checks on your PR.

Please ensure code follows the existing TypeScript and ESLint conventions.

---

## ⚠️ Disclaimer

> The financial information provided by AIVA is for **educational purposes only** and should **not** be considered professional financial advice. All investments involve risk. Always consult a qualified financial advisor before making investment decisions.

---

## 📄 License

This project is private. All rights reserved © 2024–2026 AIVA-FINTECH.

---

<div align="center">

**Built with ❤️ for smarter financial decisions in India**

[🌐 Live App](https://aiva-36.lovable.app/) • [🐳 Docker Hub](https://hub.docker.com/r/shaawtymaker/aiva-fintech) • [🐛 Report Bug](https://github.com/shaawtymaker/AIVA-FINTECH/issues) • [💡 Request Feature](https://github.com/shaawtymaker/AIVA-FINTECH/issues)

</div>
