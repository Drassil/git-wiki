---
redirect_from: /
published: true
---

# Welcome to git-wiki demo!

This is both documentation and [demo](Demo.md) of [git-wiki theme](https://github.com/Drassil/git-wiki-theme) project.

it's a **modular and full featured wiki** powered by git, [github](https://pages.github.com/)/[gitlab](https://about.gitlab.com/product/pages/) pages and pull-requests!

The git-wiki project is composed by 3 different repository:

- [git-wiki-theme](https://github.com/Drassil/git-wiki-theme): This is the repository of the theme that implements the wiki functionalities. You would have not fork it unless you need to send a Pull Request or create your wiki project from scratch.

- [git-wiki-skeleton](https://github.com/Drassil/git-wiki-skeleton): This is the repo that you should fork or use as a template. It uses the [jekyll remote theme](https://github.com/benbalter/jekyll-remote-theme) functionality that allows you to create your own wiki based on git-wiki-theme. By using the remote functionality you can automatically keep your wiki always updated with latest features from the **git-wiki-theme**, but you can also fully customize it. 

- [git-wiki](https://github.com/Drassil/git-wiki): This is the documentation repository and website of the **git-wiki-theme** project. You would have not fork it unless you want to contribute to the git-wiki project documentation.

## Getting started

The easier and faster way to use git-wiki is the "skeleton" method.

**You don't need to install anything locally!**

1. Simply fork/clone [skeleton repo](https://github.com/Drassil/git-wiki-skeleton) or click on "Use this template" button to create your copy of the skeleton project.

2. Edit _config.yml and other pages as you need and then deploy it on github/gitlab pages.

**Done**! now wait that your page will be published and you're ready **_to wiki_**!

For more installation options see the [Installation instructions](#installation-instructions)

## Features 

* Improvements in the **cooperative** aspect: forks, pull-requests and roles.
* You can **customize your wiki** as you want with style sheets and even changing the layout. (see customization section below) 
* **No databases!** Only static files that can be downloaded in a few seconds.
* **Blazing fast** and free thankfully to Github/Gitlab Pages and Jekyll Server Side Generation process!
* **Markdown and html** mixed together!
* **Multiple free search engines!** on a static site!
* **History, revision comparison** and everything you need from a wiki platform.
* You can **edit your pages** with the standard git editor, prose.io (integrated) or any kind of editor you prefer.
* Non-existent wiki page links are "[red](red.md)", you can **click on them to automatically create a new page**!
* [External links](http://www.google.com) get the right icon automatically
* **Component system with hooks** that allows you to totally customize your wiki UI. (see customization section below) 
* Some **nice internal themes** to change your entire wiki UI with 1 simple configuration (see customization section below)
* Integrated **Blogging** feature thanks to jekyll!
* Automatic generated **TOC**
* You can download the entire wiki for **offline** usage and even navigate directly using a markdown reader


You can use it with jekyll ["remote_theme"](https://github.com/benbalter/jekyll-remote-theme) feature or fork/copy the master branch  and start your wiki in just 1 minute*.

Git-wiki can be used as [theme for jekyll](https://jekyll-themes.com/git-wiki/)

 *Github/Gitlab pages takes about 10 minutes to show up the first time you configure it

**Note:**
You can even include the [official github wiki](https://help.github.com/articles/about-github-wikis/) as a submodule and enable the option in our conf file to use github wiki pages in git-wiki system, but it's an experimental feature and it implies less advantages and greater disadvantages for now.

## Who is using git-wiki

[List of git-wiki installations](examples.md)

[List of forked repository](https://github.com/Drassil/git-wiki-theme/network/members)


### [Share your wiki with us!](examples) and keep the "Powered by Git-Wiki" footer link please. It will help both of us!


## Installation instructions

### Remote theme method

1. Fork, Clone [the skeleton repository](https://github.com/Drassil/git-wiki-skeleton) or click on "Use this template" button to create your copy.

2. Edit _config.yml and other pages as you need and then deploy it on github/gitlab pages.

**Description**: This method will allow you to create a wiki based on our skeleton repository and that extends git-wiki-theme. 

**Direct installation comparison**:

 + **pros**: This will allow you to avoid upgrading process pulling files from git-wiki-theme and eventually merge them.

 - **cons**: To edit/fix git-wiki-theme core files you need to configure a second repository forked by git-wiki-theme repo. However, [YAGNI](https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it)

**GITLAB SUPPORT**: if you want to fork the skeleton from gitlab, you can use [this repo](https://gitlab.com/drassil/git-wiki-skeleton)

**Without skeleton**: you can avoid to use the skeleton repository if you want start from scratch, however it's important to use at leaset the configuration variables needed by the theme: [_config.yml](https://github.com/Drassil/git-wiki-skeleton/blob/master/_config.yml)

### Direct installation method

1. Fork, Clone [git-wiki-theme repository](https://github.com/drassil/git-wiki-theme) or click on "Use this template"

2. Edit _config.yml and push your changes in your repository, then configure the github/gitlab pages in your repository settings

**Description**: This method will allow you to create a wiki using git-wiki-theme directly. You can create your theme from scratch. It's for advanced users and people who want directly collaborate to git-wiki-theme project.

**Remote installation comparison**:

 + **pros**: You can build your wiki and collaborate with git-wiki-theme project by PR at the same time.

 - **cons**: Upgrading your wiki to the latest version need a merge with git-wiki-theme repo.


### Notes:
In both cases please is preferred to use **Fork** instead of **Template** and **Template** instead of **Clone** (Fork > Template > Clone).
Fork will allow you to make pull request to/from original repository to keep your files updated (for skeleton too). Please, keep everything open and collaborative!


### Local development

If you need to work on git-wiki locally before publish, then clone your wiki repo and follow this instructions 
from official github article: <https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/>
Git wiki already contains the Gemfile for local installations.

You can also use our **docker files** to run git-wiki under **docker**, 
the easiest method is to run `docker-compose up` command in this folder

## Configuration and customization

* [How to customize your wiki](customize.md)

* [How to setup the search feature](search-feature.md)

## Current known limitations

* You can't use the wiki internal link format: [[example]]. Please, use gh-pages links instead: \[example\](example) . It's a known jekyll limitation: <https://jekyllrb.com/docs/templates/>


## Support & Collaboration

You can open a public issue on [github](https://github.com/Drassil/git-wiki/issues) , 
send a private <a href="mailto:staff-drassil@googlegroups.com">email</a>  or create a PR to improve it.

Thank you!

## Components used

- [jekyll-toc](https://github.com/allejo/jekyll-toc)

- [jQuery](https://jquery.com/) for DOM manipulation

[MIT LICENSE](LICENSE)
