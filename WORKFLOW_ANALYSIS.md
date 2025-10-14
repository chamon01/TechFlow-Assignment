# Workflow Analysis

1. **What triggers this workflow to run?**  
   The workflow is triggered by a push or pull request to the **main** branch as shown in the `on:` section of the deploy.yml file.

2. **What are the four main steps this workflow performs?**  
   - Checkout code  
   - Setup Node.js environment  
   - Build and validate the project (HTML validation, check for broken links)  
   - Deploy to GitHub Pages  

3. **What does the "Checkout code" step do and why is it necessary?**  
   It pulls the repository code into the runner so the workflow has access to the files. Without this step, no code would be available to build or deploy.

4. **What is the purpose of the environment configuration?**  
   The environment configuration sets the runtime (like Node.js version) and permissions needed to deploy. This ensures consistency no matter who runs the workflow and prevents failures caused by mismatched environments.

5. **How does this automated deployment improve reliability compared to manual deployment?**  

6. **What would happen if you pushed code to a different branch (not main)?**  
   The workflow would not run, so the website would not deploy. Only changes to the main branch trigger the deployment.
