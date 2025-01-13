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
  
