# Getting Started with the UNDP Accelerator Labs Toolkit Micro-site

Welcome to the UNDP Accelerator Labs Toolkit Micro-site project! This README provides a quick guide on how to set up and customize your Toolkit site.

## Table of Contents

- [Introduction](#introduction)
- [Toolkit Webpage Sample](#toolkit-webpage-sample)
- [Folder Structure](#folder-structure)
- [Tutorials](#tutorials)
- [Customizing Configuration](#customizing-configuration)
- [Set Up the Toolkit Micro-site Locally](#set-up-the-toolkit-micro-site-locally)
- [License](#license)

## Introduction

The Toolkit micro-site is built using Jekyll, a static site generator. It allows you to create documentation websites with ease. Follow the steps below to get started.

## Toolkit webpage sample
The toolkit generated from this template will look like [this](https://undp-accelerator-labs.github.io/national_innovation_ecosystems_toolkit/). There is flexibility for minimum configuration of text, header, color, logo, background, etc.

## Folder Structure

Here's the recommended folder structure for your NIE Toolkit project:
```markdown
├── index.md # This is the home page
├── _data/
│ ├── site_info.yml # Customize site configuration here
├── _layouts/
│ ├── default.html # Default layout template
content
│ ├── getting-started/
│ ├── index.md # Getting started side menu config
│ │ ├── values.md # Example page under the Getting Started category
│ ├── Second Topic/
├── index.md # Side menu config
│ │ ├── values.md # Example page new sub topic
├── public/
│ ├── imgs/ # Image files
├── _config.yml # Jekyll configuration file
├── README.md # Instructions for users (you're reading this)

``````


### Customizing the Contributors Page

The current version of this template incorporates both a contributor profile page and a contributors list page. If you wish to integrate these pages into your website, you must update the `_data/contributors.yml` file with a list of your project's contributors.

To access an individual contributor's profile page, you can link to the respective profile using the ID from your `_data/contributors.yml` file. For example: `[Jane Doe]({{ site.baseurl }}/contributors/Jane-doe.html)` directs to Jane Doe's profile based on the YAML file.

If you decide not to display the contributors page in your side menu, you can exclude it by adding `Team.md` to the `excludes` list in your `_config.yml` file.

## Tutorials
To familiarize yourself with using the toolkit, from setting up your account to creating folders/files, pages, subtopics, reviewing changes, and publishing them to the live toolkit website, check out the [Tutorials section](./Tutorials/index) for a step-by-step guide.

## Customizing Configuration

You can customize the site's configuration by editing the `_data/site_info.yml` and `_data/site_styles.yml` files. These files contain settings for the site's title, background color, and more.

It is also important to update the value of `baseurl` in `_config.yml` file. 
For navigation and menu customization, update the nav.html and sidebar.html partials.

That's it! You're ready to create, customize, and deploy your Toolkit site. Have fun documenting and sharing your content!


## Set Up the Toolkit Micro-site Locally

Follow these steps to set up the UNDP Accelerator Labs Toolkit Micro-site locally on your computer for development and customization:

1. **Clone the Repository**: Open your terminal or command prompt and navigate to the directory where you want to clone the repository. Then, run the following command to clone the repository to your local machine:

    ```markdown
    git clone https://github.com/UNDP-Accelerator-Labs/toolkit-micro-site-template.git
    ```

2. ### Navigate to the Repository

Change your current directory to the cloned repository:

```markdown
cd toolkit-micro-site-template
```

3. Install Dependencies
Ensure you have Ruby and Bundler installed on your computer. If not, you can install them following these instructions. Then, install the required dependencies by running:

```markdown
    bundle install
```

5. Run the Local Server
Start the local development server by running the following command:

```markdown
bundle exec jekyll serve 
```

This command will build the site and start a local server. You'll see an output with a URL like http://127.0.0.1:4000/. Open this URL in your web browser to view your locally hosted toolkit micro-site.

## License
This project is licensed under the Creative Commons Attribution 4.0 International License.

You can view the full license text [here](https://creativecommons.org/licenses/by/4.0/legalcode).

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
