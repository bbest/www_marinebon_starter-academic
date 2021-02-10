
# Creation

This site was created via the button at [Create a site with Github/Gitlab | Wowchemy: Website Builder for Hugo](https://wowchemy.com/docs/install/):

<a href="https://app.netlify.com/start/deploy?repository=https://github.com/wowchemy/starter-academic" target="_blank" class="btn btn-primary px-3 py-3">Create your <strong>resumé</strong> or <strong>academic site</strong> now with Github 🚀</a>

# Original...

<p align="center"><a href="https://wowchemy.com" target="_blank" rel="noopener"><img src="https://wowchemy.com/img/logo_200px.png" alt="Wowchemy Website Builder"></a></p>

# Academic Template for [Hugo](https://github.com/gohugoio/hugo)

The Hugo **Academic Resumé Template** empowers you to create your job-winning online resumé and showcase your academic publications.

[Check out the latest demo](https://academic-demo.netlify.app) of what you'll get in less than 10 minutes, or [view the showcase](https://wowchemy.com/user-stories/).

[**Wowchemy**](https://wowchemy.com) makes it easy to create a beautiful website for free. Edit your site in Markdown, Jupyter, or RStudio (via Blogdown), generate it with Hugo, and deploy with GitHub or Netlify. Customize anything on your site with widgets, themes, and language packs.

- 👉 [**Get Started**](https://wowchemy.com/docs/install/)
- 📚 [View the **documentation**](https://wowchemy.com/docs/)
- 💬 [Chat with the **Wowchemy community**](https://discord.gg/z8wNYzb) or [**Hugo community**](https://discourse.gohugo.io)
- 🐦 Twitter: [@wowchemy](https://twitter.com/wowchemy) [@GeorgeCushen](https://twitter.com/GeorgeCushen) [#MadeWithWowchemy](https://twitter.com/search?q=(%23MadeWithWowchemy%20OR%20%23MadeWithAcademic)&src=typed_query)
- 💡 [Request a **feature** or report a **bug** for _Wowchemy_](https://github.com/wowchemy/wowchemy-hugo-modules/issues)
- ⬆️ **Updating Wowchemy?** View the [Update Guide](https://wowchemy.com/docs/update/) and [Release Notes](https://wowchemy.com/updates/)

## Crowd-funded open-source software

To help us develop this template and software sustainably under the MIT license, we ask all individuals and businesses that use it to help support its ongoing maintenance and development via sponsorship.

### [❤️ Click here to unlock rewards with sponsorship](https://wowchemy.com/plans/)

## Ecosystem

* **[Wowchemy Admin](https://github.com/wowchemy/wowchemy-admin/):** An admin tool to import publications from BibTeX

[![Screenshot](https://raw.githubusercontent.com/wowchemy/wowchemy-hugo-modules/master/academic.png)](https://wowchemy.com)

<!--
[![Analytics](https://ga-beacon.appspot.com/UA-78646709-2/academic-kickstart/readme?pixel)](https://github.com/igrigorik/ga-beacon)
-->

## MBON Developer

### Automatic regeneration with Github Action 

- https://github.com/r-lib/actions/tree/master/examples

* [Chapter 3 Websites using pkgdown, bookdown, and blogdown | Github actions with R](https://ropenscilabs.github.io/actions_sandbox/websites-using-pkgdown-bookdown-and-blogdown.html#deploy-blogdown)

```r
usethis::use_github_action("blogdown")

# https://www.seanwarlick.com/post/setting-up-renv/
install.packages('renv')
renv::init()
install.packages('blogdown')
renv::settings$snapshot.type("simple")
renv::snapshot()
```

Per `.github/workflows/blogdown.yaml`, set secrets in the Github repo for:
- Github: `GITHUB_TOKEN`
  Go to https://github.com/settings/tokens, click "Personal access tokens" menu, "Generate new token" button. Actually, looks like this is already reserved, so did nothing to add.
- Netlify: `NETLIFY_AUTH_TOKEN`, `NETLIFY_SITE_ID`
  See: [Deploy your bookdown project to Netlify with Github Actions | Emil Hvitfeldt](https://www.hvitfeldt.me/blog/bookdown-netlify-github-actions/)


