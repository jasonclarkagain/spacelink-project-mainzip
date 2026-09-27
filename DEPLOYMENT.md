# SpaceLink Deployment Guide

## Environment Setup

### Required Environment Variables
```bash
# Database
DATABASE_URL=your_postgresql_connection_string
PGHOST=your_db_host
PGPORT=5432
PGUSER=your_db_user
PGPASSWORD=your_db_password
PGDATABASE=your_db_name

# Authentication
SESSION_SECRET=your_random_session_secret
REPL_ID=your_replit_app_id
ISSUER_URL=https://replit.com/oidc
REPLIT_DOMAINS=your-app-domain.replit.app
```

### Database Schema
Run this command to create all tables:
```bash
npm run db:push
```

## Replit Deployment

1. Fork/Import this repository to Replit
2. Set environment variables in Replit Secrets
3. Run `npm install` to install dependencies
4. Run `npm run db:push` to create database tables
5. Start with `npm run dev`
6. Use Replit Deployments for production

## Manual Deployment

### Prerequisites
- Node.js 20+
- PostgreSQL database
- SSL certificates for HTTPS

### Steps
1. Clone repository
2. Install dependencies: `npm install`
3. Set environment variables
4. Build frontend: `npm run build`
5. Start server: `npm start`

## Demo Data
The platform includes demo content and invite codes:
- `WELCOME2025` (10 uses)
- `SPACEJOIN` (5 uses)
- `CREATIVE` (3 uses)

## Security Notes
- Always use HTTPS in production
- Keep environment variables secure
- Regularly update dependencies
- Monitor file uploads for abuse
- Review adult content verification regularly

## Backup Strategy
- Database: Daily automated backups
- Files: Regular backup of uploads directory
- Environment: Secure backup of configuration