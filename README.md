# 💰 FinTrack – AI Powered Financial Tracker

FinTrack is a modern full-stack financial management platform that helps users track expenses, manage multiple accounts, automate recurring transactions, and receive AI-powered financial insights.

Built with Next.js 15, MongoDB, Prisma, Clerk Authentication, Google Gemini AI, Inngest Workflows, ArcJet Security, and Resend Email Services.

---

## 🚀 Features

### 📊 Financial Management
- Multi-account support (Current & Savings)
- Real-time balance tracking
- Income & Expense management
- Transaction CRUD operations
- Bulk transaction deletion with balance synchronization

### 🤖 AI-Powered Features
- AI Receipt Scanner using Google Gemini 2.5 Flash
- Automatic extraction of:
  - Amount
  - Merchant
  - Date
  - Category
- Monthly AI-generated financial insights
- Personalized spending recommendations

### 🔄 Automation with Inngest
- Automated recurring transactions
- Monthly financial report generation
- Budget monitoring and alerts
- Retry handling and workflow orchestration

### 📈 Analytics & Reporting
- Spending analytics dashboard
- Category-wise expense breakdown
- Interactive charts and visualizations
- Monthly AI reports delivered via email

### 🔐 Enterprise-Grade Security
- Clerk Authentication
- Protected Routes
- ArcJet Shield Protection
- ArcJet Bot Detection
- Rate Limiting
- Atomic Database Transactions

### 📱 Modern UI
- Responsive design
- Mobile-first experience
- Built with Tailwind CSS and shadcn/ui
- Clean and intuitive dashboard

---

# 🏗️ System Architecture

## Frontend
- Next.js 15
- React 18
- Tailwind CSS
- shadcn/ui
- Recharts
- React Hook Form
- Zod

## Backend
- Next.js Server Actions
- Prisma ORM
- MongoDB

## External Services
- Clerk Authentication
- Google Gemini 2.5 Flash
- Inngest
- ArcJet
- Resend

---

# 🛠️ Tech Stack

| Category | Technology |
|-----------|------------|
| Framework | Next.js 15 |
| Frontend | React 18 |
| Styling | Tailwind CSS |
| UI Components | shadcn/ui |
| Authentication | Clerk |
| Database | MongoDB |
| ORM | Prisma |
| AI | Google Gemini 2.5 Flash |
| Background Jobs | Inngest |
| Security | ArcJet |
| Email Service | Resend |
| Validation | Zod |
| Forms | React Hook Form |
| Charts | Recharts |

---

# 🤖 AI Receipt Scanning Flow

1. User uploads receipt image
2. Image converted to Base64
3. Sent to Gemini 2.5 Flash
4. AI extracts:
   - Amount
   - Date
   - Merchant
   - Category
5. Transaction form auto-populated
6. User confirms and saves

---

# 🔄 Automated Workflows

## Trigger Recurring Transactions
Runs daily at midnight.

## Process Recurring Transactions
Automatically creates transactions and updates balances.

## Generate Monthly Reports
Creates AI-powered financial insights and emails users.

## Budget Alerts
Checks budget utilization every 6 hours and sends alerts when spending exceeds 80%.

---

# 🔐 Security Architecture

### Layer 1 – Edge Protection
- ArcJet Shield
- ArcJet Bot Detection
- Clerk Authentication Middleware

### Layer 2 – Application Security
- Session validation in every Server Action
- ArcJet Rate Limiting
- Prisma Atomic Transactions

---

# 📂 Project Structure

```bash
FinTrack/
│
├── app/
├── actions/
├── components/
├── lib/
├── prisma/
├── hooks/
├── emails/
├── public/
├── types/
├── utils/
└── inngest/
```

---

# ⚙️ Environment Variables

Create a `.env` file in the root directory:

```env
DATABASE_URL=

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up

NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/dashboard
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/dashboard

GEMINI_API_KEY=

RESEND_API_KEY=

ARCJET_KEY=

INNGEST_EVENT_KEY=
INNGEST_SIGNING_KEY=
```

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/fintrack.git
```

Navigate to project directory

```bash
cd fintrack
```

Install dependencies

```bash
npm install
```

Generate Prisma Client

```bash
npx prisma generate
```

Run database migrations

```bash
npx prisma db push
```

Start development server

```bash
npm run dev
```

---

# 📧 Monthly AI Reports

Each month FinTrack:

- Calculates income and expenses
- Analyzes spending behavior
- Generates financial recommendations using Gemini AI
- Sends reports directly to the user's email using Resend

---

# 🎯 Future Enhancements

- Multi-currency support
- Bank API integration
- React Native mobile app
- AI Financial Advisor Chatbot
- CSV/PDF Export
- Per-account budgets
- Push Notifications
- Automated bank transaction import

---

# 👨‍💻 Team

- Merugu Mourya Adithya
- V Sai Akshay
- I Mithun Reddy
- Maganti Anish Kumar
- Sandeep Surapaneni

### Supervisor
Mr. Ravi Babu Mashetti

Mahindra University (Mahindra École Centrale)

---

# 📜 License

This project was developed as a Final Year B.Tech Project for academic and learning purposes.

---

⭐ If you found this project useful, consider giving it a star.
