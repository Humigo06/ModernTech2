# Workflow Analysis
Hunter Goss

## What triggers this workflow to run?

The triggers for this workflow are changes being pushed to the main branch or pull requests targeting the main branch.

## What are the four main steps this workflow performs?

1. Checkout code

2. Validate HTML

3. Check Links

4. Upload artifact

## What does the "Checkout code" step do and why is it necessary?

The "Checkout code" step downloads the repository code. Without this step, the GitHub Actions would not be able to check any of the code, since it would not have anything to check.

## What is the purpose of the environment configuration?

The purpose of the environment configuration is tell GitHub where to deploy its output. In this case, it outputs a URL leading to the website.

## How does this automated deployment improve reliability compared to manual deployment?

Manual deployment runs into difficulties with human error. Humans may forget a step or make an error during deployment. Automating the processes allows for every step to be taken every time, which insures code is tested and the right steps are taken. Additionally, automated deployment tests in a standarized environment, which reduces bugs.

## What would happen if you pushed code to a different branch?

If code was pushed to a different branch, none of the checks listed in deploy.yml would trigger. This is because the workflow only triggers from pushes or pull requests targeting the main branch.