# Deploying to Vercel

This guide will help you deploy your React application to Vercel.

## Prerequisites

1. A [Vercel](https://vercel.com) account
2. Git installed on your computer
3. Your project pushed to a GitHub, GitLab, or Bitbucket repository

## Deployment Steps

### 1. Push Your Code to a Git Repository

If your code is not already in a Git repository, create one and push your code:

```bash
# Initialize a git repository if you haven't already
git init

# Add all files
git add .

# Commit the changes
git commit -m "Initial commit"

# Add your remote repository (replace with your actual repository URL)
git remote add origin <your-repository-url>

# Push to the repository
git push -u origin main
```

### 2. Deploy to Vercel

1. Go to [Vercel](https://vercel.com) and sign in or create an account
2. Click on "Add New..." > "Project"
3. Import your Git repository
4. Configure your project:
   - Framework Preset: Vite
   - Build Command: `npm run build` (already configured in vercel.json)
   - Output Directory: `dist` (already configured in vercel.json)
   - Install Command: `npm install`

### 3. Environment Variables

Your project uses Supabase, so you'll need to add the following environment variables in Vercel:

- `VITE_SUPABASE_URL`: `https://hazomlnzobmcvdtycfnk.supabase.co`
- `VITE_SUPABASE_ANON_KEY`: `eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6Imhhem9tbG56b2JtY3ZkdHljZm5rIiwicm9sZSI6ImFub24iLCJpYXQiOjE3NDQyOTU2MzcsImV4cCI6MjA1OTg3MTYzN30.1JCsZYEvAP9j58tAfjKiuzT4tnOtMioCHcpte0Ke6PY`

To add these variables:
1. In your Vercel project dashboard, go to "Settings" > "Environment Variables"
2. Add each variable with its corresponding value

### 4. Deploy

Click "Deploy" and wait for the build to complete. Vercel will provide you with a URL where your application is deployed.

## Updating Your Deployment

Whenever you push changes to your Git repository, Vercel will automatically rebuild and redeploy your application.

## Custom Domains

To use a custom domain:
1. Go to your project in Vercel
2. Navigate to "Settings" > "Domains"
3. Add your domain and follow the instructions to configure DNS settings

## Troubleshooting

If you encounter any issues during deployment:

1. Check the build logs in Vercel for specific errors
2. Ensure all dependencies are correctly listed in your package.json
3. Verify that your application builds successfully locally with `npm run build`
4. Make sure environment variables are correctly set in Vercel

## Deploying with Vercel CLI

You can also deploy your project using the Vercel CLI. Here's how:

1. Install the Vercel CLI globally:
   ```bash
   npm install -g vercel
   ```

2. Login to your Vercel account:
   ```bash
   vercel login
   ```

3. Navigate to your project directory and run the deployment command:
   ```bash
   cd your-project-directory
   vercel
   ```

4. Follow the interactive prompts:
   - Confirm the project directory
   - Set up and deploy project
   - Link to an existing project (select your GitHub project)
   - Confirm deployment settings

5. For subsequent deployments, you can simply run:
   ```bash
   vercel
   ```

6. For production deployments, use:
   ```bash
   vercel --prod
   ```

## Additional Resources

- [Vercel Documentation](https://vercel.com/docs)
- [Vercel CLI Documentation](https://vercel.com/docs/cli)
- [Vite Deployment Guide](https://vitejs.dev/guide/static-deploy.html)
- [Supabase Documentation](https://supabase.io/docs)