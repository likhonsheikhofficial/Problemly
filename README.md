# Problemly
Problemly - write, run, and preview code fixeablity together with vercel on GROQ powerfull as like v0.dev else bolt.new automotions !!
A comprehensive code documentation platform that allows users to create, share, and collaborate on code snippets with real-time updates. 

## Features

- **Dark Theme UI**: Modern dark-themed interface for comfortable coding
- **Component Generation**: AI-powered component generation with Groq and Together AI
- **Real-time Updates**: Socket.IO integration for live logs and preview status
- **Code Editing**: Syntax highlighting and line numbers for code snippets
- **Component Preview**: Live preview of components with Puppeteer
- **Authentication**: User authentication with JWT and GitHub OAuth
- **Database**: PostgreSQL with Prisma ORM
- **Caching**: Redis for caching and pub/sub messaging
No-code AI builder for websites, 2D/3D games, and apps that can integrate AI features.
“Rosie” the AI co-creator handles code generation, design, and in-app previews—all modifiable in a live code editor if you want more control.
Unlimited AI-generated images and 3D assets included with your projects at no extra cost.
Remix-friendly community: Access to 500,000+ public templates and user-made projects, from simple portfolios to full-blown multiplayer games.
Strong reputation as a cost-effective no-code solution, with easy deployment and minimal barrier to entry.
‍ Comprehensive No-Code Approach
Craft anything: from a plain portfolio site to a fully interactive, multi-user game.
Unlimited AI-Generated Visuals
No hidden fees for image or 3D asset creation—your projects stand out with minimal effort.
Built-In AI Features
Easily embed an AI chatbot or other generative elements directly in your app.
One-Click Deployment
Launch your project instantly—no need to fiddle with external hosting steps.
Vibrant Community & Remixing
Learn, share, and riff on other people’s work. Tap into an ever-growing library of creative ideas.
Generous Free Tier
Weekly prompt refreshes ensure you can keep iterating and building out new concepts without extra costs.
## Tech Stack

### Frontend
- React 18+
- Next.js (App Router)
- TypeScript
- Tailwind CSS
- Socket.IO Client
- shadcn/ui components
- lucide-react icons

### Backend
- Node.js
- Express
- TypeScript
- Prisma ORM
- PostgreSQL
- Redis
- Socket.IO
- Puppeteer
- JWT Authentication

### AI Integration
- Groq AI for code generation
- Together AI for real-time inference

### Infrastructure
- Docker Compose
- GitHub Actions CI/CD
- Vercel (frontend)
- DigitalOcean (backend)
- Nginx reverse proxy

## Getting Started

### Prerequisites
- Node.js 18+
- Docker and Docker Compose
- PostgreSQL
- Redis

### Installation

1. Clone the repository:
\`\`\`bash
git clone https://github.com/yourusername/component-wizard.git
cd component-wizard
\`\`\`

2. Install dependencies:
\`\`\`bash
# Frontend
cd frontend
npm install

# Backend
cd ../backend
npm install
\`\`\`

3. Set up environment variables:
\`\`\`bash
# Frontend (.env.local)
NEXT_PUBLIC_API_URL=http://localhost:4000
NEXT_PUBLIC_SOCKET_URL=http://localhost:4000

# Backend (.env)
PORT=4000
DATABASE_URL=postgresql://postgres:postgres@localhost:5432/component_wizard
REDIS_URL=redis://localhost:6379
JWT_SECRET=your-jwt-secret
FRONTEND_URL=http://localhost:3000
AI_PROVIDER=groq
GROQ_API_KEY=your-groq-api-key
TOGETHER_API_KEY=your-together-api-key
\`\`\`

4. Run database migrations:
\`\`\`bash
cd backend
npx prisma migrate dev
\`\`\`

5. Start the development servers:
\`\`\`bash
# Frontend
cd frontend
npm run dev

# Backend
cd ../backend
npm run dev
\`\`\`

### Docker Deployment

To deploy with Docker Compose:

\`\`\`bash
docker-compose up -d
\`\`\`

## Project Structure

\`\`\`
/
├─ frontend/          # React 18+ app (Tailwind JIT, dark mode)
│   ├─ app/           # Next.js App Router
│   ├─ components/    # React components
│   ├─ hooks/         # Custom React hooks
│   ├─ lib/           # Utility functions
│   └─ public/        # Static assets
├─ backend/           # Node 16+ Express API (TypeScript)
│   ├─ src/           # Source code
│   │   ├─ routes/    # API routes
│   │   ├─ services/  # Business logic
│   │   ├─ middleware/# Express middleware
│   │   └─ types/     # TypeScript types
│   └─ prisma/        # Prisma schema and migrations
├─ infra/             # Infrastructure configuration
│   ├─ nginx/         # Nginx configuration
│   └─ certbot/       # SSL certificates
├─ docker-compose.yml # Docker Compose configuration
└─ .github/workflows/ # GitHub Actions CI/CD
\`\`\`

## License

This project is licensed under the MIT License - see the LICENSE file for details.
