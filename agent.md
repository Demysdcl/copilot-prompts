# Agent Mode: Autonomous Implementation & Execution

The **Agent Mode Copilot** is your hands-on coding assistant and executor. Unlike Ask or Plan modes, the Agent is designed to actively write code, modify files, run terminal commands, and implement features directly within your workspace. It leverages the established project stack to build features from start to finish.

## What the Implementation Agent Does

When you provide an actionable task or an implementation plan, the Agent Mode Copilot takes autonomous steps to execute it according to the project's standards:

1. **Code Generation & Modification:** It writes and refactors code across the entire stack:
   - Creating new **React Router v7** route modules, along with their `loader` and `action` functions.
   - Building accessible UI components using **React 18** and **Radix UI**, styling them fluidly with **Tailwind CSS v4**, `clsx`, and `tailwind-merge`.
   - Modifying the **Prisma** schema (`schema.prisma`) to add or alter database models.
   - Implementing robust forms and validation schemas using **React Hook Form** and **Zod**.
   - Setting up or updating state management stores securely with **Zustand**.
2. **Terminal Execution:** It can execute project scripts and terminal commands to maintain workflow momentum:
   - Running development servers (`npm run dev`) or building the project.
   - Executing `npx prisma db push` or `npx prisma generate` when the database schema changes.
   - Running linters (`npm run lint`), TypeScript checks (`npm run typecheck`), or unit tests via **Vitest**.
3. **File & System Management:** It seamlessly creates, moves, or deletes files and directories to keep the `app/` structure organized and aligned with conventions.
4. **End-to-End Implementation:** You can hand off a fully defined feature (e.g., an output from Plan Mode), and the Agent will orchestrate and build the UI, server-side actions, database connections, and tests required to complete it.

## How to Interact

Give the Agent Mode definitive, actionable task descriptions. It operates best when provided with clear requirements or a structured plan. For example:

*   *"Implement the class booking form we planned earlier. Create the UI using our Radix Select components, apply Tailwind styling, and connect it to a new React Router action for submission."*
*   *"Add a new `Instructor` model to the Prisma schema, push the db changes, and create a basic list view route under `/instructors`."*
*   *"Write Vitest tests for the date formatting utility we created using `date-fns`."*
*   *"Refactor the global user state to use Zustand instead of the current Context implementation."*
*   *"Here is our implementation plan for the new dashboard header. Please execute step 1."*

**Note:** The Agent is a powerful tool surface that executes code directly in your repository. It handles code authoring automatically, allowing you to review changes in your editor as it works.