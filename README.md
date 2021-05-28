# Set Up Continuous Deployment For create-react-app & netlify

Netlify has a feature where you can configure every push to the `main` branch on GitHub to trigger a new build/update on Netlify.

## Getting Started

- Go to GitHub and create a new repository (use public so instructors can check your work)
- In your `create-react-app` add the new GitHub remote link
- Confirm your `create-react-app` is now on GitHub

**IMPORTANT:** Make sure your app runs locally. If it does not run locally, there is no hope of it working on deployment.

**IMPORTANT:** With continuous deployment, you only want working code to be on `main`, use branches like `dev` to build and confirm a working app before merging into `main`.

## Netlify Settings

Log onto Netlify and go to `Team Overview`, select `New site from Git`

![](./assets/1.team-overview.png)

<br />
<hr />
<br />

Choose the `GitHub` button - this will take you to a GithHub authentication view
![](./assets/2.create-new-site.png)

<br />
<hr />
<br />

Scroll down and select `Configre the Netlify app on GitHub`

![](./assets/3.github-netlify-config.png)

<br />
<hr />
<br />

Choose configure to install Netfliy on your GitHub account

![](./assets/4.install-netlify-on-github.png)

<br />
<hr />
<br />

Be sure to remember your GitHub password in order to move forward

![](./assets/5.log-in-to-github.png)

<br />
<hr />
<br />

Choose which repo. Use the search bar feature, if needed.

![](./assets/6.select-repos.png)

<br />
<hr />
<br />

Once, selected, your view should return to the Netlify dashboard.

![](./assets/7.choose-repo-on-netlify.png)

<br />
<hr />
<br />

Keep default settings provided, and choose `Deploy site` button

![](./assets/8.create-configure.png)

<br />
<hr />
<br />

See status of your deployment. Click on it to see more details

![](./assets/9.see-status.png)

<br />
<hr />
<br />

Check the logs, it is good to get familiar with what is there. When errors occur with the build, this is where you would go to debug.

![](./assets/10.check-logs.png)

<br />
<hr />
<br />

Check for `Site is live ✨` - to confirm your site is live

![](./assets/11.site-is-live.png)

<br />
<hr />
<br />

Go to the `Deploys` tab and you can then click on the link to see your site life. You can also share this link with your friends and family!

![](./assets/12.deploys-view.png)

<br />
<hr />
<br />
