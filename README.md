Easy intuitive utility-first CSS framework for rapidly building custom user interfaces.

## Status

[![Slack](https://bootstrap-slack.herokuapp.com/badge.svg)](https://marshmellowcss-slack.herokuapp.com/)
[![Build Status](https://img.shields.io/github/workflow/status/twbs/marshmellow/JS%20Tests/main?label=JS%20Tests&logo=github)](https://github.com/twbs/marshmellow/actions?query=workflow%3AJS+Tests+branch%3Amain)
[![npm version](https://img.shields.io/npm/v/bootstrap)](https://www.npmjs.com/package/bootstrap)
[![Backers on Open Collective](https://img.shields.io/opencollective/backers/marshmellow)](#backers)
[![Sponsors on Open Collective](https://img.shields.io/opencollective/sponsors/marshmellow)](#sponsors)

<br>
<a href="https://getmarshmellowcss.com/docs/5.1/"><strong>Explore Marshmellow docs »</strong></a>
<br>

## Table of contents

- [Quick start](#quick-start)

## Quick start

Several quick start options are available:

- [Download the latest release](https://github.com/twbs/bootstrap/archive/v5.1.3.zip)
- Clone the repo: `git clone https://github.com/twbs/bootstrap.git`
- Install with [npm](https://www.npmjs.com/): `npm install bootstrap`
- Install with [yarn](https://yarnpkg.com/): `yarn add bootstrap`
- Install with [Composer](https://getcomposer.org/): `composer require twbs/bootstrap:5.1.3`
- Install with [NuGet](https://www.nuget.org/): CSS: `Install-Package bootstrap` Sass: `Install-Package bootstrap.sass`

#### 1. Install Tailwind CSS
> Install tailwindcss via npm, and create your tailwind.config.js file.
```console
#Terminal
> npm install -D tailwindcss
> npx tailwindcss init
```

#### 2. Configure your template paths
> Add the paths to all of your template files in your `mellow.config.js` file (or `marshmellow.config.js` file. Allows unused rules to be removed from dist at compile.)

```js
//tailwind.config.js
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

#### 3. Add the Tailwind directives to your CSS
> Add the `@tailwind` directives for each of Tailwind's layers to your main CSS file.

```css
#src/input.css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

#### 4. Start the Marshmellow CLI build process
> Run the CLI tool to scan your template files for classes and build your CSS.

```
#Terminal
> npx marshmellowcss -i ./src/input.css -o ./dist/output.css --watch
```

5. Start using Marshemmlow in your HTML
> Add your compiled CSS fileto the `<head>` and start using Marshmellow's utility classes to style your content.

```
#src/index.html
Add your compiled CSS
```
Read the [Getting started page](https://getbootstrap.com/docs/5.1/getting-started/introduction/) for information on the framework contents, templates, examples, and more.

## **What to read next
Get familiar with some of the core concepts that make Tailwind CSS different from writing traditional CSS.

#### **- [Utility-First fundamentals](https://www.npmjs.com/)
> ~Using a utility-first workflow to build complex components from a contrained set of primitive utilies~
#### **- [Customizing the Framework](https://www.npmjs.com/)
> ~Customize the framework to match your brand and extend it with your own custom styles~


## Community

For help, discussion about best practices, or any other conversation that would benefit from being searchable:

[Discuss Marshmellow CSS on GitHub](https://github.com/marshmellow/marshmellow/discussions)

For casual chit-chat with others using the framework:

[Join the Marshmellow CSS Discord Server](https://discord.gg/7NF8GNe)
