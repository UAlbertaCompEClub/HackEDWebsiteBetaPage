# HackEDWebsiteBetaPage
Pulls information from HackEDWebsite. Exists so as to host a github page along side the main page

## Premise
Inorder to make use of gh-pages while maintaining the git structure of the HackEd repo, we want to take upstream code from the
HackEd repo and run the publish command so that the latest code will be built and deployed to this repo.

## General steps
Run the following in the terminal:

git remote add upstream https://github.com/UAlbertaCompEClub/HackEDWebsite.git  
git pull upstream  
git checkout HackEd_Beta  
npm run install  
npm run deploy

What this does is get the code from the source code branch, checks out the beta branch,
installs the software needed to deploy the code, and then deploys the code to this repo's gh-page.

When the initial set up is down, the only commands that need to be run would be `git pull upstream` and `npm run deploy`

## Roadmap
Bash scripts could be made for ease of access. Ideally the script to deploy to this would be from the source code repo.
