# Tailwind Learning Mini Projects

This repository is a collection of Tailwind CSS mini projects aimed at improving skills with Tailwind and exploring various techniques, layouts, and components. The projects are built using Webpack, and the repository includes two starter templates to help you get started quickly: `webpack-tailwind-starter` and `simple-tailwind-starter`.

## Table of Contents

- [Getting Started](#getting-started)
- [Current Mini Projects](#current-mini-projects)
- [Templates](#templates)
  - [Webpack-Tailwind-Starter](#webpack-tailwind-starter)
  - [Simple-Tailwind-Starter](#simple-tailwind-starter)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

Refer to the [Templates](#templates) section to start using a template.
To use the parent `node_modules` folder for your mini project, follow these steps:

1. Make sure there is no `node_modules` folder in your mini project's subfolder. If it exists, delete it.

2. Install the `cross-env` package in the parent `tailwind-mini-projects` folder, if not already installed:

```bash
cd ..  # Go to the parent folder (tailwind-mini-projects)
npm install --save-dev cross-env
```

3. Create a `.env` file in the root of your mini project.

4. Add the following line to the `.env` file:
```
NODE_PATH=./../node_modules
```

5. Update the `scripts` section in your mini project's `package.json` file:

```json
"scripts": {
  "dev": "cross-env NODE_PATH=./../node_modules webpack serve",
  "build": "cross-env NODE_PATH=./../node_modules webpack"
}
```

_NOTE: As the `node_modules` folder is located in the `tailwind-mini-projects` parent directory, all mini projects will have access to the parent modules._

## Current Mini Projects

| Name                | Date Started | Date Done  |
|---------------------|--------------|------------|
| Email Subscription  | 5 May 2023   | 5 May 2023 |
| Pricing Cards       | 6 May 2023   | 6 May 2023 |
| Modal Product       | 7 May 2023   | 8 May 2023 |

## Templates

### Webpack-Tailwind-Starter

This is a starter template that uses Webpack to bundle and build the project. It includes basic setup for Webpack, Tailwind CSS, and PostCSS.

To use this template for a new project, follow these steps:

1. Copy the `webpack-tailwind-starter` folder and rename it to your new project's name.

2. Change to the new project directory:

```bash
cd your-new-project
```

3. Install the dependencies:

```bash
npm install
```

4. Start the development server:

```bash
npm run dev
```

5. Build the project for production:

```bash
npm run build
```

### Simple-Tailwind-Starter

This is a simpler starter template that uses the Tailwind CLI to build the project. It's a more lightweight option if you don't need the complexity of Webpack.

To use this template for a new project, follow these steps:

1. Copy the `simple-tailwind-starter` folder and rename it to your new project's name.

2. Change to the new project directory:

```bash
cd your-new-project
```

3. Build the project:

```bash
npm run build
```

4. Start a local development server (e.g., using [live-server](https://www.npmjs.com/package/live-server)) and open the `index.html` file.

## Contributing

Feel free to contribute by submitting pull requests, opening issues, or suggesting new mini projects.

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
