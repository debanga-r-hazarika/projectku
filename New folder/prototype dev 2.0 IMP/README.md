# Welcome to your Lovable project

## Project info

**URL**: https://lovable.dev/projects/de9b67b4-7c44-4e57-ad7a-c5e7fbbb242a

## How can I edit this code?

There are several ways of editing your application.

**Use Lovable**

Simply visit the [Lovable Project](https://lovable.dev/projects/de9b67b4-7c44-4e57-ad7a-c5e7fbbb242a) and start prompting.

Changes made via Lovable will be committed automatically to this repo.

**Use your preferred IDE**

If you want to work locally using your own IDE, you can clone this repo and push changes. Pushed changes will also be reflected in Lovable.

The only requirement is having Node.js & npm installed - [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating)

Follow these steps:

```sh
# Step 1: Clone the repository using the project's Git URL.
git clone <YOUR_GIT_URL>

# Step 2: Navigate to the project directory.
cd <YOUR_PROJECT_NAME>

# Step 3: Install the necessary dependencies.
npm i

# Step 4: Start the development server with auto-reloading and an instant preview.
npm run dev
```

**Edit a file directly in GitHub**

- Navigate to the desired file(s).
- Click the "Edit" button (pencil icon) at the top right of the file view.
- Make your changes and commit the changes.

**Use GitHub Codespaces**

- Navigate to the main page of your repository.
- Click on the "Code" button (green button) near the top right.
- Select the "Codespaces" tab.
- Click on "New codespace" to launch a new Codespace environment.
- Edit files directly within the Codespace and commit and push your changes once you're done.

## What technologies are used for this project?

This project is built with:

- Vite
- TypeScript
- React
- shadcn-ui
- Tailwind CSS

## How can I deploy this project?

### Option 1: Using Lovable
Simply open [Lovable](https://lovable.dev/projects/de9b67b4-7c44-4e57-ad7a-c5e7fbbb242a) and click on Share -> Publish.

### Option 2: Using Vercel
This project is configured for Vercel deployment. See the [Vercel Deployment Guide](./VERCEL_DEPLOYMENT.md) for detailed instructions.

### Option 3: Using Vercel CLI
Since you've already pushed this project to GitHub, you can deploy using the Vercel CLI:

1. Install the Vercel CLI globally:
   ```bash
   npm install -g vercel
   ```

2. Login to your Vercel account:
   ```bash
   vercel login
   ```

3. In your project directory, run:
   ```bash
   vercel
   ```

4. For production deployments, use:
   ```bash
   vercel --prod
   ```

For more details, see:
- [Vercel CLI Quick Start Guide](./VERCEL_CLI_QUICKSTART.md) - Simplified guide for CLI deployment
- [Vercel Deployment Guide](./VERCEL_DEPLOYMENT.md#deploying-with-vercel-cli) - Complete deployment documentation

## Can I connect a custom domain to my Lovable project?

Yes it is!

To connect a domain, navigate to Project > Settings > Domains and click Connect Domain.

Read more here: [Setting up a custom domain](https://docs.lovable.dev/tips-tricks/custom-domain#step-by-step-guide)
