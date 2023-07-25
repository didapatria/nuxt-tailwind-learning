# Nuxt.js TailwindCSS - Learning
🚀 Dive into the world of ♻️ Nuxt.js and 🌀 Tailwind CSS! Learn to build stunning web apps with step-by-step tutorials, examples, and tips. Let's level up your web development skills! Let's create magic! ✨ #webdevelopment #javascript #vuejs #nuxtjs #tailwindcss

## Description:
This GitHub repository is dedicated to learning Nuxt.js and Tailwind CSS, two powerful tools for building modern, performant, and responsive web applications. The repository contains various projects, examples, and tutorials to help you grasp the fundamentals and advanced concepts of both Nuxt.js and Tailwind CSS.

Whether you are a beginner looking to understand the basics or an experienced developer seeking to enhance your skills, this repository provides a structured learning path, comprehensive documentation, and hands-on projects to cater to all skill levels. The combination of Nuxt.js and Tailwind CSS offers an excellent development experience, and you'll find everything you need to get started and create stunning web applications.

## Features:

- Step-by-step tutorials for setting up Nuxt.js projects with Tailwind CSS integration.
- Practical examples demonstrating the use of Nuxt.js features like routing, layouts, and data fetching.
- Comprehensive documentation explaining the core concepts of Nuxt.js and Tailwind CSS.
- Best practices and tips for optimizing and maintaining your projects.
- A collection of useful resources, links, and external references for further learning.

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#installation-and-setup-instructions">Installation and Setup Instructions</a>
      <ul>
        <li><a href="#create-your-project-with-yarn">Create your project with yarn</a></li>
        <li><a href="#install-nuxtjs-dependencies-and-tensorflow">Install Nuxt.js Dependencies and TensorFlow</a></li>
        <li><a href="#install-tailwind-css-with-prettier-plugin">Install Tailwind CSS with Prettier plugin</a></li>
        <li><a href="#add-tailwind-to-your-postcss-configuration">Add Tailwind to your PostCSS configuration</a></li>
        <li><a href="#configure-your-template-paths">Configure your template paths</a></li>
        <li><a href="#add-the-tailwind-directives-to-your-css">Add the Tailwind directives to your CSS</a></li>
        <li><a href="#import-the-css-file">Import the CSS file</a></li>
        <li><a href="#start-your-build-process">Start your build process</a></li>
      </ul>
    </li>
  </ol>
</details>

<!-- INSTALLATION AND SETUP INSTRUCTIONS -->

## Installation and Setup Instructions

Install Tailwind CSS with Nuxt.js and Setting up Tailwind CSS in a Nuxt.js project.

### Create a new react project with yarn

Start by creating a new Nuxt.js project if you don’t have one set up already. The most common approach is to use [**__Create Nuxt App__**](https://v2.nuxt.com/docs/get-started/installation/).

```bash
# Create New Project
$ yarn create nuxt-app nuxt-tailwind-learning

# To start the development server, navigate into the project directory
$ cd nuxt-tailwind-learning
```

### Install Nuxt.js Dependencies and TensorFlow

Install nuxt dependencies and tensorflow with yarn

```bash
# Install dependencies
$ yarn add nuxt axios @nuxtjs/eslint-module @nuxtjs/dotenvv @nuxt/image
```

### Install Tailwind CSS with Prettier plugin

Install `tailwindcss` and its peer dependencies via yarn, and then run the init command to generate a `tailwind.config.js` file.

```bash
$ yarn add -D tailwindcss prettier prettier-plugin-tailwindcss postcss autoprefixer
$ yarn tailwindcss init -p
```

### Add Tailwind to your PostCSS configuration

Add `tailwindcss` and `autoprefixer` to the `build.postcss.plugins` object in your `nuxt.config.js` file.

```js
export default {
  build: {
    postcss: {
      postcssOptions: {
        plugins: {
          tailwindcss: {},
          autoprefixer: {},
        },
      },
    },
  }
}
```

### Configure your template paths

Add the paths to all of your template files in your `tailwind.config.js` file.

```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "./components/**/*.{js,vue,ts}",
    "./layouts/**/*.vue",
    "./pages/**/*.vue",
    "./plugins/**/*.{js,ts}",
    "./nuxt.config.{js,ts}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### Add the Tailwind directives to your CSS

Create an `./assets/css/main.css` file and add the `@tailwind` directives for each of Tailwind’s layers.

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### Import the CSS file
Add the newly-created `./assets/css/main.css` file to the `css` array in the `nuxt.config.js` file.

```js
export default {
  css: [
    '@/assets/css/main.css',
  ],
}
```

### Start your build process

Run your build process with `yarn dev`.

```bash
# serve with hot reload at localhost:3000
$ yarn dev
```

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.
