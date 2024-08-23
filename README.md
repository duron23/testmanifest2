# Chrome Extension Template

This repository serves as a powerful and flexible template for building Chrome Extensions. It integrates modern web technologies to streamline development, ensuring your extension is robust, scalable, and maintainable.

## 🛠 Tech Stack

- **Webpack**: Efficiently bundles and transpiles your code, ensuring optimal performance and compatibility.
- **React**: Utilized for building the Popup, Options, and SidePanel interfaces, allowing for a dynamic and responsive user experience.
- **TypeScript**: Provides type safety and enhanced development features for a more reliable codebase.
- **Tailwind CSS**: A utility-first CSS framework for rapidly building custom user interfaces.
- **ViTest**: A fast and lightweight testing framework for unit tests.
- **Puppeteer**: Enables headless browser testing, ensuring your extension functions as expected across different scenarios.
- **Chrome Types**: Provides built-in for typescript support.

## 🚀 Getting Started

### 1. Setup

To get started, clone the repository and install the necessary dependencies:

\`\`\`bash
git clone https://github.com/your-repo/chrome-extension-template.git
cd chrome-extension-template
npm install
\`\`\`

### 2. Configure

Before building and running the extension, customize it by editing the \`.env\` file. Changes in the \`.env\` file automatically reflect in the extension's manifest, making it easy to update key details like:

- **Extension Name**: \`EXTENSION_NAME=YourExtensionName\`
- **Extension Description**: \`EXTENSION_DESCRIPTION=A brief description of your extension.\`
- **Manifest Version**: \`MANIFEST_VERSION=1.0.0\`

### 3. Development

Use the following scripts to manage different environments and development processes:

- **Generate Manifest**: Customize the manifest based on the environment.

  - Development: \`npm run prebuild:dev\`
  - UAT: \`npm run prebuild:uat\`
  - Production: \`npm run prebuild:prod\`

- **Build**: Compile and optimize the extension for different environments.

  - Development: \`npm run build:dev\`
  - UAT: \`npm run build:uat\`
  - Production: \`npm run build:prod\`

- **Watch**: Start a watch mode to rebuild the extension automatically on code changes.

  \`\`\`bash
  npm run watch
  \`\`\`

- **Lint**: Automatically fix code style issues with ESLint.

  \`\`\`bash
  npm run lint
  \`\`\`

### 4. Testing

Run tests using ViTest and Puppeteer with the following scripts:

- **Test Watch**: Continuously run unit tests during development.

  \`\`\`bash
  npm run test:watch
  \`\`\`

- **Test UI**: Run tests with a user interface.

  \`\`\`bash
  npm run test:ui
  \`\`\`

- **Unit Tests**: Run all unit tests.

  \`\`\`bash
  npm run test:unit
  \`\`\`

- **End-to-End Tests**: Run end-to-end tests.

  \`\`\`bash
  npm run test:e2e
  \`\`\`

- **Test Coverage**: Generate a test coverage report.

  \`\`\`bash
  npm run coverage
  \`\`\`

### 5. Load the Extension

To load the extension into Chrome for testing:

1. Open Chrome and navigate to \`chrome://extensions/\`.
2. Enable "Developer mode" at the top-right corner.
3. Click "Load unpacked" and select the \`dist/\` directory generated by the build process.
