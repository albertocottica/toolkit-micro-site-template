## Creating a Folder
1. Navigate to the repository or branch where you want to create a folder.
2. Click on `Add file` and then `Create new file`.
3. In the `Name your file...` box, type the name of your new folder followed by a `/` (e.g., `Tutorial/`). The text box will then automatically create another box for you to create a new file within that folder.

![Create a branch](./assets/create-folder.png)

## Creating a File
1. Navigate to the repository or branch where you want to create a file.
2. Click on `Add file` and then `Create new file`.
3. In the `Name your file...` box, type the name of your new file (e.g., `new_file.md`).
4. Write your content in the `<>Edit new file` tab.
5. Scroll down to the bottom of the page, write a commit message, and click `Commit new file`.

## Uploading Files
1. Navigate to the repository where you want to upload files.
2. Click on `Add file` and then `Upload files`.
3. You can either drag and drop files or click `choose your files`.
4. After you've chosen your files, scroll down, write a commit message, and click `Commit changes`.

Remember, always write meaningful commit messages to help others understand what changes you've made. Happy coding! 😊


## Creating Pages on the Toolkit

To organize your content effectively, it's recommended to create a new folder for each topic, with subfiles representing different subtopics under it. Here's an example of how you can structure your pages:

```markdown
    * Policy making
        * index.md
        * values-of-creating-new-policy.md
        * how-to-create-national-policy.md
```


### Creating a New Topic with sub-topics

1. Create a new folder in the root directory with a meaningful name for your topic. For example, `policy-making`.

2. Inside the new folder, create an `index.md` file. This file will serve as the configuration for the topic in the menu.

3. In the `index.md` file, add Jekyll's front matter to specify the metadata for the topic. Provide the `title` of the topic as it should appear in the menu and the `menu` hierarchy order for its position in the menu tree.

Example `index.md` content:

```markdown
---
title: Policy making  # This is the title of the topic in the menu list
menu: 2  # This is the hierarchy of this topic in the menu tree
---
```


### Creating Subtopics
1. Inside the same topic folder, create additional .md files for each subtopic you want to cover. For example, `values-of-creating-new-policy.md ` and `how-to-create-national-policy.md`.
Use Jekyll's front matter in each subtopic file to specify metadata such as title, parent, layout, and nav_order.
Example subtopic content:
```markdown
---
title: Values of Creating New Policy
parent: Policy making
layout: default
nav_order: 1
---
```


2. Add your content using Markdown syntax to each subtopic file.
By following this structure, you can easily organize and create a hierarchy of topics and subtopics in your Toolkit micro-site.


### Creating a Main Topic (Without Sub-Topics)

To generate a main topic without any sub-topics, follow these steps. For instance, if you intend to establish a topic named "Contributors" as a menu list item, directing to a contributors page, you can achieve this by creating a file named `Team.md`.

In the created file, it's crucial to set the `has_children` property to `false`. This ensures that topics lacking sub-topics are correctly displayed in the menu list.