# GitHub Deployment Protection Rules Playground

This repository serves as a demo for enabling deployment protection rules for target environments.

For demo purposes, be sure to follow the steps below:
* Fork this repo to your organization: https://github.com/github-technology-partners/protection-rules-playground/fork
* Enable GitHub Pages (see [GitHub Pages](#github-pages))
* Confirm Action workflow is running (see [Deploy](#deploy))
* Install GitHub demo application (see [DPR Validator](#dpr-validator))
* Install your protection rule application (be sure to include any configuration specific to your application)
* Enable environment protection rules (see [Protection Rules](#protection-rules))
* Run the workflow to see your rules in action!
<img width="1449" alt="Screenshot 2023-10-03 144008" src="https://github.com/github-technology-partners/protection-rules-playground/assets/84209/2fb8e4e9-ff20-4598-9454-5cd30b7f4e6f">

## GitHub Pages

To enable GitHub Pages for a repository, visit settings/pages
1. Visit settings/pages
2. Under "Build and deployment" choose GitHub Actions
3. Settings are autosaved
<img width="830" alt="Screenshot 2023-10-03 143704" src="https://github.com/github-technology-partners/protection-rules-playground/assets/84209/7abff956-699e-45a4-8db2-4e1637b7bdcf">

## Deploy

1. Click the Actions tab
2. Select "Deploy static content GitHub Pages" from the workflows list in the sidebar
3. Click "Run workflow" from a target branch (typically `main`)

## DPR Validator

For this demo, we have an application that will always approve an incoming request.

1. Visit https://github.com/apps/dpr-validator
2. Click install
3. Choose the org you forked this repo into
4. Select "Only select repositories"
5. Choose the fork of this repo
<img width="748" alt="Screenshot 2023-10-03 143839" src="https://github.com/github-technology-partners/protection-rules-playground/assets/84209/dd6195ec-24d0-4eda-b857-e2d5d8fb4f1e">

## Protection Rules

For demo purposes, be sure to configure the following:
1. Visit settings/environments
2. Select "github-pages"
3. Enable "Required reviewers" and choose a user from your organization
4. Enable a "Wait timer" with a time of 1 min
5. Enable "DPR Validator"
6. Enable your custom application
7. Click "Save protection rules"
<img width="832" alt="Screenshot 2023-10-03 143952" src="https://github.com/github-technology-partners/protection-rules-playground/assets/84209/2ca76a15-4124-40eb-a9ce-f7e3c2969459">
