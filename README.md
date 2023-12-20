This is a [Next.js](https://nextjs.org/) project.

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the Vercel or Netlify or any platform. Deploy the project and copy domain for webhook creation.

## Clerk details

- Create an account on [clerk](https://clerk.com/)
- Create new project and copy the key's into .env.local
- Create WEBHOOK based on hosted domain to the webhook path. [ref](https://clerk.com/docs/users/sync-data)
- update the secret key on .env.local and deploy the project

## MongoDB

- Create MongoDb account and update MONGODB_URI on .env.local

## Update on Vercel

- Update webhook secret key on vercel deployment.
- Rebuild the project.
- Run local or deployed project. Create new user using clerk.
- Confirm user creation Log's on vercel and details on User collection on mongodb.

## Required Keys on .env.local

- NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY, CLERK_SECRET_KEY, WEBHOOK_SECRET, MONGODB_URI