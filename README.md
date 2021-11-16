# Set Up Continuous Deployment For create-react-app & netlify

Netlify has a feature where you can configure every push to the `main` branch on GitHub to trigger a new build/update on Netlify.

## Getting Started

- Go to GitHub and create a new public repository.
- In your `create-react-app` add the new GitHub remote link.
- Confirm your `create-react-app` code is now on GitHub.

**IMPORTANT:** Make sure your application runs locally. If it does not run locally, there is no hope of it working on deployment.

**IMPORTANT:** With continuous deployment, you only want working code to be on `main`, use branches like `dev` to build and confirm a working app before merging into `main`.

**IMPORTANT:** Deploy early and often. The best time to deploy is right after you run `create-react-app` - the less code you have written, the less work it will take to debug each deployment, in case there is an issue. 

## Netlify Settings

Log onto Netlify and go to `Team Overview`, select `New site from Git`.

![](./assets/1.team-overview.png)

Choose the `GitHub` button - this will take you to a GithHub authentication view.

![](./assets/2.create-new-site.png)

Scroll down and select `Configure the Netlify app on GitHub`.

![](./assets/3.github-netlify-config.png)

Choose configure to install Netfliy on your GitHub account.

![](./assets/4.install-netlify-on-github.png)

Be sure to remember your GitHub password in order to move forward.

![](./assets/5.log-in-to-github.png)

Choose which repo. Use the search bar feature, if needed.

![](./assets/6.select-repos.png)

Once selected, your view should return to the Netlify dashboard.

![](./assets/7.choose-repo-on-netlify.png)

Keep the default settings provided and choose `Deploy site` button.

![](./assets/8.create-configure.png)

See the status of your deployment. Click on it to see more details.

![](./assets/9.see-status.png)

Check the logs. It is good to get familiar with what is there. When errors occur with the build, this is where you would go to debug.

![](./assets/10.check-logs.png)

Check for the line `Site is live ✨` to confirm your site is live.

![](./assets/11.site-is-live.png)

Go to the `Deploys` tab and you can then click on the link to see your site live. You can also share this link with your friends and family!

![](./assets/12.deploys-view.png)

In order to continue to update your Netlify live site:

- On the `main` branch, confirm that your app works. While working on your app, be sure to work on another branch like `dev` and then only merge into `main` when your new features are working.
- Add, commit, and push your code to main.
   ```bash
   git add -A
   git commit -m "New feature added"
   git push origin main
   ```
- Give your site a few minutes to build.
- Be sure to check the dashboard and live site to make sure everything is working right.
