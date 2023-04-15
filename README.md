tlify Next.js Blog Template designed by Bejamas](https://user-images.githubusercontent.com/43764894/223762618-62742b4e-9424-44a7-8e85-9f7e4e19dbDeploy to Netlify Button](https://www.netm/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/netlify-templates/nextjs-blog-theomizable using:nd](https:/com/) v1 supof blog theme. Author named Jay Doe and blog's name is "Next.js Blog Theme" with one blog post](nextjs-blog-theme-predemo.](https://bejamas-nextjs-blog.netlifyrough!](https://www.youtube.com/watch?v=63QZHs259dY)
arted)
y)
  - [Using thenavigate to it in your terminal.

dependencies by running:
nstall
```

Finallywith:

```shell
yarn run dev
```

Open your browser and visit <http://localhost:3000>, your project shouldng the Setup Wizeviewtjs-setup-wizard.p-wizard.netlify.app/), you can create your blog in a few clicks and deploy to Netlify.



The config is based on environment variables to make it easy to integrate with any Jamstack platform, like Netlify the es. You can do this in your Netlify dashaboard e7-9ironment variable isn't your cup of tin the code base.

- `BLOG_THEME, BLOG_FONT_HEADINGS, & BLOG_FONT_PARAGRAPHS` are used in [`tailwind-preset.js`](tailwind-preset.js)
3611928/152727802-102ec296-41c8-446d-93ed-922d11187073.maintain these templates. This template s-io/netlify-plugin-cypress) - to run our tests during our build process

If your team is not interested in this tooling, you can remove them with ease!

### Removing Renovate

In order to keep our project up-to-date with dependencies we use a tool called [Renovate](https://github.com/marketplace/renovate). If you’re not interested in this tooling, delete the `renovate.json` file and commit that onto your main branch.

### Removing Cypress

For our testing, we use [Cypress](https://www.cypress.io/) for end-to-end testing. This makes sure that we can validate that our templates are rendering and displaying as we’d expect. By default, we have Cypress not generate deploy links if our tests don’t pass. If you’d like to keep Cypress and still generate the deploy links, go into your `netlify.toml` and delete the plugin configuration lines:

```diff
[[plugins]]
  package = "netlify-plugin-cypress"
-  [plugins.inputs.postBuild]
-    enable = true
-
-  [plugins.inputs]
-    enable = false
```

If you’d like to remove the `netlify-plugin-cypress` build plugin entirely, you’d need to delete the entire block above instead. And then make sure sure to remove the package from the dependencies using:

```bash
npm uninstall -D netlify-plugin-cypress
```

And lastly if you’d like to remove Cypress entirely, delete the entire `cypress` folder and the `cypress.config.ts` file. Then remove the depend
npm uninstall cy
