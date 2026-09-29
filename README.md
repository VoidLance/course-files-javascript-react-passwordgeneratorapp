# Password Generator

A small React and TypeScript password generator built with Vite and Tailwind
CSS. Choose a password length, optionally include numbers and special
characters, generate a password, and copy it to the clipboard.

## Why use it?

- Generate passwords between 6 and 20 characters.
- Include uppercase and lowercase letters by default.
- Toggle numbers and special characters.
- Ensure each enabled character category is represented in the generated
  password.
- Copy the result with one click.
- Run locally as a lightweight, client-side application with no backend or
  account required.

> **Security note:** Passwords are generated in the browser with
> `Math.random()`. This is suitable for demos and everyday convenience, but it
> is not a cryptographically secure password generator for high-risk
> credentials.

## Getting started

### Prerequisites

- Node.js 20.19+ or 22.12+
- npm

### Installation

Clone the repository, install its dependencies, and start the development
server:

```bash
git clone https://github.com/VoidLance/course-files-javascript-react-passwordgeneratorapp.git
cd course-files-javascript-react-passwordgeneratorapp
npm install
npm run dev
```

Open the local URL printed by Vite in your browser.

### Usage

1. Set the desired password length with the slider.
2. Choose whether to include numbers and special characters.
3. Select **Generate Password**.
4. Select **Copy** to copy the result to the clipboard.

The clipboard action may require a secure browser context when the app is
deployed outside of localhost.

## Available scripts

Run these commands from the project directory:

| Command | Description |
| --- | --- |
| `npm run dev` | Start the Vite development server with hot reload. |
| `npm run build` | Type-check and create a production build in `dist/`. |
| `npm run preview` | Preview the production build locally. |
| `npm run lint` | Check the project with ESLint. |

## Project structure

```text
src/
├── components/PasswordGenerator.tsx  # Password generator interface
├── utils/hooks.tsx                    # Password generation state and logic
├── App.tsx                            # Application entry component
└── main.tsx                           # React bootstrap
```

## Support

For questions or bugs, search existing issues in the repository first. If your
problem is not already reported, open a new issue with:

- A clear description of the problem or requested improvement
- Steps to reproduce the issue
- Your browser and Node.js versions
- Relevant console output or screenshots

## Contributing

Contributions are welcome. To propose a change:

1. Fork the repository and create a focused feature or fix branch.
2. Install dependencies with `npm install`.
3. Make the change and update documentation when behavior changes.
4. Run `npm run lint` and `npm run build`.
5. Open a pull request describing the change and validation performed.

Please keep pull requests small, accessible, and consistent with the existing
React, TypeScript, and Tailwind CSS patterns.

## Maintainer

This project is maintained by [VoidLance](https://github.com/VoidLance).
Contributions and constructive feedback from the community are appreciated.
