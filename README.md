# Modern Next.js Template

A modern, full-stack Next.js template with Prisma, Supabase, React Query, and more. Built with TypeScript and featuring a complete development setup.

## 🚀 Features

- ⚡️ Next.js 15 with App Router
- 🔋 Prisma ORM with PostgreSQL
- 🔑 Authentication with NextAuth.js
- 🎨 Tailwind CSS for styling
- 📊 React Query for data fetching
- 🏢 Type-safe database queries
- 🔄 React Hook Form with Zod validation
- 📅 Date handling with date-fns
- 🎭 Dark mode support with next-themes
- 📊 Recharts for data visualization
- 🛠 Complete TypeScript support

## 📦 Prerequisites

- Node.js 18+ 
- PostgreSQL database (local or Supabase)
- pnpm (recommended) or npm

## 🛠 Setup

1. Clone the repository:
```bash
git clone [your-repo-url]
cd [your-project-name]
```

2. Install dependencies:
```bash
pnpm install
```

3. Set up your environment variables:
```bash
cp .env.example .env
```

4. Configure your `.env` file:
```env
# Database
DATABASE_URL="postgresql://user:password@localhost:5432/dbname?schema=public"

# Supabase
NEXT_PUBLIC_SUPABASE_URL=your-project-url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-anon-key

# NextAuth.js
NEXTAUTH_SECRET=your-secret-key
NEXTAUTH_URL=http://localhost:3000

# Optional: OAuth Providers
GOOGLE_CLIENT_ID=your-google-client-id
GOOGLE_CLIENT_SECRET=your-google-client-secret
```

5. Initialize Prisma:
```bash
pnpm prisma generate
pnpm prisma db push
```

## 🚀 Development

Start the development server:
```bash
pnpm dev
```

Your app will be available at `http://localhost:3000`

## 📝 Database Management

### Initialize Prisma
```bash
pnpm prisma init
```

### Create a migration
```bash
pnpm prisma migrate dev --name init
```

### Reset database
```bash
pnpm prisma migrate reset
```

### Open Prisma Studio
```bash
pnpm prisma studio
```

## 🏗 Project Structure

```
├── app/                   # Next.js App Router
│   ├── api/              # API routes
│   ├── (auth)/          # Authentication routes
│   └── (dashboard)/     # Protected dashboard routes
├── components/           # React components
├── lib/                  # Utility functions
├── prisma/              # Prisma schema and migrations
└── public/              # Static assets
```

## 🧪 Testing

```bash
pnpm test        # Run tests
pnpm test:watch  # Run tests in watch mode
```

## 🚀 Deployment

1. Build the application:
```bash
pnpm build
```

2. Start the production server:
```bash
pnpm start
```

## 📚 Key Dependencies

- Next.js 15.1.7
- React 19.0.0
- Prisma 6.4.0
- TanStack Query 5.66.7
- NextAuth.js 4.24.11
- React Hook Form 7.54.2
- Zod 3.24.2
- Tailwind CSS 3.4.17

## 🔧 Common Issues & Solutions

### Prisma Client Issues
If you encounter Prisma Client issues, try:
```bash
pnpm prisma generate
```

### Database Connection Issues
- Verify your DATABASE_URL in .env
- Ensure PostgreSQL is running
- Check network access and firewall settings

## 📄 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 🙏 Acknowledgments

- [Next.js](https://nextjs.org/)
- [Prisma](https://www.prisma.io/)
- [Supabase](https://supabase.com/)
- [TanStack Query](https://tanstack.com/query)

