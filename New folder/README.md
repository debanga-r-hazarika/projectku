# Project Setup Guide

This README provides instructions for setting up and running the project.

## Getting Started

### Step 1: Set up the Prototype Development Environment

1. Navigate to the 'prototype dev 2.0' folder
2. Install dependencies (only needed for first-time setup):
   ```
   npm i
   ```
3. Start the development server:
   ```
   npm run dev
   ```
4. The development server should now be running

### Step 2: Set up the Present Development Environment

# How to Run
## Setp the enviroment
```
python -m venv env
# (from your project root)
. .\env\Scripts\Activate.ps1
```

install requirements
```
pip install -r requirements.txt
```

## Run Original Script:
python original_script.py

## Run API:
python api.py

## Serve Website:
cd website
python -m http.server 8000

## Open Browser:
http://localhost:8000/


## Live Video Links:
Live 1 - https://youtu.be/_1PfF1v9GJc
Live 2 - https://youtu.be/mwN6l3O1MNI
Live 3 - https://youtu.be/EPKWu223XEg

1. Navigate to the 'Present Developement' folder
2. Follow the instructions in the readme.md file located in that folder:
   - To run the API: `python api.py`
   - To access the application in your browser, open: http://localhost:8000/

## Project Structure

- **prototype dev 2.0**: Frontend development environment
- **Present Developement**: Backend API and additional components

## Deployment

For deployment options, refer to the documentation in the 'prototype dev 2.0' folder:
- See VERCEL_DEPLOYMENT.md for deploying to Vercel

## Additional Information

For more detailed information about each component, please refer to the readme files in their respective directories.