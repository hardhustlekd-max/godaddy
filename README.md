# PermitFinal Application - GoDaddy Direct Connect Deployment

This is the production-ready fullstack application optimized for GoDaddy Direct Connect deployment.

## Tech Stack

- **Frontend:** React 19 with TypeScript, Vite, Tailwind CSS
- **Backend:** Express.js with Node.js/TypeScript
- **Database:** Firebase Firestore (via Admin SDK)
- **Build Tool:** Vite + esbuild
- **Authentication:** Role-based access control (RBAC)

## Features

- QR Code permit generation and verification
- Role-based user management (Clerk, Officer, Admin, Super Admin)
- Firebase Firestore real-time database integration
- Responsive UI with Tailwind CSS
- Production build optimization

## Quick Start

### Installation
```bash
npm install
```

### Development
```bash
npm run dev
```

### Production
```bash
npm run build
npm start
```

## Environment Variables

Create `.env` file from `.env.example`:
```bash
FIREBASE_PROJECT_ID=your_project_id
FIREBASE_PRIVATE_KEY=your_private_key
FIREBASE_CLIENT_EMAIL=your_email
GOOGLE_GENERATIVE_AI_API_KEY=your_api_key
NODE_ENV=production
PORT=3000
```

## Deployment

See `DEPLOYMENT.md` for detailed GoDaddy deployment instructions.

## Health Check

```bash
curl http://localhost:3000/api/health
```
