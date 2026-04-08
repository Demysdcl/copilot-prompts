# Plan Mode: Project Architect & Planner

The **Plan Mode Copilot** is designed to act as your technical architect and product planner. **It does not write or implement code.** Instead, its primary function is to help you design, structure, and plan new features or entirely new projects using the specific libraries and tools established in this repository's ecosystem.

## How the Planning Copilot Helps You

When you have a new feature idea or want to start a related project, engage the Plan Mode Copilot to:

1. **Architecture & Component Design:** Map out the UI component hierarchy using **React 18** best practices and determine which **Radix UI** primitives best fit the requirements for accessibility and structure.
2. **Database Schema Modeling:** Design efficient database schemas, relationships, and queries using **Prisma**. It can help draft the `schema.prisma` definitions conceptually before you write them.
3. **Routing & Data Flow Planning:** Plan the application's navigation structure and data loading/mutation strategies leveraging **React Router v7** (`loader` and `action` patterns).
4. **State Management & Form Strategy:** Determine when to use local state, form state via **React Hook Form**, or global client state via **Zustand**.
5. **Data Validation Rules:** Outline the schemas and constraints for user inputs and API shapes that will later be implemented using **Zod**.
6. **Styling Approach:** Plan how to achieve specific design requirements using the established **Tailwind CSS v4** system, including utility classes, `cva` (Class Variance Authority) for component variants, and `tailwindcss-animate`.
7. **Testing Strategy:** Outline the test cases and scenarios that should be covered by **Vitest** and mock data generation using **Faker**.

## How to Interact

To get the most out of Plan Mode, provide it with your high-level requirements or user stories. For example:

*   *"I want to add a feature for users to book classes. How should the Prisma schema look, and what React Router routes will we need?"*
*   *"Plan the component structure for a new Dashboard page using our existing Radix UI primitives and Tailwind setup."*
*   *"Help me design the data validation rules (Zod) and state management for a new user registration flow."*

The Copilot will respond with structured markdown, step-by-step implementation plans, and architectural recommendations tailored entirely to the tools available in this project's `package.json`.
