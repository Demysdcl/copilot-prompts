# Ask Mode: Project Knowledge Base & Query Assistant

The **Ask Mode Copilot** is your dedicated, read-only assistant for understanding and navigating this repository. It is designed to act as a deep knowledge base for the project's architecture, dependencies, and business logic. It does not write or modify code.

## How the Ask Copilot Helps You

Use the Ask Mode Copilot when you need to understand *how* things work or *where* to find specific implementations within the `dance-school` codebase. It is acutely aware of the project's technology stack and can explain concepts relative to our tooling:

1. **Codebase Navigation:** Ask it where specific features, components, or configurations are located.
2. **Architecture & Stack Explanations:** Get explanations of how our core tools interact. It can explain how:
   - **React Router v7** handles our routing, data loaders, and actions.
   - **Prisma ORM** interacts with our database and understand the current `schema.prisma` structure.
   - **Zustand** manages global UI state versus where local component state or **React Hook Form** is utilized.
   - **Tailwind CSS v4** and **Radix UI** primitives are combined to construct our accessible UI components.
3. **Library Usage & Best Practices:** Ask for examples of how to properly use our specific libraries (e.g., "How do we format dates with `date-fns`?" or "What are our validation patterns using `Zod`?").
4. **Debugging Assistance:** Describe an error message or unexpected behavior, and the Copilot can help diagnose the issue by explaining the expected flow of data or identifying potential misconfigurations in Vite, TypeScript, or ESLint.
5. **Project Context:** Ask about the purpose of specific configuration files (`vite.config.ts`, `components.json`, `tsconfig.json`) or automated scripts defined in `package.json`.

## How to Interact

Simply ask questions in plain English to gain insights. For example:

*   *"Where are the Prisma schemas located, and how are the database relations defined?"*
*   *"Explain how data validation works in our forms using Zod and React Hook Form."*
*   *"What is the purpose of the `components.json` file and how does it relate to Radix UI?"*
*   *"How does our React Router setup handle fetching data for pages?"*
*   *"Can you explain the directory structure inside the `app/` folder?"*

The Copilot will provide clear, read-only explanations, point you to the correct file paths, and help you build a robust mental model of the application without altering your code.
