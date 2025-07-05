---
title: "How to build your Blog for free on GitHub Pages using Jekyll"
date: 2025-06-28
categories: [ blog ]
tags: [ blog, git, setup ]
---

# Set up a blog on Git

The purpose of this post is to guide you through the process of setting up a blog on GitHub Pages using Jekyll. This
setup allows you to create a static website that can be hosted for free on GitHub. Credit goes to Ahmed Tremo who
recorded a video on youtube, which I will be following to set up my blog. You can find the
video [here](https://www.youtube.com/watch?v=m1RYsmOMPLs).

## Prerequisites

Before we begin, ensure you have the following prerequisites:

- A GitHub account
- Basic knowledge of Git and GitHub
- Ruby installed on your machine (Jekyll is a Ruby gem)
- Jekyll installed on your machine (you can install it using `gem install jekyll bundler`)
- A code editor (like Visual Studio Code, Atom, etc.)
- A terminal or command prompt

## Step 1: Create a New Repository

Go to this Github repository: [cotes2020/jekyll-theme-chirpy](https://github.com/cotes2020/chirpy-starter) and use
`Create a new repository` button to create a new repository. Name it `yourusername.github.io`, where `yourusername` is
your GitHub username. This is important as GitHub Pages uses this naming convention to host your site.

## Step 2: Modify the _config.yml file
Open the `_config.yml` file in your repository. This file contains the configuration settings for your Jekyll site.
1. Update the `title` and `description` fields to reflect your blog's name and description.
2. Set the `url` field to `https://yourusername.github.io`.
3. Wait for the github action to complete, you can check the status of the action in the `Actions` tab of your repository.
4. Once the action is complete, you can visit your blog at `https://yourusername.github.io` to see the default 
   Jekyll site. The page should look something like this:![image](/assets/img/chirpy.png)

## Step 3: Clone the repository locally and customize Your Blog
1. Clone the repository to your local machine and open the cloned repository in your code editor
2. Install Jekyll, you can follow the instructions in the [Jekyll documentation](https://jekyllrb.com/docs/installation/).
3. Modify the `_config.yml` file to customize your blog. You can change the title, description, avatar, author 
   information, and other settings. Note you can put your avatar image in the `assets/img` directory and update the 
   `avatar` field in `_config.yml` to point to your image. (e.g., `/assets/img/your-avatar.png`).
4. Run the following command in your terminal to build and serve your Jekyll site locally:
   ```bash
   bundle exec jekyll serve
   ```
5. Open your web browser and go to `http://localhost:4000` to see your blog locally.

## Step 4: Add Content to Your Blog
You can add new posts to your blog by creating Markdown files in the `_posts` directory. The file names should 
follow the format `YYYY-MM-DD-title.md`, where `YYYY-MM-DD` is the date of the post and `title` is a descriptive title for the post.
For example, to create a new post titled "My First Post" on June 28, 2025, you would create a file named 
`2025-06-28-my-first-post.md` in the `_posts` directory. The content of the file should follow the Jekyll front matter

## Congratulations!
That's it! You now have a basic blog set up on GitHub Pages using Jekyll. You can continue to customize your blog by adding themes, plugins, and more content. For more advanced features and customization options, refer to the [Jekyll documentation](https://jekyllrb.com/docs/).