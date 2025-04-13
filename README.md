# Shopify Theme Project

This repository contains a Shopify theme project with custom sections and templates.

## Getting Started with Shopify CLI

Shopify CLI is a tool that helps you build Shopify themes and integrate with the Shopify platform. Here's how to set it up and use it with this project.

### Prerequisites

- [Node.js](https://nodejs.org/) (v14 or later)
- [npm](https://www.npmjs.com/) (usually comes with Node.js)
- A Shopify Partner account
- A Shopify development store or existing store

### Installing Shopify CLI

#### Method 1: Using npm (Recommended)

```bash
npm install -g @shopify/cli @shopify/theme
```

#### Method 2: Using Homebrew (macOS)

```bash
brew tap shopify/shopify
brew install shopify-cli
```

#### Method 3: Using Ruby Gem

```bash
gem install shopify-cli
```

### Verifying Installation

To verify that Shopify CLI is installed correctly:

```bash
shopify version
```

## Working with This Theme Project

### Cloning the Repository

```bash
git clone https://github.com/Base0005/ShopifyFinalProject.git
cd ShopifyFinalProject
```

### Authenticating with Shopify

Before you can work with themes, you need to authenticate with Shopify:

```bash
shopify login
```

### Development Workflow

#### 1. Preview the Theme Locally

To start a local development server:

```bash
shopify theme dev
```

This will:
- Start a local server
- Open your browser with a preview of your theme
- Watch for changes and automatically reload the browser

#### 2. Push Theme to Shopify Store

To push your theme to your Shopify store:

```bash
shopify theme push
```

#### 3. Pull Theme from Shopify Store

To pull the latest version of your theme from Shopify:

```bash
shopify theme pull
```

### Working with Theme Files

The project structure follows Shopify's standard theme architecture:

- `assets/`: Contains CSS, JavaScript, and other static files
- `config/`: Contains theme settings
- `layout/`: Contains theme layout templates
- `locales/`: Contains translation files
- `sections/`: Contains modular, reusable content blocks
- `snippets/`: Contains reusable code snippets
- `templates/`: Contains templates for different page types

## Theme Features

This theme includes:
- Custom banner section (referenced in `templates/index.liquid`)
- Product display on the homepage showing the "Our Favourites" collection
- Responsive design elements

## Troubleshooting

### Common Issues

1. **Authentication Problems**
   ```bash
   shopify logout
   shopify login
   ```

2. **Theme Not Updating**
   - Make sure you're in the correct directory
   - Try restarting the development server

3. **Missing Dependencies**
   ```bash
   npm install
   ```

### Getting Help

- [Shopify CLI Documentation](https://shopify.dev/themes/tools/cli)
- [Shopify Theme Development](https://shopify.dev/themes)
- [Shopify Community Forums](https://community.shopify.com/)

## License

This project is licensed under the MIT License - see the LICENSE file for details.
