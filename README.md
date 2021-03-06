# Zumasys Documentation

This is a [VuePress](https://vuepress.vuejs.org/) documentation application that leverages [GitHub](https://github.com) as the
repository of documentation. The repository is currently hosted in the [Zumasys GitHub](https://github.com/zumasys/docs) and the app
is available at [Zumasys BetaDocs](https://betadocs.zumasys.com). The documentation was created by way of
[HelpJuice-to-Markdown](https://github.com/itsxallwater/helpjuice-to-markdown).

## Directory structure

```text
├── site
│   ├── .vuepress
│   │   ├── components
│   │   ├── theme
│   │   ├── public
│   │   ├── styles
│   │   │   ├── index.styl
│   │   │   └── palette.styl
│   │   ├── config.js
│   ├── docs
│   │   ├── jbase (Note: jBASE documentation lives here)
│   │   ├── zumasys (Note: Zumasys documentation lives here)
│   │   └── README.md
│   ├── README.md (Note: The home page of the docs)
│   └── package.json
└── README.md (Note: You are here!)
```

## Development Steps

To run the application locally:

> You will need to have [Node.js & npm](https://nodejs.org/en/download/) installed. You'll also need [Git](https://git-scm.com/downloads).

1. `git clone https://github.com/zumasys/docs.git`
2. `cd docs` (or whatever name you used for your git clone)
3. `cd site`
4. `npm install` (Not necessary on subsequent builds)
5. Optionally, if you want the [Vssue](https://vssue.js.org/) plugin to work, you'll need to create a `.env` file in the `site` folder and add the appropriate credentials.

   > `cd site && code .env`

   ```dotenv
   # Environment Variables
   VUE_APP_GITHUB_CLIENT_ID=MyClientKey
   VUE_APP_GITHUB_CLIENT_SECRET=MySecretKey
   ```

6. `npm run dev`
7. When compilation completes you should see the following message

   > success [12:25:41] Build 59cc58 finished in 75022 ms!  
   > VuePress dev server listening at [http://localhost:8080/](http://localhost:8080/)

8. Open [localhost:8080](localhost:8080) in your browser.

## TODO - Contributor Guidelines

## TODO - Community Guidelines

## TODO - Contributors

- The entire [Zumasys Team](https://www.zumasys.com/about/our-people/)
- Andy Takacs ([@andytakacs](https://github.com/andytakacs))
- Mike Wright ([@itsxallwater](https://github.com/itsxallwater))
- Ryan Medina ([@ryannmedina](https://github.com/ryannmedina))
- Peter Falson ([@pfalson](https://github.com/pfalson))
- Mike Street ([@mikes-zum](https://github.com/mikes-zum))

## Todo List

- [x] Add sidebar links matching docs directory structure
- [ ] Clean up directory structure under the Zumasys folder (i.e. AccuTerm folder -> Mobile and Web)
- [x] Clean up root directory (move docs project into sub-dir)
- [ ] Add [Table of Contents](https://vuepress.vuejs.org/guide/markdown.html#table-of-contents)
- [ ] More [config](https://vuepress.vuejs.org/config/)
- [ ] More [theme config](https://vuepress.vuejs.org/theme/default-theme-config.html)
- [ ] More [customization](https://vuepress.vuejs.org/guide/markdown.html)
- [x] Pull images from HelpJuice into static assets of this project and update links
- [ ] Add [Vssue](https://vssue.js.org/) plugin for comments
- [ ] Add breadcrumbs/navigation trail to docs layout (not seeing a plugin or config for this so we'll do it in Vue)
- [ ] Add [Google Analytics](https://v1.vuepress.vuejs.org/plugin/official/plugin-google-analytics.html) plugin or the [minimal](https://github.com/webmasterish/vuepress-plugin-minimal-analytics) version
- [ ] Add [Clean URLs](https://vuepress.github.io/en/plugins/clean-urls) plugin (may not be necessary with current directory/README.md structure)
- [ ] Add [Git Log](https://vuepress.github.io/en/plugins/git-log/) plugin (to add Git data to \$page object)
- [ ] Add [Algolia Search](https://community.algolia.com/docsearch/) plugin ([more docs](https://vuepress.vuejs.org/theme/default-theme-config.html#algolia-docsearch))
- [ ] Add [nprogress](https://vuepress.github.io/en/plugins/nprogress/#installation) plugin (to show global page loading bar)
- [ ] Add [reading progress](https://github.com/tolking/vuepress-plugin-reading-progress) plugin (to show reading progress of a document)
- [ ] Add [TypeScript](https://vuepress.github.io/en/plugins/typescript/#installation) plugin (to allow use of TypeScript in VuePress `.vue` files)
- [ ] Add [check-md](https://github.com/ulivz/vuepress-plugin-check-md) plugin (to check for dead links in Markdown)
- [ ] Add [flowchart](https://flowchart.vuepress.ulivz.com/#install) plugin (to define flowcharts in docs)
- [ ] Add [export](https://github.com/ulivz/vuepress-plugin-export) plugin (to allow for export of all docs to PDF)
- [ ] Add [sitemap](https://github.com/ekoeryanto/vuepress-plugin-sitemap) plugin (to allow for auto creation of sitemap.xml file)
- [ ] Add [SEO](https://github.com/lorisleiva/vuepress-plugin-seo) plugin (for automatic SEO meta tag generation)
- [ ] Related to above, may also need [autometa](https://github.com/webmasterish/vuepress-plugin-autometa) plugin
- [ ] Add [reading time](https://github.com/darrenjennings/vuepress-plugin-reading-time) plugin (to show etsimated reading time for an article)
- [ ] Add [social share](https://github.com/ntnyq/vuepress-plugin-social-share) plugin (to activate social network share icons)
- [ ] Add [code copy](https://github.com/znicholasbrown/vuepress-plugin-code-copy) plugin (to allow for click-to-copy of source code)
- [ ] Add [img lazy](https://github.com/tolking/vuepress-plugin-img-lazy) plugin (to add lazy loading for images)
- [ ] Add [back to top](https://github.com/vuejs/vuepress/tree/master/packages/%40vuepress/plugin-back-to-top) plugin (for automatic back-to-top links)
- [ ] Check out more on [awesome-vuepress](https://github.com/vuepressjs/awesome-vuepress)
- [ ] Convert TODOs to GitHub Issues
- [ ] Add jBASE Basic, Jabba to [Prism](https://prismjs.com/#languages)
