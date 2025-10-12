# Athleaf - AI Personal Trainer Web App

Athleaf is a modern, clean web application designed to provide personalized training and nutrition plans for athletes. It features an AI coach that offers tailored advice based on user profiles and progress.

## Features

- Personalized training and nutrition plans
- AI Coach for customized advice
- Progress tracking and visualization
- User authentication and profile management
- Mobile and desktop optimized interface

## Tech Stack

- Next.js (React framework)
- TypeScript
- Tailwind CSS for styling
- Prisma ORM with PostgreSQL
- NextAuth.js for authentication
- AI integration for personalized coaching

## Getting Started

1. Clone the repository
2. Install dependencies: `npm install`
3. Set up environment variables (see `.env.example`)
4. Run the development server: `npm run dev`
5. Open [http://localhost:3000](http://localhost:3000) in your browser

## Project Structure

- `/src/app`: App router pages and layouts
- `/src/components`: Reusable UI components
- `/src/lib`: Utility functions and shared code
- `/prisma`: Database schema and migrations
- `/public`: Static assets

## Design Guidelines

- **Color Palette:**
  - Primary: Fresh green (#4ADE80)
  - Accent: Leafy teal (#14B8A6)
  - Neutral: White and gray backgrounds
  - Optional secondary accent: Sky blue (#38BDF8)

- **Typography:**
  - Headings: Inter or Poppins (bold, motivational)
  - Body: Inter (light, legible)

## Deployment

### Deploying to Vercel

1. **Prepare your repository**
   - Push your code to a GitHub, GitLab, or Bitbucket repository

2. **Deploy to Vercel**
   - Go to [Vercel](https://vercel.com) and sign up/login
   - Click "New Project" and import your repository
   - Configure the project:
     - Framework Preset: Next.js
     - Root Directory: ./
   - Add environment variables from your `.env.example` file:
     - `DATABASE_URL`: Your PostgreSQL connection string
     - `NEXTAUTH_SECRET`: A secure random string for session encryption
     - `NEXTAUTH_URL`: Your Vercel deployment URL (will be available after first deployment)
   - Click "Deploy"

3. **Set up the database**
   - Create a PostgreSQL database (using Vercel Postgres, Supabase, Railway, etc.)
   - Update your `DATABASE_URL` in Vercel project settings
   - Run database migrations using Prisma:
     ```
     npx prisma migrate deploy
     ```
   - Optionally seed your database:
     ```
     npx prisma db seed
     ```

4. **Verify deployment**
   - Test all functionality on your deployed application
   - Update `NEXTAUTH_URL` if needed

## Future Extensions

- Wearable device integration
- AI performance analysis
- Gamified challenges and achievements
- Mobile app version# athleaf2
