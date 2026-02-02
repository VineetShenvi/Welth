<img width="1470" alt="Screenshot 2024-12-10 at 9 45 45 AM" src="https://github.com/user-attachments/assets/1bc50b85-b421-4122-8ba4-ae68b2b61432">

# Welth: AI Powered Finance Management

Welcome to Welth, an intelligent finance tracking application that helps users take control of their money through automated tracking, smart budgeting, and AI-driven insights. Welth combines modern financial tooling with AI to deliver clear monthly reports, proactive reminders, and effortless expense logging.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Future Aspects](#future-aspects)
- [Contributors](#contributors)
- [License](#license)

## Introduction

Welth is a full-stack finance management application designed to simplify personal expense tracking and budgeting. It allows users to log transactions, manage recurring expenses, set budgets, and receive automated insights about their spending habits.

Using scheduled background jobs and AI-powered analysis, Welth generates monthly financial reports, sends timely budget alerts via email, and even extracts transaction data from uploaded receipts — all with minimal manual effort from the user.

## Features

### 1. Secure Authentication & User Management

Welth uses Clerk for secure authentication, providing email/password and OAuth-based sign-in while handling sessions, user management, and authorization out of the box.

### 2. Transaction & Recurring Expense Tracking

Users can log one-time and recurring transactions, ensuring that fixed expenses like subscriptions, rent, or utilities are tracked automatically without repeated manual entry.

### 3. Budget Monitoring & Cross-Limit Reminders

Users can define a budget for their default account. When spending approaches or crosses predefined limits, Welth proactively sends email reminders to help users stay financially disciplined.

### 4. Automated Monthly Finance Reports

At the end of each month, Welth generates a detailed financial summary highlighting total spending, category-wise breakdowns, trends, and anomalies — delivered directly to the user’s inbox.

### 5. AI-Generated Financial Insights

Using Gemini, Welth analyzes monthly spending patterns and produces human-readable insights, suggestions, and observations to help users understand where their money is going and how they can improve.

### 6. AI Receipt Scanner

Users can upload images of receipts, and Gemini automatically extracts key details such as merchant name, amount, date, and category — converting physical receipts into structured digital transactions.

### 7. Interactive Financial Visualizations

Spending trends and category breakdowns are visualized using interactive charts built with Recharts, helping users quickly understand their financial data.

## Tech Stack

Welth is built using a modern, production-ready tech stack:

- Next.js: Full-stack React framework
- Clerk: Authentication, user management, and session handling
- Supabase PostgreSQL: Primary database
- Prisma: Type-safe ORM
- Inngest: Background jobs, cron tasks, and event-driven workflows
- Gemini AI: Receipt scanning and financial insight generation
- Arcjet: Security, rate limiting, and abuse protection
- Resend: Transactional and scheduled email delivery
- Recharts: Interactive financial visualizations

## Getting Started

To get started with Welth, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/VineetShenvi/Welth.git
   cd Welth
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Set up your environment variables.

    ```bash
    DATABASE_URL=
    DIRECT_URL=

    NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
    CLERK_SECRET_KEY=
    NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
    NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
    NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
    NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

    GEMINI_API_KEY=

    RESEND_API_KEY=

    ARCJET_KEY=
   ```

4. Run database migrations:

   ```bash
   npx prisma migrate dev
   ```

4. Run the application:

   ```bash
   npm run dev
   ```
   Visit `http://localhost:3000` in your browser.

## Usage

Explore Welth and take advantage of its powerful features:

- Sign up and securely authenticate using Clerk.
- Add and manage daily and recurring transactions.
- Define account budgets and receive email alerts when limits are crossed.
- Upload receipts and automatically extract expense data using AI.
- Receive detailed monthly financial reports via email.
- Visualize spending patterns and trends through interactive charts.
- Gain AI-generated insights to improve financial habits.

## Future Aspects

Stay tuned for exciting features in future releases:

- Exportable reports (PDF/CSV).
- Multi-currency support.
- Bank account integration

## Contributors

- [Vineet Shenvi](https://github.com/VineetShenvi)
## License

Welth is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code as per the terms of the license.
