# Workflow Analysis

1. **What triggers this workflow to run?**  
   It runs anytime I push new code to the `main` branch.

2. **What are the four main steps this workflow performs?**  
   - **Checkout code** – grabs the files from the repo.  
   - **Validate HTML** – checks the HTML for mistakes.  
   - **Check links** – makes sure links aren’t broken.  
   - **Deploy** – puts the site live on GitHub Pages.  

3. **What does the "Checkout code" step do and why is it necessary?**  
   This step pulls in my project files so the other steps can test and deploy them. Without it, the workflow wouldn’t have any files to work with.

4. **What is the purpose of the environment configuration?**  
   It sets things up so the site knows where and how it should be deployed.

5. **How does this automated deployment improve reliability compared to manual deployment?**  
   It reduces human error, ensures tests/validations are run automatically, and makes deployment consistent every time code is pushed. This also saves developers time since they don’t need to manually check and deploy everything.

6. **What would happen if you pushed code to a different branch (not main)?**  
   Nothing would happen until that branch gets merged into `main`, since the workflow only watches `main`.