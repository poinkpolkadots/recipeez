# [Recipeez Jekyll theme](github.com/poinkpolkadots/recipeez)
[![LICENSE](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/poinkpolkadots/recipeez/master/LICENSE)
[![Jekyll](https://img.shields.io/badge/jekyll-%3E%3D%203.7-blue.svg)](https://jekyllrb.com/)

An easy to use theme to help you keep track of or publish your recipes.

## How to use this theme
recipeez is designed to be as easy to use as possible. In order to start up your own website, you can utilize [GitHub Pages](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll), which hosts your website for free.

Below are the steps to get started with GitHub Pages.

## Step one, clone this GitHub Repository
To clone this respository, click on the "fork" button in the upper right hand of this page:

![Fork Icon](/readme_pictures/fork_icon.png)

You must name the repository `<username>.github.io`.

Your website will be visible at `https://<username>.github.io`.

- To change the title of the website: edit `title                    : "My Awesome Website"` in `config.yml`.
- You can edit some other basic information in `config.yml`.
- To remove the link to the tutorial page in the heading, you can edit `/_data/navigation.yml` and remove the lines it says to

### Files you can remove

- `README.md`
- `/readme_pictures`


## Step two, add recipes!
You can put all recipes in the `_posts` folder in this repository.

Recipes are written in markdown, don't worry though, it's not that hard! You should title your post files like this: `YYYY-MM-DD-name-of-post.md`.

I recommend [this tutorial](https://www.markdowntutorial.com/) to learn the basics of markdown, but a few example pages are provided in this repository to help you get started. To create and edit markdown files, I recommend you use [Visual Studio Code](https://code.visualstudio.com/docs/languages/markdown), as it allows you to preview markdown files directly. You can download it [here](https://code.visualstudio.com/Download).

You can add pictures to your recipes using this format: `![alt text](/path/to/image)`. I recommend you store your pictures in `./assets/images` to make them easy to find.

To upload markdown files to your GitHub repository, you can utilize the GitHub website and click the "upload" button there, or you can clone your repository remotely and edit files that way, although that is a little more technical. I recommend using the website for beginners.

### Front Matter

At the top of the markdown file, you should include some "front matter", enclosed in triple dashes. It will look something like this:

![front matter example](/readme_pictures/front_matter_example.png)

To add new authors, you can add them to the `/_data/authors.yml`, then, in the front matter you can just refer to the author by what you named them in the yaml file. Easy peasy!

![authors.yml example](/readme_pictures/authors_example.png)

Front matter gives the website some basic information to display and sort the page by. To see all of all front matter tags, look at the Minimal Mistakes website [here](https://mmistakes.github.io).

### Recipe Content

You can look at the example pages provided to get an idea of some of the content that you can put in your recipe page, and how to do it. You have the ability to fully customize how your recipes look using markdown, so go wild!

## Step three, customize more!

Once you've set up your basic page, I recommend trying to customize it! You can customize any of the files in here to get your desired look. The `_layouts` folder includes the baseline html pages which are used to construct pages from your markdown files. The styling is done through the sass files in the `_sass`. I recommend [this tutorial](https://jekyllrb.com/docs/themes/) to learn how jekyll themes are laid out. You can also look at the [Minimal Mistakes website](https://mmistakes.github.io) for further documentation.

### Author profile

The author profile is disabled by default on this theme. If you want to re-enable it, you should go to `_config.yml` and change `author_profile: false` to `author_profile: true`. or include `author_profile: true` in the front matter of your markdown file.

### Asides

An additional feature has been included to add "asides" to your recipes to add tips and tricks into the body of the text. To utilize this feature, just create a div with the class of aside-box like this: `<div class="aside-box" markdown="1">`.

# Thanks for checking out recipeez!

Based on [Minimal Mistakes](https://github.com/mmistakes) by Michael Rose