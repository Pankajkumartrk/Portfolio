# Portfolio

# step 1 create a { npm run build } if project complete and runable 
# step 2  Add a homepage to package.json  [ "homepage": "https://your-username.github.io/your-repository-name"]
# Step 3 Install GitHub Pages Package [npm install gh-pages --save-dev ]

# Step 4 Update the scripts section in your package.json file to include deployment commands:
"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
}


# Step 4: Push Your Project to GitHub
[
git init
git add .
git commit -m "Initial commit"

]
# step 5 Create a new repository on GitHub (name it something like my-portfolio).

Add the remote and push your code: 
git remote add origin https://github.com/your-username/your-repository-name.git
git branch -M main
git push -u origin main  

# step 6 Step 5: Deploy to GitHub Pages  
npm run deploy
This will:

Build your app.
Push the build/ folder to a special gh-pages branch on GitHub.
  # step 7 : Enable GitHub Pages  .
  Go to your GitHub repository in your browser.
Click on Settings > Pages (in the sidebar).
Under Source, choose the gh-pages branch.
Save the changes.

# Step 8: Access Your Live Portfolio   After enabling GitHub Pages, your portfolio will be live at:
   #----------------------------------------------------------------------------------------------------------- CI /CD live update and changes ----------------

your-repository-name/
│
├── public/                     # Public folder for static files (React default)
│   ├── index.html              # Main HTML file
│   └── ...                     # Other static assets (favicon, manifest, etc.)
│
├── src/                        # Source folder for your React components
│   ├── App.css                 # Main CSS file
│   ├── App.js                  # Main React component
│   ├── index.js                # Entry point for the React app
│   └── ...                     # Other components, styles, assets, etc.
│
├── .github/                    # Folder for GitHub-specific configuration
│   └── workflows/              # Folder for GitHub Actions workflows
│       └── deploy.yml          # GitHub Actions CI/CD workflow file
│
├── build/                      # Build folder (created by `npm run build`)
│   ├── index.html              # Final HTML file for deployment
│   ├── static/                 # Minified CSS, JS, and media files
│   └── ...                     # Other build assets
│
├── package.json                # Project metadata and dependencies
├── package-lock.json           # Lock file for npm dependencies
├── README.md                   # Documentation file for your repository
├── .gitignore                  # Files to ignore in Git
└── node_modules/               # Installed npm dependencies (auto-generated)












   # Step 1: Create the Workflow File
  In your existing repository, create a folder called .github (if it doesn’t already exist).
 Inside .github, create another folder named workflows.
Inside the workflows folder, create a file called deploy.yml.

# step 2 Step 2: Add the Workflow Configuration
Add the following configuration to deploy.yml. This file tells GitHub Actions what to do when you push changes to the repository.

# Step 3: Push the Workflow File to the Repository
Save the deploy.yml file.
Commit and push it to your repository:
bash
Copy code  ----------
      git add .github/workflows/deploy.yml
git commit -m "Add GitHub Actions workflow for CI/CD"
git push origin main


