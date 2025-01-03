# Getting started with moon

## Getting Started with @moonup/create

Welcome to the @moonup/create package documentation! This powerful tool allows you to quickly set up a new Next.js project with various configurable options, tailored for blockchain and DeFi development.

### Introduction

@moonup/create is a CLI tool that helps you bootstrap a new Next.js project with additional features specifically designed for blockchain and DeFi applications. It provides a seamless way to create a new project with options for TypeScript, ESLint, PWA support, Moon Wallet integration, and more.

### Prerequisites

Before you begin, make sure you have Node.js installed on your system. We recommend using the latest LTS version.

### Creating a New Project

To create a new project using @moonup/create, run the following command in your terminal:

```bash
npx @moonup/create@latest
```

This command will start an interactive process where you'll be prompted to make choices about your project setup.

### Configuration Options

During the project creation process, you'll be asked a series of questions to customize your setup:

1. **Project Name**: Choose a name for your project. This will be used as the directory name and in your package.json.
2. **TypeScript**: Decide whether to use TypeScript in your project.
3. **ESLint**: Choose if you want to include ESLint for code linting.
4. **PWA (Progressive Web App)**: Opt to include PWA support for your application.
5. **Moon Wallet**: Decide if you want to integrate Moon Wallet into your project.
6. **Tailwind CSS**: Choose whether to include Tailwind CSS for styling.
7. **src/ Directory**: Decide if you want to use a `src/` directory for your source files.
8. **Custom Import Alias**: Choose if you want to customize the default import alias (@/\*).
9. **Rainbowkit Connect**: Decide if you want to integrate Rainbowkit for wallet connections.
10. **Wallet Connect**: Choose whether to include Wallet Connect integration.

### Project Structure

After the creation process, your project will have a structure similar to a standard Next.js project, with additional files and configurations based on your choices. Here's a basic overview:

```
my-app/
├── pages/
│   ├── _app.js
│   └── index.js
├── public/
├── styles/
├── package.json
├── next.config.js
└── README.md
```

Additional files and directories will be present based on your configuration choices.

### Next Steps

1.  Navigate to your project directory:

    ```bash
    cd my-app
    ```
2.  Install dependencies:

    ```bash
    npm install
    ```

    or

    ```bash
    yarn
    ```
3.  Start the development server:

    ```bash
    npm run dev
    ```

    or

    ```bash
    yarn dev
    ```
4. Open http://localhost:3000 in your browser to see your application.

### Additional Features

#### Moon Wallet Integration

If you chose to include Moon Wallet, you'll find additional components and hooks in your project for easy blockchain interactions. Refer to the Moon Wallet documentation for more details on usage.

#### Tailwind CSS

If you opted for Tailwind CSS, your project will be set up with the necessary configurations. You can start using Tailwind classes in your components right away.

#### TypeScript

For TypeScript projects, you'll find .ts and .tsx files instead of .js and .jsx. TypeScript configurations will be automatically set up for you.

#### PWA Support

If you chose PWA support, your project will include the necessary service worker and manifest files. Make sure to customize these for your specific application needs.

### Customization

Feel free to modify any of the generated files to suit your project needs. The next.config.js file is a great place to start for Next.js-specific configurations.

### Conclusion

@moonup/create provides a solid foundation for building blockchain and DeFi applications with Next.js. It combines the power of Next.js with additional tools and integrations commonly used in blockchain development.

For more information on Next.js features and API, check out the Next.js documentation.

Happy coding with @moonup/create and Next.js!
