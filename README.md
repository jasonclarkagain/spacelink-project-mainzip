# SpaceLink - Social Platform

A modern social platform inspired by early MySpace, built for family and close friends with extensive customization freedom, privacy tools, and community features.

## Features

### Core Social Features
- **User Profiles** with extensive customization options
- **File Sharing** supporting files up to 50GB
- **Real-time Messaging** with WebSocket support
- **Posts & Comments** with media integration
- **Invite-only Registration** system

### Media Integration
- Support for YouTube, Rumble, BitChute, X (Twitter), Odysee, and Brighteon
- Automatic media detection and embedded playback
- Video platform integration with metadata

### Specialized Content Areas
- **Health Hub** - Alternative medicine resources and independent health information
- **Safety Center** - Human trafficking awareness and educational content
- **Privacy Tools** - Built-in Tor browser and encrypted communications
- **Civic Engagement** - Community resources and representative contact tools

### Customization & Apps
- **App Marketplace** with installable widgets
- **Custom Themes** (Cyberpunk, Ocean, Fire, Matrix)
- **Profile Customization** with CSS editing capabilities
- **Layout Options** for personalized experiences

### Privacy & Security
- **Age Verification System** with robust adult content protection
- **End-to-end Encryption** for secure messaging
- **Anonymous Email** with temporary addresses
- **Tor Browser Integration** for privacy-focused browsing

## Tech Stack

- **Frontend**: React, TypeScript, Vite, Tailwind CSS, shadcn/ui
- **Backend**: Express.js, TypeScript, PostgreSQL, Drizzle ORM
- **Authentication**: Replit Auth with OpenID Connect
- **Real-time**: WebSocket for messaging
- **Database**: PostgreSQL with 13+ tables
- **Deployment**: Replit with Node.js 20

## Quick Start

### Prerequisites
- Node.js 20+
- PostgreSQL database
- Replit account (for authentication)

### Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd spacelink
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
```bash
# Required environment variables
DATABASE_URL=your_postgresql_connection_string
SESSION_SECRET=your_session_secret
REPL_ID=your_replit_id
ISSUER_URL=https://replit.com/oidc
```

4. Push database schema:
```bash
npm run db:push
```

5. Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:5000`

## Project Structure

```
├── client/          # React frontend application
│   ├── src/
│   │   ├── components/  # Reusable UI components
│   │   ├── pages/      # Application pages
│   │   ├── hooks/      # Custom React hooks
│   │   └── lib/        # Utility functions
├── server/          # Express.js backend
│   ├── db.ts           # Database connection
│   ├── routes.ts       # API routes
│   ├── storage.ts      # Data layer
│   └── replitAuth.ts   # Authentication setup
├── shared/          # Shared TypeScript schemas
│   └── schema.ts       # Drizzle database schemas
└── uploads/         # File upload directory
```

## Demo Access

The platform includes demo invite codes for testing:
- `WELCOME2025` - General access (10 uses)
- `SPACEJOIN` - Community access (5 uses) 
- `CREATIVE` - Creator access (3 uses)

## Key Features Overview

### 🛡️ Privacy First
- Built-in Tor browser for anonymous browsing
- Encrypted messaging with automatic PGP key management
- Anonymous email with self-destruct functionality
- No tracking or data collection

### 🏥 Health Resources
- Alternative medicine information from independent sources
- Treatment center directories (Burzynski, Gerson, Mexican clinics)
- COVID protocol resources from FLCCC
- Vaccine injury support discussions

### 🛡️ Safety Awareness
- Human trafficking education and awareness
- Content from independent researchers and citizen journalists
- Crisis support resources and hotlines
- Community safety protocols

### 🏛️ Civic Engagement
- Congressional representative contact system
- 211 helpline resource integration
- Community support group directories
- Faith community finder

### 🔞 Responsible Content
- Robust age verification system (18+)
- Adult content protection for minors
- Content warnings and age gates
- Separate adult areas with verification requirements

## Contributing

This platform prioritizes:
- Free speech principles with responsible content management
- Independent information sources over mainstream media
- Community safety and support
- Privacy and security for all users
- Unity through respect and understanding

## License

[Add your chosen license here]

## Support

For support and questions, please [add contact information or issue reporting process].