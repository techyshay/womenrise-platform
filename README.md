# WomenRise Platform

A comprehensive community platform designed to empower underrepresented women through resources, mentorship, and networking opportunities.

## 🌟 Features

- **Resource Library**: Curated resources for career development, financial literacy, entrepreneurship, health & wellness, education, and leadership
- **Community Discussions**: Interactive forums for sharing experiences and supporting each other
- **Mentorship Program**: Connect with experienced professionals for guidance and career growth
- **Opportunities Hub**: Discover events, job openings, programs, and workshops
- **Success Stories**: Share and celebrate achievements within the community
- **User Authentication**: Secure login system with Replit Auth integration

## 🚀 Tech Stack

### Frontend
- **React** with TypeScript
- **Vite** for fast development and building
- **Tailwind CSS** for styling
- **Radix UI** components with shadcn/ui
- **TanStack React Query** for server state management
- **Wouter** for lightweight routing
- **React Hook Form** with Zod validation

### Backend
- **Node.js** with Express.js
- **TypeScript** with ES modules
- **PostgreSQL** with Neon Database
- **Drizzle ORM** for type-safe database operations
- **OpenID Connect** authentication with Replit

## 🛠️ Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd womenrise-platform
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
Create a `.env` file with the following variables:
```bash
DATABASE_URL=your_postgresql_connection_string
SESSION_SECRET=your_session_secret
REPLIT_DOMAINS=your_allowed_domains
ISSUER_URL=https://replit.com/oidc
REPL_ID=your_repl_id
```

4. Set up the database:
```bash
npm run db:push
```

5. Start the development server:
```bash
npm run dev
```

## 📁 Project Structure

```
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── hooks/          # Custom React hooks
│   │   ├── lib/            # Utility functions
│   │   ├── pages/          # Page components
│   │   └── App.tsx         # Main application component
├── server/                 # Express backend
│   ├── db.ts              # Database configuration
│   ├── routes.ts          # API routes
│   ├── storage.ts         # Database operations
│   ├── replitAuth.ts      # Authentication setup
│   └── index.ts           # Server entry point
├── shared/                # Shared types and schemas
│   └── schema.ts          # Database schema and types
└── package.json           # Dependencies and scripts
```

## 🗄️ Database Schema

The platform uses a comprehensive PostgreSQL schema with the following main entities:

- **Users**: Profile management with interests, goals, and role-based permissions
- **Resources**: Categorized learning materials and career development content
- **Discussions**: Community forum functionality with replies and engagement tracking
- **Mentorship**: Mentor matching and relationship management
- **Opportunities**: Events, jobs, programs, and workshops
- **Success Stories**: Community achievements and testimonials

## 🔧 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run db:push` - Push database schema changes
- `npm run db:studio` - Open database studio

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🎯 Mission

WomenRise is committed to creating an inclusive platform that addresses the unique challenges faced by underrepresented women in their professional and personal growth journeys. Our goal is to provide accessible resources, meaningful connections, and opportunities that empower women to achieve their full potential.

## 🌐 Deployment

The application is designed to run seamlessly in various environments:

- **Development**: Vite dev server with hot module replacement
- **Production**: Optimized builds with static file serving
- **Database**: PostgreSQL with connection pooling
- **Authentication**: Secure session management with PostgreSQL storage

## 📞 Support

For questions, suggestions, or support, please:
- Open an issue in this repository
- Contact the development team
- Join our community discussions

---

Built with 💜 for empowering women everywhere.
