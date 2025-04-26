# Vercel CLI Quick Start Guide

This is a quick guide to deploy your project using the Vercel CLI. Since you've already pushed your project to GitHub, you can follow these steps to deploy it quickly.

## Prerequisites

- A [Vercel](https://vercel.com) account
- Your project already pushed to GitHub (which you've done)

## Deployment Steps

### 1. Install the Vercel CLI

```bash
npm install -g vercel
```

### 2. Login to Vercel

```bash
vercel login
```

Follow the prompts to authenticate your account. This will open a browser window for you to confirm the login.

### 3. Deploy Your Project

Navigate to your project directory and run:

```bash
vercel
```

During the first deployment, you'll be asked a series of questions:

- **Set up and deploy?** Select `Y`
- **Link to existing project?** Select `Y` if you've already created a project on Vercel dashboard
- **Which scope?** Select your personal account or team
- **Link to existing project?** Select your GitHub project from the list

### 4. Environment Variables

If prompted about environment variables, make sure to add:

- `VITE_SUPABASE_URL`: `https://hazomlnzobmcvdtycfnk.supabase.co`
- `VITE_SUPABASE_ANON_KEY`: `eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6Imhhem9tbG56b2JtY3ZkdHljZm5rIiwicm9sZSI6ImFub24iLCJpYXQiOjE3NDQyOTU2MzcsImV4cCI6MjA1OTg3MTYzN30.1JCsZYEvAP9j58tAfjKiuzT4tnOtMioCHcpte0Ke6PY`

### 5. Production Deployment

For production deployments, use:

```bash
vercel --prod
```

### 6. View Your Deployment

After deployment completes, Vercel will provide a URL where your application is live. You can also view all your deployments on the Vercel dashboard.

## Troubleshooting

If you encounter any issues:

1. Ensure you're in the correct project directory
2. Check that all environment variables are correctly set
3. Verify your project builds locally with `npm run build`
4. Run `vercel logs` to see deployment logs

## Additional Commands

- `vercel ls` - List all your deployments
- `vercel logs` - View deployment logs
- `vercel env add` - Add environment variables
- `vercel domains add` - Add custom domains

For more information, see the [Vercel CLI Documentation](https://vercel.com/docs/cli).