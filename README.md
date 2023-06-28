## Introduction

Welcome to the documentation for the OpenAtlas Discovery (OAD) Content Repository. This repository serves as a central location for managing content and related assets for an OAD site. It includes a configuration file, content files, and directories for storing images, favicons, and logos. This documentation will guide you through the structure and usage of the repository.

## Repository Structure

The repository consists of the following elements:

1. `discoveryConfig.json`: This JSON file contains options for configuring the base behavior of the website. It defines the settings for various aspects such as default language, default filters, and other site-specific features. The configuration options in this file can be customized according to the requirements of your website.

2. `content/` directory: This directory holds the Markdown (`.md`) files that contain various content for the website. The content files may be organized in subdirectories for better organization and management. You can create new Markdown files or modify existing ones to update the content of your website.

3. `public/` directory: This directory contains the assets required by the website, including the favicon, logo, and images used throughout the site. It may also include subdirectories to further organize the images. The assets in the `public/` directory are typically referenced from the content files or the website's code.

## Usage

### Configuring the Website Behavior

To configure the behavior of the website, you can modify the `discoveryConfig.json` file. Open the file using a text editor and update the values of the available options according to your needs. The options provided in the file are documented at [OpenAtlas-Discovery: A presentation website for OpenAtlas projects.](https://github.com/craws/OpenAtlas-Discovery) in the documentation directory.

### Managing Content

The `content/` directory is where you can create and manage the content for your website. The content is written in Markdown format, which allows for easy formatting and structuring of text-based content. You can use any text editor or Markdown editor of your choice to create or modify the Markdown files.

When creating new content, you can either create the Markdown file directly inside the `content/` directory or create subdirectories within `content/` for better organization. It is recommended to follow a logical structure while organizing the content files in subdirectories, especially if your website has multiple sections or categories.

Example Structure
```
content/
├── team.md
├── about.md
├── articles/
│   ├── articel1.md
│   └── article2.md
└── news/
    ├── news1.md
    ├── news2.md
    └── subdirectory/
        └── news3.md
```

### Adding Assets

The `public/` directory is used to store the assets required by the website. It should contain the following elements:

- Favicon: The favicon is a small icon that represents your website. Place the favicon file (typically in `.ico` or `.png` format) directly inside the `public/` directory.
- Logo: The logo represents the visual identity of your website. It's recommended (though not necessary) to store the logo file directly inside the `public/` directory (as valid image file, e.g. `logo.png`, `logo.svg`, ...).
- Header Logo: The header logo is the logo displayed in the top bar of the site. It's requires and needs to be stored directly inside the `public/` directory as `header_logo.svg`.
- Images: The `public/` directory can also contain images that are used within the website's content. You can organize the images in subdirectories within the `public/` directory based on your requirements. Make sure to update the image URLs or references in the content files accordingly.

### Referencing Assets

To reference the assets stored in the `public/` directory within your content files, you can use relative paths. For example, if you have an image called `example.jpg` stored in `public/images/`, you can reference it in your content file using the following Markdown syntax:

```markdown
![Example Image](/images/example.jpg)
```

Make sure to adjust the path based on the location of the content file and the relative position of the image within the directory structure.

As reference, for this example the folder structure could look like this:

```
root/
├── discoveryConfig.json
├── content/
│   ├── index.md
│   ├── about.md
│   └── team.md
└── public/
    ├── favicon.svg
    ├── logo.svg
    └── images/
        └── example.png
```

## Conclusion

Congratulations! You are now familiar with the structure and usage of the Content Repository. By leveraging the `discoveryConfig.json` file, the `content/` directory, and the `public/` directory, you can manage and organize the content and assets of your website. Feel free to explore and customize the repository to meet the specific requirements of your project.
