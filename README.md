tlify Next.js Blog Template designed by Bejamas](https://user-images.githubusercontent.com/43764894/223762618-62742b4e-9424-44a7-8e85-9f7e4e19dbDeploy loy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/netlify-templates/nextjs-blog-theomizable using:nd](https:/and blog's name is "Next.js Blog Theme" with one blog post](nextjs-blog-theme-predemo.](https://bejamas-nextjs-blog.netlifyrough!](https://www.youtube.com/watch?v=63QZHs259dY)
arted)
y)


dependencies by running:
nstall
```

Finallywith:

```shell
yarn run dev


, your project shouldng the Setup Wizeviewtjs-setup-wizard.p-wizard.netlify.app/few clicks and deploy to Netl


The config is based on environment variables to make it easy to integrate with any Jamstack platform, like Netlify the es. ronment variable isn't your cup of tin the code base.RAPHS` are used in [`tailwind-preset.js`](tailwind-preset.js).maintain these templates. This template s-io/netlify-



In order to keep our project up-to-date with dependencies we use a tool called [Renovate](https://github.com/marketplace/renovate). If you’re not interested in this tooling, delete the `renovate.json` file and commit that onto your main branch.

For our testing, we use [Cypress](https://www.cypress.io/) for end-to-end testing. This makes sure that we can validate that our templates are rendering and displaying as we’d expect. By default, we have Cypress not generate deploy links if our tests don’t pass. If you’d like to keep Cypress and still generate the deploy links, go into your `netlify.toml` and delete the plugin configuration lines:

```diff

  package = "netlify-plugin-cypress"
-  [plugins.inputs.postBuild]
-    enable = true
-
-  [plugins.inputs]
-    ena

If you’d like to remove the `netlify-plugin-cypress` build plugin entirely, you’d need to delete the entire block above instead. And then make sure sure to remove the package from the dependencies using:

```bash
npm uninstall -D netlify-pl

And lastly if you’d like to remove Cypress entirely, delete the entire `cypress` folder and the `cypress.config.ts` file. Then remove the
