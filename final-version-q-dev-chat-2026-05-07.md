my manager told you are not able to explain the project , how frontend to backend working flow like how login, create study, site , examiner and audit and other flow. act as senior developer and teach me from scratch, suppose if i want to build this project then how it do it and from where i should i start , i want you consider me as begginner and teach me fron zero to hero to help me to know how i should build. i do not want to change any code just teach me if i am developer and i do not have any ai support then how would i built this project from scratch. and my manager also told that we have existing projects some are built from months and some from years , if you guys do not understand this simple sna website then how will you work in existing codebase.


i need you help and teach me quickly everything means everything about this project. first create a plan how will you teach me and then we will proceed.

---

I hear you — let me break this down properly. Your manager is right: if you can understand how this project is wired end-to-end, you'll be able to jump into any existing codebase with confidence. Let me teach you this like a senior dev would mentor a junior.

---

## Teaching Plan — SNA Project (Zero to Hero)

Here's how I'll walk you through this. We'll go module by module, layer by layer:

**Phase 1: Foundation (What is this project?)**
1. The big picture — what problem does it solve, what tech is used, how do the pieces connect
2. Project folder structure — where does what live and why

**Phase 2: Backend (The Engine)**
3. How the server starts — entry point, Express setup, middleware
4. Database layer — SQLite, schema, migrations, how data is stored
5. Repository layer — raw SQL queries, typed helpers
6. Service layer — business logic, domain rules
7. GraphQL layer — schema definitions, resolvers, how a request flows
8. Authentication — JWT, cookies, login/logout/refresh flow
9. Authorization — role guards (requireAuth, requireAdmin)
10. Validation — Zod schemas, error handling
11. Audit logging — how every action is tracked

**Phase 3: Frontend (The Face)**
12. React app setup — Vite, routing, theme
13. Apollo Client — how frontend talks to backend (GraphQL)
14. Auth context — how the app knows who's logged in
15. Pages & components — admin vs viewer, layouts, shared components
16. Forms & CRUD — react-hook-form, Zod, 2-step dialogs
17. Error handling — how errors flow from backend to user's screen

**Phase 4: Full Flows (Connecting the Dots)**
18. Login flow — end to end
19. Create Study flow — end to end
20. Assignment flow — end to end
21. Audit log flow — end to end
22. Search flow — end to end

**Phase 5: Testing & Deployment**
23. How tests are structured — unit, integration, E2E
24. How you'd build this from scratch — the order of steps

---

Tell me — should I start from Phase 1 and go through everything sequentially? Or do you want me to jump to a specific phase first?

I'd recommend starting from Phase 1 because understanding the big picture first makes everything else click. Once you see how a request travels from the user's click → React → Apollo → Express → SQLite → back, the whole project becomes obvious.

Say "go" and I'll start teaching Phase 1, or tell me which phase you want first.

---

before proceeding will you tell everthing from scratch that if i would built this project how would i built this from scratch without any help of ai , where to start and which file to create first and what to write and how to connect files and it should be design and all overall thinking. 


so will you teach me all this in above phases?

---

Yes — absolutely. That's exactly what the phases will cover. Let me be crystal clear about what you'll learn:

---

## What I'll Teach You (The Developer's Thinking Process)

**Not just "what the code does" — but HOW you'd think, decide, and build it step by step if you were sitting alone with an empty folder.**

Here's what each phase will answer:

**Phase 1** — "I have a requirement to build a clinical study management app. Where do I even start? What tech do I pick and why? How do I structure my folders?"

**Phase 2** — "Okay I picked Express + GraphQL + SQLite. Which file do I create first? How do I wire them together? How do I design my database tables? How do I make sure my business rules are enforced?"

**Phase 3** — "Backend is done. Now I need a UI. How do I set up React? How does React talk to my GraphQL backend? How do I handle login state? How do I build forms that show errors from the server?"

**Phase 4** — "I have both pieces. Let me trace a full user action — from button click to database write and back. How do all the files connect?"

**Phase 5** — "How do I make sure nothing breaks? How do I test this? If I were building from day 1, what's the exact order?"

---

## The Key Thing Your Manager Wants You to Understand:

> Every file exists for a reason. Every import connects two layers. If you understand **why** each layer exists and **how data flows between them**, you can read ANY codebase — whether it's 1 month old or 5 years old.

---

## How I'll Teach:

1. **The thinking** — why this decision was made
2. **The file** — which file to create, what to write first
3. **The connection** — how this file talks to other files
4. **The order** — what you'd build first, second, third
5. **Real code from this project** — I'll show you the actual files so you see it's not theory

---

Ready? Say "start" and I'll begin with Phase 1 — the big picture, the thinking process, and the very first decisions you'd make on Day 1 with an empty folder.

---

i want you show me your teaching plan one again then you start teaching me

---

## Teaching Plan — Building SNA From Scratch (Zero to Hero)

---

### Phase 1: Foundation (Day 1 Thinking)
1. **What is this app?** — The requirement, the domain (studies, sites, examiners)
2. **Tech decisions** — Why React? Why GraphQL? Why SQLite? Why not REST?
3. **Project structure** — Monorepo setup, folder design philosophy, how to organize code so it scales

---

### Phase 2: Backend (Building the Engine)
4. **Entry point** — Creating `server.ts`, starting Express, environment variables
5. **Middleware** — Security (helmet, CORS, rate limiting), request ID, logging
6. **Database setup** — SQLite connection, schema design, migrations, seed data
7. **Repository layer** — Raw SQL queries, typed helpers, why separate from business logic
8. **Service layer** — Business rules, domain logic, validation enforcement
9. **GraphQL schema** — Type definitions, queries, mutations — designing your API contract
10. **GraphQL resolvers** — How incoming requests get processed, calling services
11. **Authentication** — JWT strategy, HttpOnly cookies, login/logout/refresh token rotation
12. **Authorization** — Role guards (requireAuth, requireAdmin), protecting resolvers
13. **Validation** — Zod schemas, parseOrThrow pattern, error formatting
14. **Audit logging** — Tracking every action with before/after snapshots
15. **DataLoaders** — Preventing N+1 queries, per-request batching

---

### Phase 3: Frontend (Building the Face)
16. **Vite + React setup** — Project init, folder structure, theme configuration
17. **Apollo Client** — Connecting to GraphQL, error link, cookie credentials
18. **Routing** — React Router, protected routes, admin vs viewer separation
19. **Auth context** — How the app knows who's logged in, role-based rendering
20. **Layouts & navigation** — Sidebar, header, admin layout vs viewer layout
21. **List pages** — DataGrid, server-side pagination, useUrlPagination hook
22. **Detail pages** — Single entity view, related data, skeletons
23. **CRUD dialogs** — react-hook-form + Zod, 2-step stepper pattern
24. **Assignment UI** — Autocomplete pickers, checkbox panels, certificate picker
25. **Error handling** — parseGqlError, field-level errors, toast notifications
26. **Search** — Debounced input, lazy queries, filter-only search
27. **Audit UI** — Global audit page, per-entity history, expandable diff rows

---

### Phase 4: Full Flows (End-to-End Tracing)
28. **Login flow** — Click → mutation → cookie → context → redirect
29. **Create Study flow** — Form → validation → mutation → resolver → service → DB → audit → refetch → UI update
30. **Assign Site to Study flow** — Autocomplete → mutation → domain rules → junction table → audit
31. **SSE Assignment flow** — Checkbox → certificate picker → mutation → 3-way junction → audit
32. **Token refresh flow** — Token expires → errorLink intercepts → refreshSession → retry original request
33. **Search flow** — Typing → debounce → lazy query → backend LIKE queries → grouped results

---

### Phase 5: Building Order & Testing
34. **If I start from scratch — exact order** — What to build on Day 1, Day 2, Day 3... Day N
35. **Testing strategy** — Unit → Integration → E2E, what to test and why
36. **How to read any existing codebase** — The mental model your manager wants you to have

---

## Total: 36 lessons, covering every single file, every decision, every connection.

---

Say **"start"** and I begin Phase 1, Lesson 1. I'll go one lesson at a time, and you can ask questions anytime before we move to the next.

---

start

---

## Phase 1, Lesson 1: What Is This App?

---

### The Requirement (Imagine your manager gives you this)

> "Build a web app where our team can manage clinical studies. We have studies, each study runs at multiple sites (hospitals/clinics), and examiners (doctors) work at those sites. Admin users can create/edit everything. Viewer users can only look. Track every change anyone makes."

---

### Breaking Down the Domain

Think of it like a real-world clinical trial:

```
STUDY (e.g., "COVID Vaccine Trial Phase 3")
  └── runs at multiple SITES (e.g., "Apollo Hospital Mumbai", "AIIMS Delhi")
       └── each site has EXAMINERS (doctors) doing the work
            └── each examiner needs a valid CERTIFICATE (GCP certification) to participate
```

So you have **3 main entities**:
- **Study** — has a protocol ID, title, sponsor, phase, dates, status (Planned → Active → Completed)
- **Site** — has a site code, name, city, country, status (Planned → Active → Closed)
- **Examiner** — has a code, name, specialty, role (Principal Investigator / Sub-Investigator), certificates

And **relationships between them**:
- A study can have many sites (many-to-many → `study_sites` junction table)
- A site can have many examiners (many-to-many → `site_examiners` junction table)
- An examiner can work on a specific study at a specific site (3-way → `study_site_examiners` junction table)

---

### The Users

Two roles:
- **ADMIN** — can create, edit, assign, unassign everything. Sees audit logs.
- **VIEWER** — can only read. No create/edit buttons. No audit logs.

---

### The Key Business Rules (Why This Isn't Just a Simple CRUD App)

This is what makes it interesting — the app enforces real-world rules:

1. A new study always starts as "Planned" — you can't create it as "Active"
2. To activate a study, it must have at least 1 site and 1 examiner assigned
3. Status only moves forward: Planned → Active → Completed (never backward)
4. An examiner can't be assigned to a site unless they have a valid (non-expired) certificate
5. If you remove the last examiner from an Active site, the site auto-downgrades to Planned
6. Nothing is ever deleted — only status changes and unassignments

---

### What You're Building (The Two Pieces)

```
┌─────────────────┐         HTTP (GraphQL)         ┌─────────────────┐
│                 │  ──────────────────────────────▶│                 │
│   FRONTEND      │                                 │   BACKEND       │
│   (React app)   │◀──────────────────────────────  │   (Express API) │
│   Port 5173     │         JSON responses          │   Port 4040     │
│                 │                                 │                 │
└─────────────────┘                                 └────────┬────────┘
                                                             │
                                                             ▼
                                                    ┌─────────────────┐
                                                    │   SQLite DB     │
                                                    │   (app.db file) │
                                                    └─────────────────┘
```

The user opens the browser → React app loads → user clicks something → React sends a GraphQL request to Express → Express checks auth, validates input, runs business logic, talks to SQLite → sends response back → React updates the screen.

---

### Why This Matters for Existing Codebases

Every web app you'll ever work on follows this same pattern:
- **Frontend** (UI) → talks to → **Backend** (API) → talks to → **Database**
- The tech changes (React/Angular/Vue, REST/GraphQL, Postgres/MongoDB) but the FLOW is always the same

Once you understand this flow in SNA, you understand it everywhere.

---

**Lesson 1 done.** Next is **Lesson 2: Tech Decisions** — why React, why GraphQL instead of REST, why SQLite, and how you'd make these choices yourself.

Say **"next"** to continue, or ask questions about anything above.

---

next

---

## Phase 1, Lesson 2: Tech Decisions

---

### The Thinking Process (How a Developer Chooses Tech)

When you start a project, you ask yourself these questions:

1. **What kind of app is it?** — Web app with complex UI → need a frontend framework
2. **How complex is the data?** — Multiple related entities, nested queries → need a smart API layer
3. **How many users?** — Small team/demo → lightweight database is fine
4. **What's the team familiar with?** — TypeScript everywhere → fewer context switches

---

### Decision 1: Why TypeScript (not plain JavaScript)?

```
Plain JS:  function getUser(id) { ... }  // What does id look like? What does it return? No idea.
TypeScript: function getUser(id: string): UserRow { ... }  // Crystal clear.
```

- Catches bugs BEFORE you run the code (compile time)
- Your IDE gives you autocomplete, shows you what fields exist
- When you're reading someone else's code (existing codebase), types tell you exactly what's happening
- Same language on frontend AND backend — one mental model

**Decision: TypeScript for both frontend and backend.**

---

### Decision 2: Why React (not Angular, Vue, or plain HTML)?

| Option | Pros | Cons |
|--------|------|------|
| Plain HTML/JS | Simple | Painful for complex UIs, no component reuse |
| Angular | Full framework, batteries included | Heavy, steep learning curve, opinionated |
| Vue | Easy to learn, flexible | Smaller ecosystem than React |
| **React** | Huge ecosystem, component-based, flexible | Need to pick your own libraries |

For this project:
- Complex UI (tables, forms, dialogs, charts, role-based views) → need components
- MUI (Material UI) gives you pre-built professional components
- React has the largest ecosystem — easy to find libraries for everything

**Decision: React + Vite (fast build tool) + MUI (UI components)**

---

### Decision 3: Why GraphQL (not REST)?

This is the big one. Let me show you the difference:

**REST approach** (traditional):
```
GET /api/studies              → list of studies
GET /api/studies/123          → one study
GET /api/studies/123/sites    → sites for that study
GET /api/studies/123/sites/456/examiners  → examiners at that site for that study
```

Problem: To show a study detail page, you need 3-4 separate HTTP requests. Or you over-fetch everything in one bloated endpoint.

**GraphQL approach**:
```graphql
query {
  getStudy(id: "123") {
    title
    status
    sites {
      name
      examiners {
        name
        certificates { expiresOn }
      }
    }
  }
}
```

One request. You ask for exactly what you need. The server figures out how to get it.

**Why GraphQL wins for this project:**
- Deeply nested data (study → sites → examiners → certificates)
- Frontend can ask for exactly the fields it needs — no over-fetching
- Single endpoint (`/graphql`) — no need to design dozens of REST URLs
- Built-in type system — the schema IS your API documentation
- Apollo Client on frontend gives you caching, error handling, loading states for free

**Decision: GraphQL (Apollo Server on backend, Apollo Client on frontend)**

---

### Decision 4: Why SQLite (not PostgreSQL, MySQL, MongoDB)?

| Option | Pros | Cons |
|--------|------|------|
| PostgreSQL | Production-grade, powerful | Needs separate server, setup overhead |
| MySQL | Widely used | Same as Postgres — needs server |
| MongoDB | Flexible schema, JSON-like | Bad for relational data with joins |
| **SQLite** | Zero setup, single file, fast | Not for high-concurrency production |

For this project:
- It's a demo/learning app — no need for a separate database server
- Data is highly relational (studies ↔ sites ↔ examiners) → SQL is perfect
- SQLite is just a file (`app.db`) — no installation, no configuration
- `better-sqlite3` library gives synchronous API — simpler code, no async/await for DB calls

**Decision: SQLite via better-sqlite3**

---

### Decision 5: Why JWT in HttpOnly Cookies (not localStorage)?

```
localStorage approach:
  - Store token in browser's localStorage
  - Problem: Any JavaScript on the page can read it (XSS attack)

HttpOnly Cookie approach:
  - Browser stores the cookie automatically
  - JavaScript CANNOT read it (HttpOnly flag)
  - Browser sends it automatically with every request
  - Much more secure
```

**Decision: JWT access token (15 min) + refresh token (7 days), both in HttpOnly cookies**

---

### Decision 6: Supporting Libraries

| Need | Choice | Why |
|------|--------|-----|
| Form handling | react-hook-form | Performant, minimal re-renders |
| Validation | Zod | TypeScript-first, works on both frontend & backend |
| Toasts/notifications | notistack | Works with MUI, simple API |
| Charts | Chart.js | Lightweight, good enough for dashboards |
| Security headers | helmet | One-line Express middleware |
| Logging | Winston + Morgan | Structured logs, HTTP request logging |
| Password hashing | bcryptjs | Industry standard |

---

### The Final Architecture (What You Decided)

```
Frontend:  React + Vite + Apollo Client + MUI + react-hook-form + Zod + notistack
Backend:   Express + Apollo Server + SQLite (better-sqlite3) + JWT + Zod + Winston
```

Both in TypeScript. Both use Zod for validation. GraphQL connects them.

---

### How You'd Think About This in an Existing Codebase

When you join a project, look at `package.json` first. It tells you:
- What framework (React? Angular? Express? Fastify?)
- What API style (Apollo = GraphQL, axios = REST)
- What database (pg = PostgreSQL, better-sqlite3 = SQLite, mongoose = MongoDB)
- What auth (jsonwebtoken = JWT, passport = various strategies)

Once you know the tech, you know the patterns.

---

**Lesson 2 done.** Next is **Lesson 3: Project Structure** — how you organize folders so the code doesn't become a mess, and the philosophy behind this project's layout.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 1, Lesson 3: Project Structure

---

### The Thinking Process (Before You Write Any Code)

You've decided your tech. Now the first real question:

> "How do I organize my files so that when this project has 100+ files, I can still find anything in 5 seconds?"

The answer: **Separation by concern** — each folder has ONE job.

---

### Step 1: Monorepo Layout

You create ONE root folder with TWO independent packages:

```
SNA-y2/
├── backend/       ← Its own package.json, its own node_modules
├── frontend/      ← Its own package.json, its own node_modules
├── docs/          ← Documentation
└── e2e/           ← End-to-end tests
```

**Why separate packages?**
- Backend and frontend have completely different dependencies
- You can deploy them independently
- A new developer can work on frontend without touching backend (and vice versa)
- Each has its own `tsconfig.json` with different settings

---

### Step 2: Backend Folder Design (The Layered Architecture)

This is the most important concept. Think of it as floors in a building:

```
backend/src/
├── server.ts              ← FLOOR 0: Entry point (starts everything)
├── app.ts                 ← FLOOR 1: Express + Apollo wiring
├── middleware/            ← FLOOR 1.5: Security, logging, request ID
├── graphql/
│   ├── schema/            ← FLOOR 2: API contract (what can clients ask for?)
│   └── resolvers/         ← FLOOR 3: Request handlers (what happens when they ask?)
├── services/              ← FLOOR 4: Business logic (rules, decisions)
├── repositories/          ← FLOOR 5: Database queries (raw SQL)
├── db/                    ← FLOOR 6: Database connection + schema
├── validation/            ← UTILITY: Zod schemas (used by resolvers)
├── utils/                 ← UTILITY: JWT, password hashing, token generation
├── types/                 ← UTILITY: TypeScript interfaces
└── __tests__/             ← Tests (mirrors the src structure)
```

**The golden rule: Data flows DOWN, never UP.**

```
Resolver → calls → Service → calls → Repository → calls → Database
   ↓                  ↓                    ↓
 NEVER imports     NEVER imports       NEVER imports
 from Service      from Repository     from Service
   ↑                  ↑                    ↑
```

A resolver NEVER touches the database directly.
A service NEVER writes raw SQL.
A repository NEVER knows about GraphQL or business rules.

**Why?** Because when something breaks:
- Wrong data in response? → Check the resolver
- Business rule violated? → Check the service
- Wrong SQL query? → Check the repository
- Database schema issue? → Check db/migrate.ts

You know EXACTLY where to look.

---

### Step 3: Frontend Folder Design

```
frontend/src/
├── main.tsx               ← Entry point (renders App)
├── App.tsx                ← Router setup (all routes defined here)
├── theme.ts               ← MUI theme (colors, fonts, spacing)
├── components/            ← Reusable UI pieces
│   ├── admin/             ← Admin-specific layout components
│   ├── shared/            ← Used by both admin and viewer
│   ├── skeletons/         ← Loading placeholders
│   └── study/             ← Study-specific complex components
├── pages/                 ← Full page components (one per route)
│   ├── admin/             ← Admin pages (CRUD, detail, audit)
│   ├── viewer/            ← Viewer pages (read-only)
│   └── shared/            ← Pages used by both roles
├── hooks/                 ← Custom React hooks (data fetching)
├── services/              ← GraphQL query/mutation definitions
├── contexts/              ← React context (auth state)
├── validation/            ← Zod schemas for forms
├── utils/                 ← Helper functions
├── types/                 ← TypeScript interfaces
└── __tests__/             ← Tests
```

**The frontend philosophy:**
- `services/` = WHERE you define GraphQL queries (the "what to ask")
- `hooks/` = HOW you fetch data (wraps Apollo's useQuery)
- `pages/` = WHAT the user sees (full screens)
- `components/` = REUSABLE pieces used across pages

---

### Step 4: How Files Connect (The Import Chain)

**Backend — a request for "get all studies":**
```
graphql/resolvers/study.ts
  → imports from services/studyService.ts
    → imports from repositories/studyRepository.ts
      → imports from db/connection.ts
```

**Frontend — showing the studies list:**
```
pages/admin/StudiesPage.tsx
  → imports useStudies from hooks/useStudies.ts
    → imports GET_STUDIES_QUERY from services/studyService.ts
      → uses Apollo Client from utils/apolloClient.ts
```

---

### Step 5: The Naming Conventions (So You Can Find Anything)

| What | Convention | Example |
|------|-----------|---------|
| Files | camelCase | `studyService.ts`, `apolloClient.ts` |
| React components | PascalCase | `AdminStudiesPage.tsx` |
| Hooks | use prefix | `useStudies.ts`, `useAuth.ts` |
| GraphQL constants | SCREAMING_SNAKE | `GET_STUDIES_QUERY`, `CREATE_STUDY_MUTATION` |
| DB row types | PascalCase + Row | `StudyRow`, `SiteRow` |
| Repositories | domain + Repository | `studyRepository.ts` |
| Services | domain + Service | `studyService.ts` |

**Why this matters:** When you see `useStudies` in code, you INSTANTLY know:
- It's a hook (starts with `use`)
- It's about studies
- It lives in `hooks/useStudies.ts`

---

### Step 6: The "Barrel" Pattern (index.ts files)

You'll see `index.ts` files in many folders:

```typescript
// components/study/index.ts
export { StudySitePanel } from './StudySitePanel';
export { CertificatePickerDialog } from './CertificatePickerDialog';
```

This lets other files import cleanly:
```typescript
// Instead of:
import { StudySitePanel } from '../components/study/StudySitePanel';

// You write:
import { StudySitePanel } from '../components/study';
```

---

### Step 7: If You Were Starting From Scratch — The First Files

Here's the exact order you'd create files:

```
Day 1 (Backend skeleton):
  1. backend/package.json          ← npm init, install dependencies
  2. backend/tsconfig.json         ← TypeScript config
  3. backend/.env                  ← Environment variables
  4. backend/src/server.ts         ← "Hello world" Express server
  5. backend/src/app.ts            ← Express app setup

Day 2 (Database):
  6. backend/src/db/connection.ts  ← SQLite connection
  7. backend/src/db/migrate.ts     ← Create tables
  8. backend/src/types/index.ts    ← Row interfaces

Day 3 (First feature — auth):
  9. backend/src/utils/jwt.ts      ← Token signing
  10. backend/src/utils/password.ts ← Bcrypt helpers
  ... and so on
```

We'll cover this exact build order in detail in Phase 5.

---

### The Mental Model for Existing Codebases

When you open ANY project for the first time:

1. **Read `package.json`** — what tech is used?
2. **Find the entry point** — `server.ts`, `main.tsx`, `index.ts`
3. **Identify the layers** — where's the API? Where's the business logic? Where's the DB?
4. **Trace one request** — pick one feature, follow it from UI to database and back
5. **Understand the naming** — once you see the pattern, you can find anything

---

**Phase 1 complete!** You now understand:
- ✅ What the app does (domain)
- ✅ Why each technology was chosen
- ✅ How the folders are organized and why
- ✅ How files connect to each other
- ✅ The naming conventions

**Next: Phase 2, Lesson 4 — Entry Point.** We'll open the actual `server.ts` and `app.ts` files and I'll show you how the backend starts up, line by line.

Say **"next"** to continue.

---

next

---

## Phase 2, Lesson 4: Entry Point — How the Backend Starts

---

### The Thinking Process

> "I have an empty `backend/src/` folder. What's the FIRST file I write?"

Answer: The file that starts your server. Everything else is useless if the server doesn't run.

You need TWO files:
- `server.ts` — the entry point (validates environment, initializes DB, starts listening)
- `app.ts` — the Express app configuration (middleware, routes, Apollo)

**Why two files?** Because in tests, you want to import `app` without actually starting the server on a port.

---

### Let me show you the actual files:

---

---

### Breaking Down `server.ts` (The Boot Sequence)

Think of this as the ignition key of a car. It does 4 things in order:

```
Step 1: Load environment variables (.env file)
Step 2: Validate them (crash early if something's missing)
Step 3: Connect to database + create tables
Step 4: Create the Express app + start listening
```

Let me walk through each line:

```typescript
import 'dotenv/config';  // Reads .env file → puts values into process.env
```
This is always the FIRST import. Without it, `process.env.PORT` would be undefined.

```typescript
function validateEnv(): void {
  const result = envSchema.safeParse(process.env);
  if (!result.success) {
    throw new Error(`Invalid environment variables:\n${issues}`);
  }
}
```
**Why validate env?** Imagine you deploy and forget to set `JWT_SECRET`. Without validation, the app starts but auth silently breaks. With validation, it crashes immediately with a clear error message. **Fail fast, fail loud.**

```typescript
initConnection(process.env.DB_PATH ?? './data/app.db');  // Open SQLite file
initDb();  // Create tables if they don't exist
```
Database must be ready BEFORE the server accepts requests.

```typescript
const app = await createApp();  // Build the Express app (from app.ts)
app.listen(port, () => { ... });  // Start accepting HTTP requests
```

```typescript
start().catch((err) => logger.error('Failed to start server', { err }));
```
If ANYTHING fails during startup, log it and crash. Don't run a broken server.

---

### Breaking Down `app.ts` (The Express Configuration)

This is where you wire everything together. Think of it as an assembly line — each request passes through layers:

```
Request arrives
  → helmet (security headers)
  → requestId (attach unique ID for tracing)
  → morgan/winston (log the request)
  → cors (allow frontend origin)
  → express.json (parse JSON body)
  → cookieParser (parse cookies)
  → rate limiting (block abuse)
  → Apollo Server (process GraphQL)
```

**The most important part — the context function:**

```typescript
context: async ({ req, res }) => {
  const token = req.cookies?.auth_token ?? null;
  const user = token ? verifyToken(token) : null;
  return { user, req, res, requestId: req.requestId, loaders: createLoaders() };
},
```

This runs on EVERY GraphQL request. It:
1. Reads the JWT cookie from the request
2. Verifies it (returns user info or null)
3. Passes `user` to every resolver — so resolvers know WHO is making the request
4. Creates fresh DataLoaders (for N+1 prevention — we'll cover later)

**If user is null** → the request is unauthenticated. Resolvers that call `requireAuth()` will reject it.

---

### The Health Check (Simple but Important)

```typescript
app.get('/health', (_req, res) => {
  getDb().prepare('SELECT 1').get();
  res.json({ status: 'ok', db: 'ok' });
});
```

This is the ONLY REST endpoint. It exists so monitoring tools can check "is the server alive and can it reach the database?" — useful in production.

---

### Key Design Decisions to Notice

1. **`createApp()` is async and exported** — tests can import it without starting a real server
2. **Context is built per-request** — every request gets its own `user`, its own `loaders`
3. **Error formatting strips stack traces** — never leak internal details to clients
4. **Introspection disabled in production** — attackers can't explore your API schema
5. **Rate limiting BEFORE GraphQL** — abusive requests are blocked before they hit resolvers

---

### If You Were Building This From Scratch

You'd write it in this order:

```
1. npm init → package.json
2. npm install express cors cookie-parser dotenv
3. Create server.ts with just:
     import express from 'express';
     const app = express();
     app.listen(4040, () => console.log('running'));
4. Verify it works: npm run dev → see "running" in terminal
5. Add middleware one by one (cors, json, cookieParser)
6. Add Apollo Server later (after you have schema + resolvers)
```

**Always start with the simplest possible working server, then add layers.**

---

### How This Connects to Everything Else

```
server.ts
  ├── imports db/connection.ts      (Lesson 6 — Database)
  ├── imports db/migrate.ts         (Lesson 6 — Database)
  ├── imports validation/envSchema  (Lesson 13 — Validation)
  └── imports app.ts
        ├── imports graphql/schema    (Lesson 9 — GraphQL Schema)
        ├── imports graphql/resolvers (Lesson 10 — Resolvers)
        ├── imports graphql/loaders   (Lesson 15 — DataLoaders)
        ├── imports utils/jwt.ts      (Lesson 11 — Auth)
        ├── imports middleware/*       (Lesson 5 — Middleware)
        └── imports logger/*          (Lesson 5 — Middleware)
```

---

**Lesson 4 done.** Next is **Lesson 5: Middleware** — security headers, rate limiting, request IDs, and logging. These are the "invisible guards" that protect your app.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 2, Lesson 5: Middleware — The Invisible Guards

---

### The Thinking Process

> "My server starts. But before any request reaches my business logic, I need to protect it, track it, and log it."

Middleware = functions that run BETWEEN the request arriving and your code handling it. Think of them as security checkpoints at an airport:

```
Request arrives at server
  → Checkpoint 1: Security headers (helmet)
  → Checkpoint 2: Attach tracking ID (requestId)
  → Checkpoint 3: Log the request (morgan/winston)
  → Checkpoint 4: Allow/block origin (CORS)
  → Checkpoint 5: Parse the body (express.json)
  → Checkpoint 6: Parse cookies (cookieParser)
  → Checkpoint 7: Rate limiting (block abuse)
  → ✅ Finally reaches your GraphQL resolver
```

If any checkpoint fails, the request is rejected before it wastes your server's resources.

---

### Let me show you the actual middleware files:

---

---

### Middleware 1: Security Headers (Helmet)

```typescript
export const helmetMiddleware = helmet({
  contentSecurityPolicy: process.env.NODE_ENV === 'production',
});
```

**What it does:** Adds HTTP headers that tell the browser "be strict about security":
- `X-Content-Type-Options: nosniff` — don't guess file types
- `X-Frame-Options: DENY` — can't embed this site in an iframe (prevents clickjacking)
- `Strict-Transport-Security` — force HTTPS
- `Content-Security-Policy` — control what scripts/styles can load (disabled in dev because Vite needs flexibility)

**Why?** One line of code, massive security improvement. No reason NOT to use it.

---

### Middleware 2: Request ID

```typescript
export function requestIdMiddleware(req: Request, res: Response, next: NextFunction): void {
  req.requestId = randomUUID();
  res.setHeader('X-Request-Id', req.requestId);
  next();
}
```

**What it does:** Every request gets a unique ID (like `a3f7b2c1-...`).

**Why?** Imagine 100 users hit your server at the same time. Something fails. Your logs show:
```
ERROR: Database query failed
ERROR: Database query failed
ERROR: Database query failed
```

Which user? Which request? No idea.

With request IDs:
```
ERROR [req:a3f7b2c1]: Database query failed
```

Now you can trace the ENTIRE journey of one request through all your logs. This is essential in production.

---

### Middleware 3: Logging (Winston + Morgan)

**Winston** = your structured logger:
```typescript
const logger = createLogger({
  level: process.env.LOG_LEVEL ?? (isProd ? 'info' : 'debug'),
  format: isProd ? format.json() : format.colorize() + format.printf(...)
});
```

- In development: colorful, human-readable logs (`10:30:45 info: Server running...`)
- In production: JSON format (machines can parse it, send to monitoring tools)

**Morgan** = HTTP request logger:
```typescript
const requestLogger = morgan('combined', { stream });
```

Logs every HTTP request automatically:
```
GET /graphql 200 45ms
POST /graphql 401 12ms
```

**The clever part:** Morgan pipes into Winston (`stream.write → logger.http`), so ALL logs go through one system.

---

### Middleware 4: Rate Limiting

**General rate limit:**
```typescript
export const graphqlRateLimit = rateLimit({
  windowMs: 60 * 1000,     // 1 minute window
  max: 500,                 // max 500 requests per IP per minute
});
```

**Why?** Without this, someone could send 10,000 requests per second and crash your server (DDoS attack).

**Login-specific rate limit:**
```typescript
// 20 attempts per 15 minutes per IP+email combination
```

**Why separate?** Login is the most attacked endpoint. If someone tries to brute-force a password, you block them after 20 attempts. But you key it by IP+email, so:
- Attacker trying `admin@test.com` gets blocked
- Legitimate user trying `viewer@test.com` from the same IP is NOT blocked

**The smart detection:**
```typescript
const isLoginMutation = body?.operationName === 'Login' ||
  (typeof req.body?.query === 'string' && req.body.query.includes('login('));
```

It only applies the strict limit to login mutations — all other GraphQL operations use the general 500/min limit.

---

### Middleware 5: CORS (Cross-Origin Resource Sharing)

This was in `app.ts`:
```typescript
app.use(cors({ origin: 'http://localhost:5173', credentials: true }));
```

**What problem does it solve?**

Your frontend runs on `localhost:5173`. Your backend runs on `localhost:4040`. By default, browsers BLOCK requests between different origins (ports count as different origins).

CORS tells the browser: "It's okay, I trust requests from `localhost:5173`."

`credentials: true` = "Also send cookies with cross-origin requests" (needed for our HttpOnly auth cookie).

---

### The Order Matters!

```typescript
// In app.ts — this order is intentional:
app.use(helmetMiddleware);      // 1. Security headers FIRST
app.use(requestIdMiddleware);   // 2. ID for tracking
app.use(requestLogger);         // 3. Log the request (now has ID)
app.use(cors(...));             // 4. CORS check
app.use(express.json());        // 5. Parse body
app.use(cookieParser());        // 6. Parse cookies
// ... then rate limiting and GraphQL
```

**Why this order?**
- Helmet goes first because security headers should be on EVERY response, even errors
- Request ID goes before logging so the log includes the ID
- CORS goes before body parsing — if origin is blocked, don't waste time parsing
- Cookie parser goes before GraphQL — resolvers need to read the auth cookie

---

### The `next()` Function — How Middleware Chains Work

Every middleware has this signature:
```typescript
function myMiddleware(req: Request, res: Response, next: NextFunction): void {
  // Do something with req/res
  next();  // Pass to the NEXT middleware in the chain
}
```

If you DON'T call `next()`, the request stops there. That's how rate limiting works — if limit exceeded, it sends a response and never calls `next()`.

---

### If You Were Building From Scratch

```
1. Start with NO middleware — just get the server running
2. Add cors (you'll need it immediately when frontend tries to call backend)
3. Add express.json + cookieParser (needed for GraphQL and auth)
4. Add helmet (one line, instant security)
5. Add requestId + logging (when you start debugging issues)
6. Add rate limiting (before going to production)
```

Don't add everything at once. Add each middleware when you NEED it.

---

### Key Takeaway for Existing Codebases

When you open any Express app, look at the middleware stack in `app.ts` (or `app.js`). It tells you:
- What security measures are in place
- How requests are logged
- What parsing is available (JSON? form data? cookies?)
- What rate limits exist

It's the "security posture" of the application in one file.

---

**Lesson 5 done.** Next is **Lesson 6: Database Setup** — how you design tables, create the schema, handle migrations, and seed initial data. This is where your data model comes to life.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 2, Lesson 6: Database Setup

---

### The Thinking Process

> "My server runs, middleware is in place. Now I need somewhere to STORE data. How do I design my tables? How do I create them? How do I handle changes over time?"

Three files handle this:
- `connection.ts` — opens the SQLite file
- `migrate.ts` — creates tables, indexes, seeds data
- `query.ts` — typed helper functions for running SQL

---

### Let me show you the actual files:

---

---

### File 1: `connection.ts` — The Database Singleton

```typescript
let db: Database.Database;

export function getDb(): Database.Database {
  return db;
}

export function initConnection(dbPath: string): void {
  fs.mkdirSync(path.dirname(dbPath), { recursive: true });
  db = new Database(dbPath);
}
```

**What's happening:**
- `db` is a module-level variable — there's only ONE connection for the entire app (singleton pattern)
- `initConnection` creates the folder if it doesn't exist, then opens the SQLite file
- `getDb()` is how every other file accesses the database — they never create their own connection

**Why a singleton?** SQLite is a file-based database. Opening multiple connections to the same file causes locking issues. One connection, shared everywhere.

**Why `getDb()` function instead of exporting `db` directly?** Because `db` is `undefined` until `initConnection` is called. If you exported it directly, other files would import `undefined` at module load time. The function ensures you always get the initialized instance.

---

### File 2: `query.ts` — Typed SQL Helpers

```typescript
export function queryAll<T>(sql: string, params: unknown[] = []): T[] {
  return getDb().prepare(sql).all(...params) as T[];
}

export function queryOne<T>(sql: string, params: unknown[] = []): T | undefined {
  return getDb().prepare(sql).get(...params) as T | undefined;
}
```

**Only 2 functions.** That's it. But they're used EVERYWHERE.

**What they do:**
- `queryAll<StudyRow>('SELECT * FROM studies')` → returns an array of `StudyRow` objects
- `queryOne<UserRow>('SELECT * FROM users WHERE id = ?', [5])` → returns one `UserRow` or `undefined`

**Why these helpers?**
1. **Type safety** — the generic `<T>` tells TypeScript what shape the result has
2. **Parameterized queries** — `params` array prevents SQL injection (NEVER concatenate user input into SQL strings)
3. **DRY** — without these, every query would repeat `getDb().prepare(sql).all(...)` 

**SQL Injection — the #1 security rule:**
```typescript
// ❌ NEVER DO THIS — attacker can inject SQL
const sql = `SELECT * FROM users WHERE email = '${userInput}'`;

// ✅ ALWAYS DO THIS — parameterized, safe
const sql = `SELECT * FROM users WHERE email = ?`;
queryOne<UserRow>(sql, [userInput]);
```

---

### File 3: `migrate.ts` — Schema + Migrations + Seeds

This is the longest file. Let me break it into 4 parts:

---

#### Part A: Table Creation (Schema Design)

**How you think about table design:**

Start with your entities and their fields:

```
Study: protocolId (unique), title, sponsor, phase, startDate, endDate, status, description
Site: siteCode (unique), name, city, country, status
Examiner: examinerCode (unique), name, specialty, email, role, status
```

Then think about relationships:

```
Study ←→ Site (many-to-many) → need a junction table: study_sites
Site ←→ Examiner (many-to-many) → need a junction table: site_examiners
Study + Site + Examiner (3-way) → need: study_site_examiners
```

**Junction tables explained:**

A study can have many sites. A site can be in many studies. You can't represent this with a single column. You need a separate table:

```
study_sites:
  study_id | site_id
  ---------|--------
  1        | 3        ← Study 1 runs at Site 3
  1        | 7        ← Study 1 also runs at Site 7
  2        | 3        ← Study 2 also runs at Site 3
```

Primary key is `(study_id, site_id)` — prevents duplicates.

**CHECK constraints — database-level validation:**
```sql
status TEXT NOT NULL CHECK(status IN ('Planned','Active','Completed'))
```

Even if your application code has a bug, the DATABASE will reject invalid values. Defense in depth.

**REFERENCES (Foreign Keys):**
```sql
study_id INTEGER NOT NULL REFERENCES studies(id)
```

This means: "study_id MUST be a valid id from the studies table." You can't assign a non-existent study.

---

#### Part B: Indexes (Performance)

```sql
CREATE INDEX IF NOT EXISTS idx_studies_title ON studies(title);
CREATE INDEX IF NOT EXISTS idx_audit_entity ON audit_logs(entityType, entityId);
```

**What's an index?** Think of it like the index at the back of a textbook. Without it, to find "Chapter 5", you'd flip through every page. With it, you look up "Chapter 5 → page 87" instantly.

**When to add indexes:**
- Columns you search/filter by frequently (title, status, name)
- Columns you JOIN on (foreign keys in junction tables)
- Columns you ORDER BY frequently

**Trade-off:** Indexes speed up reads but slow down writes (the index must be updated on every INSERT/UPDATE). For this app, reads far outnumber writes, so indexes are worth it.

---

#### Part C: Migration Shims (Handling Schema Changes)

```typescript
try { 
  db.exec(`ALTER TABLE users ADD COLUMN role TEXT NOT NULL DEFAULT 'VIEWER'`); 
} catch { /* already exists */ }
```

**The problem:** You built the app. It's running. Users have data. Now you need to add a new column. You can't just drop and recreate the table — you'd lose all data.

**The solution:** `ALTER TABLE ... ADD COLUMN` wrapped in try/catch. If the column already exists, SQLite throws an error, you catch it and move on. Idempotent — safe to run multiple times.

**The audit_logs migration is more complex:**
```typescript
// Try inserting an ASSIGN action — if old CHECK constraint rejects it, recreate the table
try {
  db.prepare(`INSERT INTO audit_logs ... 'ASSIGN' ...`).run();
  db.prepare(`DELETE FROM audit_logs WHERE ...`).run();  // Clean up test row
} catch {
  // Old constraint doesn't allow ASSIGN — recreate table with new constraint
  db.exec(`ALTER TABLE audit_logs RENAME TO audit_logs_old; ...`);
}
```

This is a real-world pattern: you can't ALTER a CHECK constraint in SQLite, so you rename the old table, create a new one with the correct constraint, copy data over, and drop the old one.

---

#### Part D: Seed Data

```typescript
function seedUsers(db) {
  if (!queryOne('SELECT id FROM users WHERE email = ?', ['admin@test.com'])) {
    db.prepare('INSERT INTO users (email, password, role) VALUES (?, ?, ?)').run(
      'admin@test.com', hashPassword('password123'), 'ADMIN'
    );
  }
}
```

**Why seed?** You need at least one user to log in. Without seeding, you'd have no way to access the app after a fresh install.

**Why check before inserting?** Idempotency. If you run `initDb()` 100 times, it should create the user only ONCE. The `if (!queryOne(...))` check prevents duplicates.

**Password is hashed:** Never store plain text passwords. `hashPassword('password123')` → stores something like `$2a$10$xK3j...` (bcrypt hash).

---

### The Complete Data Model (Visual)

```
┌──────────┐       ┌─────────────┐       ┌──────────┐
│  studies │──M:M──│ study_sites │──M:M──│  sites   │
└──────────┘       └─────────────┘       └──────────┘
                                               │
                                              M:M
                                               │
                                         ┌──────────────┐
                                         │site_examiners│
                                         └──────────────┘
                                               │
                                              M:M
                                               │
┌──────────────────────┐                 ┌───────────┐
│study_site_examiners  │─────────────────│ examiners │
│(3-way + certificate) │                 └───────────┘
└──────────────────────┘                       │
         │                                    1:M
         │                                     │
         └──────────────────────────────┌──────────────────────┐
                                        │examiner_certificates │
                                        └──────────────────────┘

┌───────────┐     ┌────────────────┐     ┌────────────┐
│   users   │────▶│ refresh_tokens │     │ audit_logs │
└───────────┘     └────────────────┘     └────────────┘
```

---

### If You Were Building From Scratch — The Order

```
1. Create connection.ts (just getDb + initConnection)
2. Create query.ts (queryAll + queryOne — you'll use these immediately)
3. Create migrate.ts with ONLY the users table (you need auth first)
4. Test: run server → check that app.db file appears
5. Add studies table (your first real entity)
6. Add sites, examiners tables
7. Add junction tables (study_sites, site_examiners)
8. Add indexes (when you notice queries getting slow)
9. Add study_site_examiners + examiner_certificates (advanced features)
10. Add audit_logs + refresh_tokens (when you build those features)
```

**Key principle: Build tables as you build features. Don't design the entire schema upfront.**

---

### Key Takeaways

1. **Singleton connection** — one `getDb()` function, called inside other functions (never at module load)
2. **Typed helpers** — `queryAll<T>` and `queryOne<T>` give you type safety + SQL injection protection
3. **CREATE TABLE IF NOT EXISTS** — idempotent, safe to run repeatedly
4. **CHECK constraints** — database enforces valid values even if app code has bugs
5. **Junction tables** — how you model many-to-many relationships
6. **Migration shims** — ALTER TABLE in try/catch for backward compatibility
7. **Seed data** — check-before-insert pattern for idempotency
8. **Indexes** — add them on columns you search/filter/join on

---

**Lesson 6 done.** Next is **Lesson 7: Repository Layer** — where all the raw SQL queries live, organized by domain. This is the layer that talks directly to the database.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 2, Lesson 7: Repository Layer

---

### The Thinking Process

> "I have my database and typed helpers. Now where do I write my actual SQL queries? Do I put them in the service? In the resolver?"

Answer: **Neither.** You create a dedicated repository layer. Each domain entity gets its own repository file.

**Why separate repositories?**
- Services contain business logic (rules, decisions) — they shouldn't know SQL syntax
- Resolvers handle GraphQL concerns — they shouldn't know about databases at all
- Repositories are PURE data access — "give me this data" or "save this data"

```
Resolver: "I need the study with ID 5"
  → Service: "Let me check if you're allowed to see it"
    → Repository: "SELECT * FROM studies WHERE id = 5"
```

If you ever switch from SQLite to PostgreSQL, you ONLY change repository files. Services and resolvers stay untouched.

---

### Let me show you the actual repository files:

---

---

### The Repository Pattern — What You're Looking At

Each repository file follows the same structure:

```
1. Import typed helpers (queryAll, queryOne, getDb)
2. Import TypeScript interfaces (StudyRow, SiteRow, etc.)
3. Export functions — each does ONE database operation
```

No business logic. No validation. No auth checks. Just: "You give me parameters, I give you data."

---

### Breaking Down the Patterns

#### Pattern 1: Find by ID

```typescript
export function findStudyById(id: number): StudyRow | null {
  return queryOne<StudyRow>('SELECT * FROM studies WHERE id = ?', [id]) ?? null;
}
```

- Takes an `id`
- Returns the row OR `null` (not `undefined` — cleaner for callers)
- `?? null` converts `undefined` (from queryOne) to `null`

#### Pattern 2: Paginated List

```typescript
export function findStudiesPaged(pageSize: number, offset: number): { rows: StudyRow[]; total: number } {
  const rows = queryAll<StudyRow>('SELECT * FROM studies ORDER BY id ASC LIMIT ? OFFSET ?', [pageSize, offset]);
  const total = (queryOne<{ cnt: number }>('SELECT COUNT(*) as cnt FROM studies') ?? { cnt: 0 }).cnt;
  return { rows, total };
}
```

- Two queries: one for the page of data, one for the total count
- `LIMIT ? OFFSET ?` = pagination in SQL (e.g., LIMIT 10 OFFSET 20 = skip 20, take 10)
- Returns `{ rows, total }` — frontend needs both to show "Page 2 of 5"

#### Pattern 3: Find Related Entities (JOIN)

```typescript
export function findSitesByStudyId(studyId: number): SiteRow[] {
  return queryAll<SiteRow>(
    `SELECT si.* FROM sites si 
     JOIN study_sites ss ON ss.site_id = si.id 
     WHERE ss.study_id = ?`,
    [studyId]
  );
}
```

**How JOINs work (simplified):**
```
study_sites table:          sites table:
study_id | site_id          id | name
---------|--------          ---|------
1        | 3                3  | Apollo Hospital
1        | 7                7  | AIIMS Delhi

JOIN says: "Match study_sites.site_id with sites.id"
WHERE says: "Only for study_id = 1"
Result: Apollo Hospital, AIIMS Delhi
```

#### Pattern 4: Check Existence

```typescript
export function protocolIdExists(protocolId: string): boolean {
  return !!queryOne('SELECT id FROM studies WHERE protocolId = ?', [protocolId]);
}
```

- `!!` converts truthy/falsy to boolean
- Only selects `id` (not `*`) — we don't need the full row, just "does it exist?"
- Used by services to enforce uniqueness before INSERT

#### Pattern 5: Insert and Return ID

```typescript
export function insertStudy(...): number {
  const result = getDb()
    .prepare('INSERT INTO studies (...) VALUES (?,?,?,?,?,?,?,?)')
    .run(protocolId, title, sponsor, phase, startDate, endDate, 'Planned', description);
  return result.lastInsertRowid as number;
}
```

- Uses `getDb().prepare().run()` directly (not queryAll/queryOne — those are for SELECT)
- `lastInsertRowid` gives you the auto-generated ID of the new row
- Notice: status is HARDCODED as `'Planned'` — the repository enforces this, not the caller

#### Pattern 6: Dynamic Update

```typescript
export function updateStudyById(id: number, fields: Array<[string, unknown]>): void {
  const setClauses = fields.map(([k]) => `${k} = ?`).join(', ');
  const values = fields.map(([, v]) => v);
  getDb().prepare(`UPDATE studies SET ${setClauses} WHERE id = ?`).run(...values, id);
}
```

- Takes an array of `[columnName, value]` pairs
- Builds the SET clause dynamically: `SET title = ?, status = ?`
- Only updates the fields that changed — not the entire row

**Why dynamic?** Because `updateStudy` might change just the title, or just the status, or both. You don't want 10 different update functions.

#### Pattern 7: Junction Table Operations

```typescript
export function insertStudySite(studyId: number, siteId: number): void {
  getDb().prepare('INSERT OR IGNORE INTO study_sites (study_id, site_id) VALUES (?, ?)').run(studyId, siteId);
}

export function deleteStudySite(studyId: number, siteId: number): void {
  getDb().prepare('DELETE FROM study_sites WHERE study_id = ? AND site_id = ?').run(studyId, siteId);
}
```

- `INSERT OR IGNORE` — if the pair already exists, do nothing (idempotent)
- `DELETE` — removes the relationship (unassign)
- These are the "assign" and "unassign" operations

#### Pattern 8: Count for Business Rules

```typescript
export function countExaminersForSite(siteId: number): number {
  return (queryOne<{ cnt: number }>('SELECT COUNT(*) as cnt FROM site_examiners WHERE site_id = ?', [siteId]) ?? { cnt: 0 }).cnt;
}
```

- Services use this to check rules like "site needs ≥1 examiner to be Active"
- Returns a number, not rows — efficient

---

### The Auth Repository (Simplest One)

```typescript
export function findUserByEmail(email: string): UserRow | null { ... }
export function findUserById(id: number): Omit<UserRow, 'password'> | null { ... }
```

Notice `findUserById` returns `Omit<UserRow, 'password'>` — it explicitly EXCLUDES the password hash from the result. Security by design — you never accidentally leak the password.

---

### The Audit Repository

```typescript
export function insertAuditLog(actorUserId, actorEmail, action, entityType, entityId, beforeJson, afterJson): void { ... }

export function queryAuditLogs(types, entityId, pageSize, offset): { rows, total } { ... }
```

`queryAuditLogs` handles 3 cases:
1. Filter by types AND entityId (per-entity history)
2. Filter by types only (global audit page with filter)
3. No filter (all audit logs)

**The dynamic IN clause:**
```typescript
const ph = types.map(() => '?').join(',');  // Creates "?,?,?" for 3 types
`WHERE entityType IN (${ph})`              // Becomes "WHERE entityType IN (?,?,?)"
```

This is how you do parameterized `IN` queries — you can't use a single `?` for an array.

---

### The Complete Repository Map

```
repositories/
├── authRepository.ts        ← findUserByEmail, findUserById
├── studyRepository.ts       ← findStudyById, findStudiesPaged, insertStudy, updateStudy, junction ops, SSE ops
├── siteRepository.ts        ← findSiteById, findSitesPaged, insertSite, updateSite, examiner junction ops
├── examinerRepository.ts    ← findExaminerById, findExaminersPaged, insertExaminer, updateExaminer
├── certificateRepository.ts ← findCertificatesByExaminerId, insertCertificate, updateCertificate
├── auditRepository.ts       ← insertAuditLog, queryAuditLogs
├── refreshTokenRepository.ts ← insertRefreshToken, findRefreshToken, revokeRefreshToken
└── searchRepository.ts      ← searchStudies, searchSites, searchExaminers (LIKE queries)
```

Each domain = one file. Easy to find, easy to test.

---

### If You Were Building From Scratch

```
1. Start with authRepository.ts (you need login first)
   - findUserByEmail (for login)
   - findUserById (for "me" query)

2. Then studyRepository.ts (your first real entity)
   - findStudyById
   - findStudiesPaged
   - insertStudy
   - updateStudyById

3. Then siteRepository.ts + examinerRepository.ts (same patterns)

4. Then junction operations (when you build assignment features)
   - insertStudySite, deleteStudySite

5. Then auditRepository.ts (when you build audit logging)

6. Then searchRepository.ts (when you build search)

7. Then refreshTokenRepository.ts (when you add refresh tokens)
```

**Build each repository function WHEN the service needs it. Don't write all queries upfront.**

---

### Key Takeaways

1. **One repository per domain** — studies, sites, examiners, auth, audit, etc.
2. **Functions do ONE thing** — find, insert, update, delete, count
3. **Always parameterized** — never concatenate user input into SQL
4. **Return typed data** — `StudyRow | null`, `{ rows: T[]; total: number }`
5. **No business logic** — repositories don't know about rules, they just read/write data
6. **INSERT OR IGNORE** — for junction tables (idempotent assigns)
7. **Dynamic updates** — `fields: Array<[string, unknown]>` pattern for flexible updates
8. **Batch queries** — `findStudiesByIds` for DataLoader (we'll cover in Lesson 15)

---

**Lesson 7 done.** Next is **Lesson 8: Service Layer** — where business rules live. This is the BRAIN of the application. It decides "is this operation allowed?" before telling the repository to do anything.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 2, Lesson 8: Service Layer — The Brain

---

### The Thinking Process

> "I have repositories that can read/write data. But who decides IF a write should happen? Who enforces 'a study can't become Active without sites'? Who checks 'this protocol ID is already taken'?"

Answer: **The service layer.** It sits between resolvers and repositories:

```
Resolver: "User wants to update study 5 to Active"
  → Service: "Let me check... does study 5 have sites? examiners? Is startDate ≤ today? 
              Yes to all → okay, tell the repository to update it"
    → Repository: "UPDATE studies SET status = 'Active' WHERE id = 5"
```

**Services contain ALL business logic. If a rule exists, it lives here.**

---

### Let me show you the actual service files:

---

---

### The Service Layer — What You're Looking At

Each service file has the same structure:

```
1. Import from repositories (data access)
2. Import types
3. Export query functions (simple pass-through to repository)
4. Export mutation functions (business logic + validation + repository calls)
```

---

### Key Patterns in the Service Layer

#### Pattern 1: Simple Query Pass-Through

```typescript
export function getStudiesPaged(page: number, pageSize: number): { rows: StudyRow[]; total: number } {
  return findStudiesPaged(pageSize, (page - 1) * pageSize);
}
```

- Converts `page` (human-friendly: 1, 2, 3) to `offset` (SQL-friendly: 0, 10, 20)
- No business logic needed for reads — just translate and delegate

#### Pattern 2: Create with Validation

```typescript
export function createStudy(input: CreateStudyInput): StudyRow {
  // Rule D1: startDate must be ≥ today
  if (input.startDate < today) {
    throw new GraphQLError('Start date cannot be in the past.', { ... });
  }
  // Rule S8: protocolId must be unique
  if (protocolIdExists(input.protocolId)) {
    throw new GraphQLError('Protocol ID already exists', { ... });
  }
  // All rules pass → insert
  const id = insertStudy(...);
  return findStudyById(id)!;
}
```

**The pattern:**
1. Check all business rules FIRST
2. If any rule fails → throw GraphQLError with `BAD_USER_INPUT` code + `fieldErrors`
3. If all pass → call repository to insert
4. Return the newly created row

#### Pattern 3: Update with Status Transitions

This is the most complex logic in the app. Let me explain the thinking:

```typescript
export function updateStudy(id: number, input: UpdateStudyInput): StudyRow {
  // 1. Find existing record
  const existing = findStudyById(id);
  if (!existing) throw new GraphQLError('Study not found');

  // 2. If status is changing, enforce transition rules
  if (input.status !== undefined && input.status !== existing.status) {
    enforceStatusTransition(existing, input.status, { startDate: input.startDate, endDate: input.endDate });
  }

  // 3. Build update fields (only changed ones)
  const fields = Object.entries(input).filter(([, v]) => v !== undefined);
  if (fields.length === 0) return existing;  // Nothing to update

  // 4. Execute update
  updateStudyById(id, fields);
  return findStudyById(id)!;
}
```

#### Pattern 4: Status Transition Rules (The Heart of Domain Logic)

```typescript
function enforceStatusTransition(existing, newStatus, inputDates): void {
  // S2: Forward-only (Planned→Active→Completed, never backward)
  if (toOrder !== fromOrder + 1) throw ...

  if (to === 'Active') {
    // S3: Must have ≥1 site
    // S4: Must have ≥1 examiner
    // D7: No Closed sites
    // D4: startDate ≤ today
    // D5: endDate ≥ today (if present)
  }

  if (to === 'Completed') {
    // S5: Must have ≥1 site
    // S6: Must have ≥1 examiner
    // D8: No Active sites
    // D6: endDate required, ≤ today, ≥ startDate
  }
}
```

**Why is this a separate function?** Because it's complex enough to deserve isolation. It makes the main `updateStudy` function readable, and it's easy to test independently.

#### Pattern 5: Assignment with Prerequisites

```typescript
export function assignExaminerToSite(siteId: number, examinerId: number): void {
  // Check: site exists?
  const site = findSiteById(siteId);
  if (!site) throw ...

  // SI3: site not Closed?
  if (site.status === 'Closed') throw ...

  // Check: examiner exists?
  if (!findExaminerById(examinerId)) throw ...

  // SI6: examiner has valid certificate?
  if (!hasValidCertificate(examinerId)) throw ...

  // All checks pass → insert the relationship
  insertSiteExaminer(siteId, examinerId);
}
```

#### Pattern 6: Unassign with Side Effects

```typescript
export function unassignExaminerFromSite(siteId: number, examinerId: number): void {
  // SI4: block if examiner is in SSE for this site
  if (countSSEForSiteExaminer(siteId, examinerId) > 0) throw ...

  // P2: if this is the last examiner on an Active site → auto-downgrade
  if (site.status === 'Active' && countExaminersForSite(siteId) - 1 === 0) {
    downgradeSiteToPlanned(siteId);
  }

  deleteSiteExaminer(siteId, examinerId);
}
```

**This is a side effect** — removing an examiner can change the site's status. The service knows this rule; the repository doesn't.

#### Pattern 7: Certificate Resolution (SSE Assignment)

```typescript
export function assignExaminerToStudySite(studyId, siteId, examinerId, certificateId?): void {
  // Check prerequisites (SI5a, SI5b, SI5c)
  
  if (certificateId) {
    // Explicit cert: validate ownership + not expired
  } else {
    // Auto-select: find latest valid cert for this examiner
    const validCerts = getCertificatesByExaminer(examinerId).filter(c => c.expiresOn >= today);
    if (validCerts.length === 0) throw ...
    resolvedCertId = validCerts[0].id;
  }

  insertSSE(studyId, siteId, examinerId, resolvedCertId);
}
```

**Why optional certificateId?** The frontend shows a picker dialog when there are multiple valid certs. If there's only one, it can be auto-selected.

---

### The Error Pattern (Consistent Across All Services)

Every business rule violation throws the same structure:

```typescript
throw new GraphQLError('Human-readable message', {
  extensions: {
    code: 'BAD_USER_INPUT',
    fieldErrors: { fieldName: 'Specific error for this field' }
  }
});
```

**Why `fieldErrors`?** The frontend can map these directly to form fields:
```
Server says: { fieldErrors: { protocolId: 'Protocol ID must be unique' } }
Frontend shows: red border + error text under the protocolId input
```

---

### Policy Flags (Configurable Rules)

```typescript
const STRICT_STUDY_COMPLETE_REQUIRES_NO_ACTIVE_SITES = true;
const STRICT_NO_SITE_UNASSIGN_WHEN_STUDY_ACTIVE = true;
```

These are boolean flags that control optional strictness. In a real production app, these might come from a config file or database. They let you toggle rules without changing logic.

---

### If You Were Building From Scratch

```
1. Start with authService.ts (login/logout — you need auth first)
2. Then studyService.ts with ONLY:
   - getStudiesPaged (list)
   - getStudyById (detail)
   - createStudy (with just uniqueness check)
3. Add updateStudy (without status transitions initially)
4. Add status transition rules one by one (test each)
5. Then siteService.ts + examinerService.ts (same patterns)
6. Then assignment functions (assignSiteToStudy, etc.)
7. Then SSE functions (most complex — build last)
8. Then certificate functions
```

**Build the simplest version first, then add rules incrementally.**

---

### Key Takeaways

1. **Services = business rules** — they decide IF an operation is allowed
2. **Repositories = data access** — they execute the operation
3. **Throw GraphQLError with fieldErrors** — consistent error format for frontend
4. **Check rules BEFORE writing** — validate everything, then call repository
5. **Side effects live in services** — auto-downgrade, auto-select certificate
6. **Status transitions are the most complex logic** — isolate them in a dedicated function
7. **Policy flags** — make strict rules configurable
8. **Return the updated entity** — after insert/update, fetch and return the fresh row

---

**Lesson 8 done.** Next is **Lesson 9: GraphQL Schema** — how you define your API contract (what clients can ask for, what data looks like). This is the "menu" of your restaurant.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 2, Lesson 9: GraphQL Schema — The API Contract

---

### The Thinking Process

> "I have my database, repositories, and services. Now I need to expose this to the frontend. How does the frontend know what it can ask for? What data looks like? What operations are available?"

Answer: **The GraphQL schema.** It's like a menu at a restaurant — it tells the client:
- What types of data exist (Study, Site, Examiner)
- What queries you can make (getStudies, getStudy)
- What mutations you can perform (createStudy, updateStudy)
- What fields each type has (title, status, startDate)

**The frontend can ONLY ask for things defined in the schema. Nothing more.**

---

### Let me show you the actual schema files:

---

---

### Understanding GraphQL Schema Language

The schema is written in **GraphQL SDL (Schema Definition Language)**. It's NOT TypeScript — it's a special language that defines your API. Let me break down the syntax:

---

#### Types — "What does the data look like?"

```graphql
type Study {
  id: ID!
  protocolId: String!
  title: String!
  status: String!
  endDate: String!
  sites: [Site!]!
  examiners: [Examiner!]!
}
```

| Syntax | Meaning |
|--------|---------|
| `String!` | Required string (never null) |
| `String` | Optional string (can be null) |
| `[Site!]!` | Required array of non-null Sites (array itself is never null, items are never null) |
| `ID!` | Required unique identifier |
| `Int!` | Required integer |

**Think of types as the "shape" of your data.** When the frontend asks for a Study, it gets exactly these fields.

---

#### Input Types — "What does the client send?"

```graphql
input CreateStudyInput {
  protocolId: String!    # Required — must provide
  title: String!         # Required
  endDate: String        # Optional (no !) — can omit
  description: String    # Optional
}
```

**`type` = what the server RETURNS. `input` = what the client SENDS.**

Notice: `CreateStudyInput` has NO `status` field. The client can't set the status on creation — the server always sets it to "Planned". This is schema-level enforcement.

---

#### Queries — "What can the client READ?"

```graphql
type Query {
  me: User                                    # Get current logged-in user
}

extend type Query {
  getStudy(id: ID!): Study                    # Get one study (can return null)
  getStudies(page: Int, pageSize: Int): StudyPage!  # Get paginated list
}
```

- `me: User` — returns User or null (no `!` means nullable)
- `getStudy(id: ID!): Study` — takes required id, returns Study or null
- `getStudies(...): StudyPage!` — always returns a StudyPage (never null)

**`extend type Query`** — this is how you split queries across multiple files. The `auth.ts` file defines the base `type Query`, and other files extend it.

---

#### Mutations — "What can the client WRITE?"

```graphql
extend type Mutation {
  createStudy(input: CreateStudyInput!): Study!
  updateStudy(id: ID!, input: UpdateStudyInput!): Study!
  assignSiteToStudy(studyId: ID!, siteId: ID!): Boolean!
}
```

- `createStudy` — takes input, returns the created Study
- `updateStudy` — takes id + input, returns the updated Study
- `assignSiteToStudy` — takes two IDs, returns true/false

---

#### Page Types — "How pagination works"

```graphql
type StudyPage {
  rows: [Study!]!
  total: Int!
}
```

Every paginated query returns `{ rows: [...], total: 123 }`. The frontend uses `total` to calculate "Page 2 of 13".

---

### How the Schema Files Are Organized

```
schema/
├── index.ts      ← Merges all schemas into one array
├── auth.ts       ← User, AuthPayload, me, login, logout, refreshSession
├── study.ts      ← Study, StudySite, StudyPage, CRUD + assignment mutations
├── site.ts       ← Site, SitePage, CRUD + assignment mutations
├── examiner.ts   ← Examiner, ExaminerCertificate, ExaminerPage, CRUD + cert mutations
├── search.ts     ← SearchResults, SearchFilters, globalSearch query
└── audit.ts      ← AuditLog, AuditLogPage, getAuditLogs query
```

**One file per domain.** Same pattern as repositories and services.

The `index.ts` just merges them:
```typescript
export const typeDefs = [authSchema, studySchema, siteSchema, examinerSchema, searchSchema, auditSchema];
```

Apollo Server accepts an array of type definitions and merges them automatically.

---

### Key Design Decisions

#### 1. Nested Types (The Power of GraphQL)

```graphql
type Study {
  sites: [Site!]!          # ← This is a RELATION, not a column
  examiners: [Examiner!]!  # ← This too
  studySites: [StudySite!]! # ← And this
}
```

These fields don't exist in the `studies` database table. They're **resolved separately** by the resolver (next lesson). The frontend can ask for them or not:

```graphql
# Simple query — just basic fields
query { getStudies { rows { id title status } } }

# Rich query — includes related data
query { getStudy(id: "1") { title sites { name } examiners { name } } }
```

**This is why GraphQL beats REST** — the client decides how much data it needs.

#### 2. StudySite Composite Type

```graphql
type StudySite {
  site: Site!
  examiners: [StudySiteExaminer!]!      # Assigned to THIS study at THIS site
  availableExaminers: [Examiner!]!      # All examiners on the site (for picker)
}
```

This is a **computed type** — it doesn't map to a single table. It combines data from `study_sites`, `study_site_examiners`, and `site_examiners`. The service builds this in `getStudySitesWithStudyExaminers()`.

#### 3. Separate Create vs Update Inputs

```graphql
input CreateStudyInput {
  protocolId: String!   # Required on create
  title: String!        # Required on create
}

input UpdateStudyInput {
  title: String         # Optional on update (only send what changed)
  status: String        # Can change status on update
}
```

- Create: all required fields are `!` (must provide)
- Update: all fields are optional (only send what you're changing)
- `protocolId` is NOT in UpdateStudyInput — you can't change it after creation

#### 4. Boolean Returns for Assignments

```graphql
assignSiteToStudy(studyId: ID!, siteId: ID!): Boolean!
```

Assignment mutations return `Boolean!` (always true if successful). If they fail, they throw a GraphQLError — the client never sees `false`, it sees an error.

#### 5. Auth Schema Defines the Base Types

```graphql
# auth.ts defines the ROOT Query and Mutation types
type Query {
  me: User
}

type Mutation {
  login(email: String!, password: String!): AuthPayload!
  logout: Boolean!
  refreshSession: Boolean!
}
```

All other files use `extend type Query` and `extend type Mutation` to add their operations. This is because GraphQL requires exactly ONE `type Query` and ONE `type Mutation` — extensions add to them.

---

### How the Frontend Uses This Schema

When the frontend writes a query:
```graphql
query GetStudy($id: ID!) {
  getStudy(id: $id) {
    id
    title
    status
    sites {
      id
      name
    }
  }
}
```

It's saying: "I want the study with this ID, but I only need id, title, status, and the names of its sites." The server returns EXACTLY that — nothing more.

---

### If You Were Building From Scratch

```
1. Start with auth.ts:
   - type User { id, email, role }
   - type Query { me: User }
   - type Mutation { login(...): AuthPayload! }

2. Then study.ts (your first entity):
   - type Study { id, title, status }  ← start simple
   - type StudyPage { rows, total }
   - extend type Query { getStudies, getStudy }
   - extend type Mutation { createStudy }

3. Add fields to Study as you build features:
   - Add sites: [Site!]! when you build the site relationship
   - Add studySites when you build SSE

4. Then site.ts, examiner.ts (same pattern)

5. Then search.ts, audit.ts (when you build those features)
```

**Start with minimal types. Add fields as features require them.**

---

### Key Takeaways

1. **Schema = API contract** — defines what clients can ask for
2. **Types = data shape** — what the server returns
3. **Inputs = request shape** — what the client sends
4. **`!` = required/non-null** — without it, the field can be null
5. **`[Type!]!` = required array of non-null items** — the standard for lists
6. **Nested types** — fields like `sites: [Site!]!` are resolved separately (not from the same table)
7. **extend type Query/Mutation** — how you split across files
8. **Page types** — `{ rows: [...], total: Int }` pattern for pagination
9. **Separate Create/Update inputs** — different required fields for each operation
10. **One file per domain** — matches your service and repository structure

---

**Lesson 9 done.** Next is **Lesson 10: GraphQL Resolvers** — the functions that IMPLEMENT the schema. When a client asks for `getStudy(id: "5")`, the resolver is the code that actually runs.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 2, Lesson 10: GraphQL Resolvers — The Request Handlers

---

### The Thinking Process

> "I have a schema that says `getStudy(id: ID!): Study` exists. But that's just a declaration — like a function signature without a body. WHO actually fetches the study? WHO calls the service?"

Answer: **Resolvers.** They're the implementation behind every schema field. When a client sends a query, Apollo Server looks at the schema, finds the matching resolver, and runs it.

```
Client sends: query { getStudy(id: "5") { title sites { name } } }

Apollo thinks:
  1. "getStudy" → run Query.getStudy resolver → returns a Study object
  2. "title" → it's a scalar field on the Study object → just return it
  3. "sites" → it's a relation field → run Study.sites resolver → returns Site[]
  4. "name" → scalar on Site → just return it
```

---

### Let me show you the actual resolver files:

---

---

### The Resolver Structure

Every resolver file exports an object with this shape:

```typescript
export const studyResolvers = {
  Query: {
    getStudies(...) { ... },    // Handles: query { getStudies { ... } }
    getStudy(...) { ... },      // Handles: query { getStudy(id: "5") { ... } }
  },
  Mutation: {
    createStudy(...) { ... },   // Handles: mutation { createStudy(input: {...}) { ... } }
    updateStudy(...) { ... },
  },
  Study: {
    sites(...) { ... },         // Handles: when someone asks for study.sites
    examiners(...) { ... },     // Handles: when someone asks for study.examiners
  },
};
```

The `index.ts` merges all resolvers into one big object that Apollo Server uses.

---

### The Resolver Function Signature

Every resolver gets 4 arguments:

```typescript
function resolver(parent, args, context, info) { ... }
```

| Argument | What it is | Example |
|----------|-----------|---------|
| `parent` | The parent object (for nested resolvers) | For `Study.sites`, parent = the Study object |
| `args` | The arguments from the query | `{ id: "5" }` or `{ input: { title: "..." } }` |
| `context` | Shared per-request data (user, req, res, loaders) | `{ user: { userId: 1, role: 'ADMIN' } }` |
| `info` | Query AST info (rarely used) | — |

---

### Breaking Down the Patterns

#### Pattern 1: Query Resolver (Read Data)

```typescript
getStudies(_: unknown, args: { page?: number; pageSize?: number }, context: GraphQLContext) {
  requireAuth(context);                    // 1. Check: is user logged in?
  const { page, pageSize } = parseOrThrow( // 2. Validate input
    pickerPaginationSchema, 
    { page: args.page ?? 1, pageSize: args.pageSize ?? 10 }
  );
  return getStudiesPaged(page, pageSize);  // 3. Call service → return data
},
```

**Every query resolver follows this 3-step pattern:**
1. Auth check
2. Validate input
3. Call service, return result

#### Pattern 2: Mutation Resolver (Write Data)

```typescript
createStudy(_: unknown, { input }: { input: CreateStudyInput }, context: GraphQLContext) {
  requireAdmin(context);                              // 1. Check: is user ADMIN?
  const validated = parseOrThrow(createStudySchema, input); // 2. Validate input
  const study = createStudy(validated as CreateStudyInput);  // 3. Call service
  logAudit(context, 'CREATE', 'Study', study.id,     // 4. Log the action
    null, JSON.stringify(study));
  return study;                                       // 5. Return created entity
},
```

**Every mutation resolver follows this 5-step pattern:**
1. Auth check (requireAdmin for writes)
2. Validate input (Zod schema)
3. Call service (business logic)
4. Log audit (before/after snapshot)
5. Return result

#### Pattern 3: Update with Before/After Snapshot

```typescript
updateStudy(_: unknown, { id, input }, context: GraphQLContext) {
  requireAdmin(context);
  parseOrThrow(idSchema, id);
  const validated = parseOrThrow(updateStudySchema, input);
  const before = getStudyById(Number(id));           // ← Snapshot BEFORE
  const study = updateStudy(Number(id), validated);  // ← Do the update
  logAudit(context, 'UPDATE', 'Study', study.id, 
    JSON.stringify(before),                          // ← Before JSON
    JSON.stringify(study));                           // ← After JSON
  return study;
},
```

This captures what the entity looked like BEFORE and AFTER the change — essential for audit trails.

#### Pattern 4: Type Resolvers (Nested Fields)

```typescript
Study: {
  sites(parent: StudyRow, _: unknown, context: GraphQLContext) {
    return context.loaders.sitesByStudyId.load(parent.id);
  },
  examiners(parent: StudyRow, _: unknown, context: GraphQLContext) {
    return context.loaders.examinersByStudyId.load(parent.id);
  },
  studySites(parent: StudyRow) {
    return getStudySitesWithStudyExaminers(parent.id);
  },
},
```

**How this works:**

When the client asks for:
```graphql
query {
  getStudies {
    rows {
      id
      title
      sites { name }    ← triggers Study.sites resolver
    }
  }
}
```

1. `Query.getStudies` runs → returns array of `StudyRow` objects (just DB columns: id, title, status...)
2. For each study, Apollo sees the client wants `sites`
3. `sites` isn't a column on StudyRow — so Apollo calls `Study.sites(parent)` resolver
4. That resolver uses `parent.id` to load the related sites

**If the client DOESN'T ask for `sites`, the resolver NEVER runs.** This is GraphQL's efficiency — only resolve what's requested.

---

### The Helper Functions (helpers.ts)

```typescript
export function requireAuth(context: GraphQLContext): void {
  if (!context.user) {
    throw new GraphQLError('Unauthorized', { extensions: { code: 'UNAUTHENTICATED' } });
  }
}

export function requireAdmin(context: GraphQLContext): void {
  requireAuth(context);  // First check: logged in?
  if (context.user!.role !== 'ADMIN') {
    throw new GraphQLError('Forbidden', { extensions: { code: 'FORBIDDEN' } });
  }
}

export function logAudit(context, action, entityType, entityId, beforeJson, afterJson): void {
  const user = context.user!;
  insertAuditLog(user.userId, user.email, action, entityType, entityId, beforeJson, afterJson);
}
```

**Three helpers used by EVERY resolver:**
- `requireAuth` — throws UNAUTHENTICATED if no user in context
- `requireAdmin` — throws FORBIDDEN if user isn't ADMIN
- `logAudit` — records the action (gets actor info from context)

---

### The Auth Resolver (Login/Logout/Refresh)

```typescript
login(_: unknown, args, context: GraphQLContext) {
  const { email, password } = parseOrThrow(loginSchema, args);
  const result = loginUser(email, password);      // Service validates credentials
  setAccessCookie(context.res, result.accessToken);  // Set JWT cookie
  setRefreshCookie(context.res, result.refreshToken); // Set refresh cookie
  return { user: result.user };
},

logout(_: unknown, __: unknown, context: GraphQLContext) {
  requireAuth(context);
  const rawRefresh = context.req.cookies?.[REFRESH_COOKIE];
  if (rawRefresh) revokeSession(rawRefresh);  // Invalidate refresh token in DB
  clearAuthCookies(context.res);               // Clear both cookies
  return true;
},

refreshSession(_: unknown, __: unknown, context: GraphQLContext) {
  const rawRefresh = context.req.cookies?.[REFRESH_COOKIE];
  if (!rawRefresh) { clearAuthCookies(context.res); return false; }
  const result = refreshSession(rawRefresh);   // Rotate token
  if (!result) { clearAuthCookies(context.res); return false; }
  setAccessCookie(context.res, result.accessToken);
  setRefreshCookie(context.res, result.refreshToken);
  return true;
},
```

**Key insight:** The resolver has access to `context.res` (Express response object) — that's how it sets cookies. Cookies are HTTP-level, not GraphQL-level.

---

### How Resolvers Connect to Everything

```
Client sends GraphQL query
  → Apollo Server parses it
  → Finds matching resolver
  → Resolver calls:
      1. helpers.ts (requireAuth/requireAdmin)
      2. validation/ (parseOrThrow with Zod schema)
      3. services/ (business logic)
      4. helpers.ts (logAudit)
  → Returns data to Apollo
  → Apollo formats response
  → Sends JSON back to client
```

---

### The Resolver Index (Merging Everything)

```typescript
export const resolvers = {
  Query: {
    ...authResolvers.Query,      // me
    ...studyResolvers.Query,     // getStudies, getStudy
    ...siteResolvers.Query,      // getSites, getSite
    ...examinerResolvers.Query,  // getExaminers, getExaminer
    ...searchResolvers.Query,    // globalSearch
    ...auditResolvers.Query,     // getAuditLogs
  },
  Mutation: {
    ...authResolvers.Mutation,   // login, logout, refreshSession
    ...studyResolvers.Mutation,  // createStudy, updateStudy, assign/unassign
    ...siteResolvers.Mutation,   // createSite, updateSite, assign/unassign
    ...examinerResolvers.Mutation, // createExaminer, updateExaminer, certificates
  },
  Study: studyResolvers.Study,     // sites, examiners, studySites
  Site: siteResolvers.Site,        // studies, examiners
  Examiner: examinerResolvers.Examiner, // studies, sites, certificates
};
```

Apollo needs ONE resolvers object. The index merges all domain resolvers into it.

---

### If You Were Building From Scratch

```
1. Start with helpers.ts:
   - requireAuth (you need this immediately)
   - requireAdmin
   - logAudit (add later when you build audit)

2. Then auth.ts:
   - login (first thing users do)
   - me (frontend needs to check "am I logged in?")
   - logout

3. Then study.ts with ONLY:
   - Query.getStudies (list page)
   - Query.getStudy (detail page)
   - Mutation.createStudy

4. Add Study type resolvers when you add relations:
   - Study.sites (when you build site assignment)

5. Then site.ts, examiner.ts (same pattern)

6. Then assignment mutations (assignSiteToStudy, etc.)

7. Then audit.ts, search.ts (last features)
```

---

### Key Takeaways

1. **Resolvers implement the schema** — one function per query/mutation/type field
2. **4 arguments:** parent, args, context, info
3. **Query pattern:** auth → validate → call service → return
4. **Mutation pattern:** auth → validate → call service → audit → return
5. **Type resolvers** handle nested fields (sites, examiners) — only run when requested
6. **Context carries user info** — set in app.ts, used in every resolver
7. **Helpers centralize auth + audit** — DRY, consistent across all resolvers
8. **Resolvers are THIN** — they don't contain business logic, they delegate to services
9. **DataLoaders** used in type resolvers to prevent N+1 (covered in Lesson 15)
10. **Before/after snapshots** for UPDATE audit logs

---

**Lesson 10 done.** Next is **Lesson 11: Authentication** — the complete JWT + cookie + refresh token system. How login works, how tokens are created, verified, and rotated.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 2, Lesson 11: Authentication — JWT + Cookies + Refresh Tokens

---

### The Thinking Process

> "I need to know WHO is making each request. But HTTP is stateless — each request is independent. How do I remember that 'this user logged in 5 minutes ago'?"

Answer: **Tokens.** After login, the server gives the client a token (proof of identity). The client sends it with every request. The server verifies it.

**But where to store the token?** Two options:
- localStorage → JavaScript can read it → XSS attack can steal it ❌
- HttpOnly cookie → JavaScript CANNOT read it → browser sends it automatically ✅

**And what about token expiry?** Two strategies:
- Long-lived token (30 days) → if stolen, attacker has access for 30 days ❌
- Short-lived access token (15 min) + long-lived refresh token (7 days) → if access token is stolen, it expires quickly ✅

---

### The Dual-Token Strategy

```
LOGIN:
  Server creates:
    1. Access token (JWT, 15 min) → stored in auth_token cookie
    2. Refresh token (random string, 7 days) → stored in refresh_token cookie + hashed in DB

EVERY REQUEST:
  Browser automatically sends auth_token cookie
  Server verifies JWT → knows who the user is

AFTER 15 MINUTES (access token expires):
  Server rejects request with UNAUTHENTICATED
  Frontend automatically calls refreshSession mutation
  Server checks refresh_token cookie → issues NEW access token + NEW refresh token
  Original request is retried → user never notices

AFTER 7 DAYS (refresh token expires):
  refreshSession fails → user is redirected to login page
```

---

### Let me show you the actual auth files:

---

---

### The Complete Auth Flow — Step by Step

Let me trace the ENTIRE login → use → refresh → logout cycle:

---

#### Step 1: LOGIN

```
User types email + password → clicks Login
  → Frontend sends: mutation { login(email: "admin@test.com", password: "password123") }
  → Resolver: parseOrThrow(loginSchema, args) → validates email format + password length
  → Service: loginUser(email, password)
```

Inside `loginUser`:
```typescript
// 1. Find user in DB
const user = findUserByEmail(email);

// 2. Verify password (bcrypt compare)
if (!user || !verifyPassword(password, user.password)) {
  throw new GraphQLError('Invalid credentials', { code: 'UNAUTHENTICATED' });
}

// 3. Create access token (JWT with user info, expires in 15 min)
const accessToken = signToken({ userId: user.id, role: user.role, email: user.email });

// 4. Create refresh token (random 96-char hex string)
const rawToken = generateRefreshToken();  // crypto.randomBytes(48).toString('hex')
const tokenHash = hashToken(rawToken);     // SHA-256 hash (stored in DB)
insertRefreshToken(userId, tokenHash, expiresAt);  // Save hash to DB

// 5. Return both tokens + user info
return { accessToken, refreshToken: rawToken, user: {...} };
```

Back in the resolver:
```typescript
setAccessCookie(context.res, result.accessToken);   // Set auth_token cookie (15 min)
setRefreshCookie(context.res, result.refreshToken); // Set refresh_token cookie (7 days)
return { user: result.user };
```

**After login, the browser has TWO HttpOnly cookies. JavaScript can't read them. The browser sends them automatically.**

---

#### Step 2: EVERY SUBSEQUENT REQUEST

```
Browser sends request to /graphql
  → Cookie header automatically includes: auth_token=eyJhbG...; refresh_token=a3f7b2...
  → app.ts context function:
      const token = req.cookies?.auth_token;
      const user = token ? verifyToken(token) : null;
      return { user, req, res, ... };
```

Inside `verifyToken`:
```typescript
export function verifyToken(token: string): JwtPayload | null {
  try {
    return jwt.verify(token, getSecret()) as JwtPayload;
    // Returns: { userId: 1, role: 'ADMIN', email: 'admin@test.com' }
  } catch {
    return null;  // Token expired or invalid
  }
}
```

If valid → `context.user` has the user info → resolvers can check auth.
If expired → `context.user` is null → resolvers throw UNAUTHENTICATED.

---

#### Step 3: TOKEN REFRESH (After 15 Minutes)

```
Access token expires → server returns UNAUTHENTICATED error
  → Frontend Apollo errorLink catches it
  → Sends: mutation { refreshSession }
  → Resolver reads refresh_token cookie
  → Service: refreshSession(rawRefreshToken)
```

Inside `refreshSession`:
```typescript
// 1. Hash the incoming token to look it up in DB
const incomingHash = hashToken(rawRefreshToken);
const row = findRefreshToken(incomingHash);

// 2. Validate: exists? not revoked? not expired?
if (!row) return null;
if (row.revoked_at !== null) return null;
if (new Date(row.expires_at) <= new Date()) return null;

// 3. ROTATION: create new refresh token, revoke old one
const { rawToken: newRaw, tokenHash: newHash } = createRefreshTokenRecord(row.user_id);
revokeRefreshToken(incomingHash, newHash);  // Old token marked as revoked, linked to new

// 4. Issue new access token
const accessToken = signToken({ userId: user.id, role: user.role, email: user.email });

return { accessToken, refreshToken: newRaw };
```

**Token rotation explained:**
- Old refresh token is REVOKED (can never be used again)
- New refresh token is issued
- `replaced_by_token_hash` links old → new (audit trail)
- If an attacker steals the old token and tries to use it → it's already revoked → attack detected

---

#### Step 4: LOGOUT

```
User clicks Logout
  → Frontend sends: mutation { logout }
  → Resolver:
      const rawRefresh = context.req.cookies?.refresh_token;
      revokeSession(rawRefresh);     // Revoke refresh token in DB
      clearAuthCookies(context.res); // Clear both cookies
      return true;
```

After logout:
- Cookies are gone from the browser
- Refresh token is revoked in DB (even if someone copied it, it won't work)

---

### Why Hash the Refresh Token?

```typescript
// What's stored in the cookie (sent to browser):
"a3f7b2c1d4e5f6a7b8c9d0e1f2a3b4c5d6e7f8a9b0c1d2e3f4a5b6c7d8e9f0a1b2c3d4e5f6a7b8c9d0e1f2a3"

// What's stored in the database:
"7f83b1657ff1fc53b92dc18148a1d65dfc2d4b1fa3d677284addd200126d9069"  (SHA-256 hash)
```

**Why?** If someone gets access to your database (SQL injection, backup leak), they see HASHES, not actual tokens. They can't use the hashes to impersonate users. Same principle as password hashing.

---

### The JWT Payload

```typescript
export interface JwtPayload {
  userId: number;
  role: 'ADMIN' | 'VIEWER';
  email: string;
}
```

The JWT contains just enough info to:
- Identify the user (`userId`)
- Check their role (`role`) — without a DB query
- Log their actions (`email`) — without a DB query

**Why include role in JWT?** So every request can check "is this user an admin?" without hitting the database. The trade-off: if you change a user's role, their old JWT still has the old role until it expires (15 min max).

---

### The Password Utilities

```typescript
export function hashPassword(plain: string): string {
  return bcrypt.hashSync(plain, 10);  // Cost factor 10 = ~100ms to hash
}

export function verifyPassword(plain: string, hashed: string): boolean {
  return bcrypt.compareSync(plain, hashed);
}
```

- **Cost factor 10** = each hash takes ~100ms. This is intentional — it makes brute-force attacks slow
- `hashSync` is synchronous (fine for SQLite which is also sync)
- You NEVER store plain passwords. You NEVER decrypt hashes. You only COMPARE.

---

### Security Properties of This Design

| Threat | Protection |
|--------|-----------|
| XSS steals token | HttpOnly cookies — JS can't read them |
| Token stolen from network | HTTPS in production (secure: true) |
| Long-term token theft | Access token expires in 15 min |
| Refresh token stolen | Rotation — old token is immediately revoked |
| Replay attack (reuse old refresh) | Revoked tokens are rejected |
| Database breach | Refresh tokens are SHA-256 hashed |
| Brute-force login | Rate limiting (20 attempts/15 min) |
| CSRF attack | sameSite: 'lax' on cookies |

---

### If You Were Building From Scratch

```
1. Start with password.ts (hashPassword + verifyPassword)
   - You need this to seed users

2. Then jwt.ts (signToken + verifyToken)
   - You need this for the login flow

3. Then authService.ts with ONLY loginUser
   - Just access token, no refresh yet
   - Get login working end-to-end first

4. Then auth resolver (login + me + logout)
   - Set cookie on login, clear on logout

5. Then add context function in app.ts
   - Read cookie → verify → set context.user

6. Then add requireAuth/requireAdmin helpers
   - Now your resolvers are protected

7. LATER: add refresh tokens
   - token.ts (generateRefreshToken + hashToken)
   - refreshTokenRepository.ts
   - refreshSession in authService
   - refreshSession resolver
```

**Refresh tokens are an ADVANCED feature. Get basic JWT auth working first, then add refresh.**

---

### Key Takeaways

1. **Dual-token strategy** — short access (15m) + long refresh (7d)
2. **HttpOnly cookies** — browser manages them, JS can't touch them
3. **JWT contains userId + role + email** — no DB lookup needed per request
4. **Refresh token rotation** — each use revokes old, issues new
5. **SHA-256 hashing** — raw tokens never stored in DB
6. **Context function** — runs per-request, extracts user from cookie
7. **requireAuth/requireAdmin** — first line of every protected resolver
8. **Fail gracefully** — verifyToken returns null (not throws) on invalid tokens
9. **Rate limiting on login** — prevents brute-force
10. **Logout revokes refresh token** — even if cookie is somehow preserved, it won't work

---

**Lesson 11 done.** Next is **Lesson 12: Authorization** — how role-based access control works in practice, how ADMIN vs VIEWER is enforced across the entire app.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 2, Lesson 12: Authorization — Role-Based Access Control

---

### The Thinking Process

> "Authentication tells me WHO the user is. But I also need to control WHAT they can do. An ADMIN can create studies. A VIEWER can only read. How do I enforce this consistently across 20+ resolvers?"

Answer: **Two guard functions + consistent placement.** Every resolver starts with one of these:

```
requireAuth(context)  → Any logged-in user (ADMIN or VIEWER) can proceed
requireAdmin(context) → Only ADMIN can proceed (calls requireAuth first)
```

---

### The Authorization Matrix

| Operation | Guard | Who can do it |
|-----------|-------|---------------|
| `me` | requireAuth | Any logged-in user |
| `getStudies` | requireAuth | Any logged-in user |
| `getStudy` | requireAuth | Any logged-in user |
| `getSites` | requireAuth | Any logged-in user |
| `getExaminers` | requireAuth | Any logged-in user |
| `globalSearch` | requireAuth | Any logged-in user |
| `createStudy` | requireAdmin | ADMIN only |
| `updateStudy` | requireAdmin | ADMIN only |
| `assignSiteToStudy` | requireAdmin | ADMIN only |
| `unassignSiteFromStudy` | requireAdmin | ADMIN only |
| `createSite` | requireAdmin | ADMIN only |
| `updateSite` | requireAdmin | ADMIN only |
| `assignExaminerToSite` | requireAdmin | ADMIN only |
| `createExaminer` | requireAdmin | ADMIN only |
| `updateExaminer` | requireAdmin | ADMIN only |
| `addExaminerCertificate` | requireAdmin | ADMIN only |
| `getAuditLogs` | requireAdmin | ADMIN only |
| `login` | none | Public (no auth needed) |
| `logout` | requireAuth | Any logged-in user |
| `refreshSession` | none | Public (cookie is the credential) |

**Simple rule:** Reads = requireAuth. Writes = requireAdmin. Auth operations = special cases.

---

### How It Works (Already Seen, Now Deeply Understood)

```typescript
// helpers.ts
export function requireAuth(context: GraphQLContext): void {
  if (!context.user) {
    throw new GraphQLError('Unauthorized', { extensions: { code: 'UNAUTHENTICATED' } });
  }
}

export function requireAdmin(context: GraphQLContext): void {
  requireAuth(context);  // Step 1: Are you logged in at all?
  if (context.user!.role !== 'ADMIN') {
    throw new GraphQLError('Forbidden: admin access required', { extensions: { code: 'FORBIDDEN' } });
  }
}
```

**The flow:**

```
Request arrives → context function reads cookie → verifyToken
  → If no cookie or invalid token: context.user = null
  → If valid token: context.user = { userId: 1, role: 'ADMIN', email: 'admin@test.com' }

Resolver runs → first line: requireAdmin(context)
  → requireAuth: context.user is null? → throw UNAUTHENTICATED (401)
  → requireAdmin: context.user.role !== 'ADMIN'? → throw FORBIDDEN (403)
  → Both pass? → continue with the resolver logic
```

---

### The Two Error Codes (Important Distinction)

| Code | HTTP Equivalent | Meaning | Frontend Behavior |
|------|----------------|---------|-------------------|
| `UNAUTHENTICATED` | 401 | "I don't know who you are" | Redirect to /login |
| `FORBIDDEN` | 403 | "I know who you are, but you can't do this" | Show error toast |

**Why separate?**
- UNAUTHENTICATED → token expired or missing → try refresh, then redirect to login
- FORBIDDEN → user is logged in but wrong role → show "access denied" message, stay on page

---

### Where Authorization Lives (Defense in Depth)

Authorization is enforced at MULTIPLE levels:

```
Level 1: Frontend routing (UI-level, easily bypassed)
  → AdminRoute component blocks non-admin from /admin/* pages
  → But this is just UX — a developer could call the API directly

Level 2: Resolver guards (API-level, authoritative)
  → requireAdmin() in every mutation resolver
  → This is the REAL enforcement — can't be bypassed

Level 3: Frontend hides UI elements (UX-level)
  → Viewer pages don't show "Create" buttons
  → But even if they did, the API would reject the request
```

**The backend is ALWAYS the authority.** Frontend restrictions are just UX convenience.

---

### How Role Gets Into the JWT

During login:
```typescript
// authService.ts → loginUser
const accessToken = signToken({ userId: user.id, role: user.role, email: user.email });
```

The JWT payload contains:
```json
{
  "userId": 1,
  "role": "ADMIN",
  "email": "admin@test.com",
  "iat": 1700000000,
  "exp": 1700000900
}
```

On every request, `verifyToken` decodes this → `context.user.role` is available → no DB query needed.

---

### How the Frontend Knows the Role

The frontend uses the `me` query:
```graphql
query Me {
  me {
    id
    email
    role    ← This tells the frontend what to show
  }
}
```

The `AuthContext` stores this:
```typescript
// Frontend: contexts/AuthContext.tsx
const { data } = useQuery(ME_QUERY);
const role = data?.me?.role;  // 'ADMIN' or 'VIEWER'
const isLoggedIn = !!data?.me;
```

Then routing uses it:
```typescript
// AdminRoute component
if (role !== 'ADMIN') return <Navigate to="/viewer/dashboard" />;

// ProtectedRoute component
if (!isLoggedIn) return <Navigate to="/login" />;
```

---

### The Complete Authorization Chain (End to End)

```
1. User logs in as ADMIN
   → JWT created with role: 'ADMIN'
   → Cookie set

2. User navigates to /admin/studies
   → AdminRoute checks: role === 'ADMIN'? ✅ → render page

3. Page loads → sends query { getStudies { ... } }
   → Resolver: requireAuth(context) → context.user exists? ✅
   → Returns data

4. User clicks "Create Study" → fills form → submits
   → Sends mutation { createStudy(input: {...}) }
   → Resolver: requireAdmin(context) → role === 'ADMIN'? ✅
   → Study created

5. Now imagine a VIEWER tries to call createStudy directly (via API tool):
   → Resolver: requireAdmin(context)
   → requireAuth: context.user exists? ✅ (they're logged in)
   → role === 'ADMIN'? ❌ (they're VIEWER)
   → throw FORBIDDEN
   → Client receives error, study NOT created
```

---

### Why Not More Granular Permissions?

This app has only 2 roles. In a real enterprise app, you might have:
- `ADMIN` — full access
- `EDITOR` — can create/edit but not delete
- `VIEWER` — read only
- `AUDITOR` — can see audit logs but not edit

The pattern would be the same — just more guard functions:
```typescript
function requireEditor(context) { ... }
function requireAuditor(context) { ... }
```

Or a generic:
```typescript
function requireRole(context, ...allowedRoles: string[]) {
  requireAuth(context);
  if (!allowedRoles.includes(context.user!.role)) throw FORBIDDEN;
}
```

This project keeps it simple with 2 roles because it's a demo. The pattern scales to any number of roles.

---

### If You Were Building From Scratch

```
1. Start with just requireAuth (any logged-in user)
   - Get login + protected queries working first

2. Add requireAdmin when you build mutations
   - Now you have read (any user) vs write (admin only)

3. Add frontend AdminRoute/ProtectedRoute
   - Route-level protection for UX

4. Add role to AuthContext
   - So components can conditionally render (show/hide buttons)

5. LATER: if you need more roles, extend the pattern
```

---

### Key Takeaways

1. **Two guards cover everything** — requireAuth (reads) + requireAdmin (writes)
2. **First line of every resolver** — auth check before ANY logic runs
3. **UNAUTHENTICATED vs FORBIDDEN** — different meanings, different frontend behavior
4. **Backend is authoritative** — frontend restrictions are UX only
5. **Role in JWT** — no DB query needed per request for auth checks
6. **Defense in depth** — routing + resolver + UI all enforce access, but resolver is the truth
7. **Pattern scales** — add more roles by adding more guard functions
8. **Public operations** — login and refreshSession don't need auth (they CREATE auth)

---

**Lesson 12 done.** Next is **Lesson 13: Validation** — how Zod schemas validate every input on both frontend and backend, and how validation errors flow back to form fields.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 2, Lesson 13: Validation — Zod Schemas + Error Flow

---

### The Thinking Process

> "Users will send garbage data. Empty strings, negative numbers, SQL injection attempts, dates in the past. How do I reject bad input BEFORE it reaches my business logic? And how do I tell the user EXACTLY which field is wrong?"

Answer: **Zod schemas.** Define the shape of valid input once, validate automatically, and return field-level errors.

**Why validate on BOTH frontend and backend?**
- Frontend validation = instant feedback (no network round-trip)
- Backend validation = security (frontend can be bypassed)
- Backend is AUTHORITATIVE. Frontend is UX convenience.

---

### Let me show you the actual validation files:

---

---

### The Core Concept: parseOrThrow

This is the single most important function in the validation layer:

```typescript
export function parseOrThrow<T>(schema, value: unknown): T {
  const result = schema.safeParse(value);
  if (!result.success) {
    throwBadUserInput(zodErrorToFieldErrors(result.error));
  }
  return result.data;  // ← Validated + transformed data
}
```

**What it does:**
1. Takes a Zod schema and raw input
2. Validates the input against the schema
3. If invalid → throws GraphQLError with field-level errors
4. If valid → returns the cleaned/transformed data

**Used in EVERY mutation resolver:**
```typescript
createStudy(_: unknown, { input }, context) {
  requireAdmin(context);
  const validated = parseOrThrow(createStudySchema, input);  // ← HERE
  const study = createStudy(validated);
  ...
}
```

---

### How Zod Schemas Work (The Building Blocks)

#### Basic field validation:
```typescript
z.string()                          // Must be a string
z.string().min(1, 'Required')       // Non-empty string
z.string().max(50, 'Too long')      // Max 50 chars
z.string().email('Invalid email')   // Must be valid email format
z.string().regex(/^\d{4}-\d{2}-\d{2}$/, 'Must be YYYY-MM-DD')  // Pattern match
```

#### Enums (restricted values):
```typescript
z.enum(['Phase I', 'Phase II', 'Phase III', 'Phase IV'])
// Only these exact values are accepted. Anything else → error.
```

#### Optional fields:
```typescript
z.string().min(1).optional()
// Can be undefined (not provided) — but if provided, must be non-empty string
```

#### Transform (normalize input):
```typescript
z.string().transform((v) => v.trim().toUpperCase())
// Input: "  abc-123  " → Output: "ABC-123"
// Happens AFTER validation passes
```

#### Object schemas:
```typescript
z.object({
  protocolId: z.string().min(1).transform(v => v.trim().toUpperCase()),
  title: z.string().min(1).max(200),
  phase: z.enum(STUDY_PHASES),
  startDate: z.string().regex(DATE_REGEX),
  endDate: z.string().regex(DATE_REGEX).optional(),
})
```

#### Cross-field validation (superRefine):
```typescript
.superRefine((data, ctx) => {
  if (data.startDate && data.endDate && data.startDate > data.endDate) {
    ctx.addIssue({ 
      code: z.ZodIssueCode.custom, 
      path: ['endDate'],  // ← Which field gets the error
      message: 'End date must be on or after start date' 
    });
  }
})
```

This validates relationships BETWEEN fields — something single-field validation can't do.

---

### The Error Flow (Backend → Frontend)

**Step 1: Zod validation fails**
```typescript
// User sends: { protocolId: "", title: "", phase: "Invalid" }
const result = createStudySchema.safeParse(input);
// result.success = false
// result.error.issues = [
//   { path: ['protocolId'], message: 'Protocol ID is required' },
//   { path: ['title'], message: 'Study name is required' },
//   { path: ['phase'], message: 'Invalid phase' },
// ]
```

**Step 2: Convert to fieldErrors map**
```typescript
zodErrorToFieldErrors(result.error)
// Returns: {
//   protocolId: 'Protocol ID is required',
//   title: 'Study name is required',
//   phase: 'Invalid phase',
// }
```

**Step 3: Throw GraphQLError**
```typescript
throw new GraphQLError('Validation error', {
  extensions: {
    code: 'BAD_USER_INPUT',
    fieldErrors: {
      protocolId: 'Protocol ID is required',
      title: 'Study name is required',
      phase: 'Invalid phase',
    }
  }
});
```

**Step 4: Frontend receives the error**
```typescript
// In the CRUD dialog's onSubmit:
catch (err) {
  const { code, fieldErrors } = parseGqlError(err);
  if (code === 'BAD_USER_INPUT') {
    // Map each error to its form field
    Object.entries(fieldErrors).forEach(([field, message]) => {
      setError(field, { message });  // react-hook-form shows it under the input
    });
  }
}
```

**Step 5: User sees red error under each invalid field**
```
┌─────────────────────────────────┐
│ Protocol ID: [              ]   │
│ ⚠️ Protocol ID is required      │
│                                 │
│ Title: [                    ]   │
│ ⚠️ Study name is required       │
│                                 │
│ Phase: [ Select... ▼ ]          │
│ ⚠️ Invalid phase                │
└─────────────────────────────────┘
```

---

### Create vs Update Schema Design

**Create schema — all required fields are mandatory:**
```typescript
export const createStudySchema = z.object({
  protocolId: z.string().min(1, 'Required'),  // MUST provide
  title: z.string().min(1, 'Required'),       // MUST provide
  phase: z.enum(STUDY_PHASES),                // MUST provide
  startDate: z.string().regex(DATE_REGEX),    // MUST provide
  endDate: z.string().regex(DATE_REGEX).optional(),  // CAN omit
});
```

**Update schema — all fields are optional:**
```typescript
export const updateStudySchema = z.object({
  title: z.string().min(1).max(200).optional(),     // Only send if changing
  phase: z.enum(STUDY_PHASES).optional(),           // Only send if changing
  status: z.enum(STUDY_STATUSES).optional(),        // Only send if changing
  startDate: z.string().regex(DATE_REGEX).optional(),
});
```

**Why?** On update, you only send the fields that changed. If you send `{ title: "New Title" }`, only title is validated and updated. Other fields stay as they are.

---

### Special Schemas

#### ID validation:
```typescript
export const idSchema = z.string().regex(/^\d+$/, 'ID must be a positive integer');
```
GraphQL sends IDs as strings. This ensures they're numeric before `Number(id)` conversion.

#### Pagination validation:
```typescript
export const paginationSchema = z.object({
  page: z.number().int().min(1).default(1),
  pageSize: z.number().int().min(1).max(100).default(10),
});
```
- `page` must be ≥ 1 (no page 0 or negative)
- `pageSize` capped at 100 (prevents someone requesting 1 million rows)
- `.default(1)` — if not provided, use 1

#### Search validation:
```typescript
export const searchSchema = z.object({
  keyword: z.string().min(2, 'Keyword must be at least 2 characters').max(200),
  filters: z.object({ ... }).optional(),
});
```
Minimum 2 characters prevents expensive single-character searches.

---

### The Transform Pattern (Data Normalization)

```typescript
protocolId: z.string().min(1).transform((v) => v.trim().toUpperCase()),
siteCode: z.string().min(1).transform((v) => v.trim().toUpperCase()),
```

**Why transform?**
- User types: `"  abc-123  "` → stored as: `"ABC-123"`
- Prevents duplicates: `"ABC"` and `"abc"` and `" ABC "` all become `"ABC"`
- Consistent data in the database

**Important:** Transform runs AFTER validation. If `min(1)` fails, transform never runs.

---

### Frontend Validation (Mirror of Backend)

Now let me show you how the frontend uses Zod too:

---

---

### Frontend vs Backend Schemas — The Differences

| Aspect | Backend | Frontend |
|--------|---------|----------|
| Purpose | Security (authoritative) | UX (instant feedback) |
| Date check | UTC (`todayUTC()`) | Local time (`todayLocal()`) — UX hint only |
| Transform | `.transform(v => v.trim().toUpperCase())` | Same on protocolId |
| Cross-field | `.superRefine()` | `.refine()` (simpler syntax) |
| Status field | Absent in create schema | Absent in create schema |
| Error handling | Throws GraphQLError | react-hook-form shows inline |

**Key insight:** Frontend schemas are SIMPLER. They don't need to be as strict because the backend will catch anything the frontend misses.

---

### How Frontend Validation Integrates with react-hook-form

```typescript
import { useForm } from 'react-hook-form';
import { zodResolver } from '@hookform/resolvers/zod';
import { createStudySchema, CreateStudyFormValues } from '../validation/studySchemas';

const { register, handleSubmit, formState: { errors } } = useForm<CreateStudyFormValues>({
  resolver: zodResolver(createStudySchema),  // ← Zod validates on submit
});
```

When user clicks Submit:
1. react-hook-form calls `zodResolver(createStudySchema)` with form values
2. If Zod fails → errors appear under fields instantly (no network request)
3. If Zod passes → `onSubmit` function runs → sends mutation to backend
4. If backend ALSO rejects → `setError` maps server errors to fields

**Two layers of validation, same user experience:**
```
User submits form
  → Frontend Zod: "Protocol ID is required" → shows instantly
  → User fixes it, submits again
  → Frontend Zod: passes ✅
  → Backend Zod: passes ✅
  → Backend Service: "Protocol ID already exists" → shows via setError
```

---

### The Complete Validation Chain

```
User types in form
  ↓
Frontend Zod schema (zodResolver) — instant, client-side
  ↓ (if passes)
GraphQL mutation sent to backend
  ↓
Backend Zod schema (parseOrThrow) — authoritative validation
  ↓ (if passes)
Service business rules — domain logic (dates, uniqueness, prerequisites)
  ↓ (if passes)
Repository — data saved to database
```

Each layer catches different things:
- **Frontend Zod:** format errors (empty fields, invalid email, date format)
- **Backend Zod:** same + transform/normalize
- **Service:** business rules (uniqueness, date logic, status transitions)

---

### If You Were Building From Scratch

```
1. Start with helpers.ts (parseOrThrow + zodErrorToFieldErrors)
   - You need this before any validation works

2. Then authSchemas.ts (loginSchema)
   - Validate email + password on login

3. Then studySchemas.ts (createStudySchema)
   - Your first entity's validation

4. Then assignmentSchemas.ts (idSchema, paginationSchema)
   - Used by all resolvers for ID and pagination validation

5. Then siteSchemas.ts, examinerSchemas.ts
   - Same patterns as study

6. Frontend schemas LAST
   - Mirror the backend schemas but simpler
   - Add only after forms are built
```

---

### Key Takeaways

1. **parseOrThrow** — single function used in every resolver, converts Zod errors to GraphQL errors
2. **fieldErrors map** — `{ fieldName: 'error message' }` flows from backend to frontend form fields
3. **Create schemas = required fields, Update schemas = optional fields**
4. **Transform** — normalize data (trim, uppercase) during validation
5. **superRefine/refine** — cross-field validation (endDate ≥ startDate)
6. **Backend is authoritative** — frontend validation is UX only
7. **Pagination capped** — pageSize max 100 prevents abuse
8. **ID validation** — ensures string IDs are numeric before conversion
9. **Two-layer validation** — frontend Zod (instant) + backend Zod (secure)
10. **Same library (Zod) on both sides** — consistent patterns, easy to maintain

---

**Lesson 13 done.** Next is **Lesson 14: Audit Logging** — how every admin action is tracked with before/after snapshots, creating a complete change history.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 2, Lesson 14: Audit Logging — Tracking Every Change

---

### The Thinking Process

> "My admin can create, update, assign, and unassign things. But what if something goes wrong? What if someone asks 'who changed this study's status last week?' I need a complete history of every action."

Answer: **Audit logging.** Every mutation records WHO did WHAT to WHICH entity, with BEFORE and AFTER snapshots. It's like a security camera for your data.

---

### The Audit Log Table (What Gets Stored)

```sql
audit_logs:
  id          — auto-increment
  actorUserId — WHO did it (user ID)
  actorEmail  — WHO did it (email, for display)
  action      — WHAT they did: CREATE, UPDATE, ASSIGN, UNASSIGN
  entityType  — WHAT type of thing: Study, Site, Examiner, StudySite, SiteExaminer, etc.
  entityId    — WHICH specific entity (ID)
  beforeJson  — What it looked like BEFORE (null for CREATE/ASSIGN)
  afterJson   — What it looks like AFTER (null for UNASSIGN)
  createdAt   — WHEN it happened
```

---

### The Four Actions

| Action | beforeJson | afterJson | Example |
|--------|-----------|-----------|---------|
| CREATE | null | full entity JSON | Created a new study |
| UPDATE | entity before change | entity after change | Changed status from Planned to Active |
| ASSIGN | null | relationship JSON | Assigned site 3 to study 1 |
| UNASSIGN | relationship JSON | null | Removed site 3 from study 1 |

---

### How It Works in Practice

You already saw `logAudit` in the resolvers. Let me trace a complete example:

**Example: Admin updates a study's status from Planned to Active**

```typescript
// In study resolver:
updateStudy(_: unknown, { id, input }, context: GraphQLContext) {
  requireAdmin(context);
  parseOrThrow(idSchema, id);
  const validated = parseOrThrow(updateStudySchema, input);
  
  const before = getStudyById(Number(id));           // ← Snapshot BEFORE
  const study = updateStudy(Number(id), validated);  // ← Do the update
  
  logAudit(context, 'UPDATE', 'Study', study.id,
    JSON.stringify(before),    // ← Before: {"id":1,"status":"Planned","title":"..."}
    JSON.stringify(study)      // ← After:  {"id":1,"status":"Active","title":"..."}
  );
  return study;
}
```

**What gets stored in audit_logs:**
```json
{
  "actorUserId": 1,
  "actorEmail": "admin@test.com",
  "action": "UPDATE",
  "entityType": "Study",
  "entityId": 1,
  "beforeJson": "{\"id\":1,\"status\":\"Planned\",\"title\":\"COVID Trial\",\"startDate\":\"2024-01-01\",...}",
  "afterJson": "{\"id\":1,\"status\":\"Active\",\"title\":\"COVID Trial\",\"startDate\":\"2024-01-01\",...}",
  "createdAt": "2024-06-15 10:30:45"
}
```

Now anyone can see: "admin@test.com changed Study 1's status from Planned to Active on June 15th."

---

### The logAudit Helper (Simple but Critical)

```typescript
// helpers.ts
export function logAudit(
  context: GraphQLContext,
  action: 'CREATE' | 'UPDATE' | 'ASSIGN' | 'UNASSIGN',
  entityType: string,
  entityId: number,
  beforeJson: string | null,
  afterJson: string | null
): void {
  const user = context.user!;
  insertAuditLog(user.userId, user.email, action, entityType, entityId, beforeJson, afterJson);
}
```

**Why get actor info from context?**
- `context.user` was set from the JWT in the context function
- No extra DB query needed — email and userId are already in the token
- Every audit log automatically knows WHO performed the action

---

### Audit Patterns for Each Operation Type

#### CREATE (new entity):
```typescript
const study = createStudy(validated);
logAudit(context, 'CREATE', 'Study', study.id, 
  null,                    // ← No "before" (didn't exist)
  JSON.stringify(study)    // ← "after" is the new entity
);
```

#### UPDATE (modify entity):
```typescript
const before = getStudyById(Number(id));  // ← Capture before
const study = updateStudy(Number(id), validated);
logAudit(context, 'UPDATE', 'Study', study.id,
  JSON.stringify(before),  // ← What it was
  JSON.stringify(study)    // ← What it is now
);
```

#### ASSIGN (create relationship):
```typescript
assignSiteToStudy(Number(studyId), Number(siteId));
logAudit(context, 'ASSIGN', 'StudySite', Number(studyId),
  null,                                              // ← No "before"
  JSON.stringify({ studyId: Number(studyId), siteId: Number(siteId) })  // ← The relationship
);
```

#### UNASSIGN (remove relationship):
```typescript
unassignSiteFromStudy(Number(studyId), Number(siteId));
logAudit(context, 'UNASSIGN', 'StudySite', Number(studyId),
  JSON.stringify({ studyId: Number(studyId), siteId: Number(siteId) }),  // ← What was removed
  null                                               // ← No "after"
);
```

---

### The Audit Query (Reading Logs)

---

---

### How Audit Logs Are Queried

The `getAuditLogs` query supports multiple use cases:

**1. Global audit page (all logs, filterable by type):**
```graphql
query {
  getAuditLogs(entityType: "Study", page: 1, pageSize: 25) {
    rows { id actorEmail action entityType entityId beforeJson afterJson createdAt }
    total
  }
}
```

**2. Per-entity history (all changes to a specific study):**
```graphql
query {
  getAuditLogs(entityTypes: ["Study", "StudySite", "StudySiteExaminer"], entityId: 5, page: 1, pageSize: 25) {
    rows { ... }
    total
  }
}
```

**Why `entityTypes` array?** When viewing a study's history, you want to see:
- Changes to the study itself (`Study`)
- Sites assigned/unassigned (`StudySite`)
- Examiners assigned/unassigned at sites (`StudySiteExaminer`)

All related to entity ID 5. The array lets you query all related types at once.

---

### The Entity Type Map (What Gets Logged Where)

| entityType | Logged for | entityId is |
|---|---|---|
| `Study` | createStudy, updateStudy | study.id |
| `Site` | createSite, updateSite | site.id |
| `Examiner` | createExaminer, updateExaminer | examiner.id |
| `StudySite` | assignSiteToStudy, unassignSiteFromStudy | studyId |
| `SiteExaminer` | assignExaminerToSite, unassignExaminerFromSite | siteId |
| `StudySiteExaminer` | assignExaminerToStudySite, unassignExaminerFromStudySite | studyId |
| `ExaminerCertificate` | addExaminerCertificate, updateExaminerCertificate | examiner.id |

---

### How the Frontend Displays Audit Logs

The frontend takes `beforeJson` and `afterJson` and computes a DIFF:

```typescript
// utils/auditDiff.ts
export function diffObjects(before: Record<string, unknown>, after: Record<string, unknown>) {
  // Compare each field — show only what changed
  // Returns: [{ field: 'status', from: 'Planned', to: 'Active' }, ...]
}
```

The UI shows:
```
┌─────────────────────────────────────────────────────────────┐
│ admin@test.com • UPDATE • Study #1 • June 15, 2024 10:30   │
├─────────────────────────────────────────────────────────────┤
│ ▼ Changes:                                                  │
│   status:  Planned → Active                                 │
│   (other fields unchanged)                                  │
└─────────────────────────────────────────────────────────────┘
```

---

### Related Entity Types (Per-Entity History)

When viewing audit history for a specific entity, the frontend queries multiple related types:

```typescript
// Frontend: utils/auditDiff.ts or EntityAuditHistoryPage
const RELATED_ENTITY_TYPES: Record<string, string[]> = {
  Study: ['Study', 'StudySite', 'StudySiteExaminer'],
  Site: ['Site', 'SiteExaminer'],
  Examiner: ['Examiner', 'ExaminerCertificate'],
};
```

**Why?** A study's complete history includes:
- When it was created/updated (entityType: Study)
- When sites were assigned/unassigned (entityType: StudySite)
- When examiners were assigned to study sites (entityType: StudySiteExaminer)

All with `entityId = studyId`. One query gets the full picture.

---

### Why Audit Logging Matters

1. **Compliance** — clinical trials require audit trails (regulatory requirement)
2. **Debugging** — "when did this status change? who did it?"
3. **Accountability** — every action is attributed to a specific user
4. **Undo context** — beforeJson shows what to revert to (manual process)
5. **Security** — detect unauthorized changes

---

### Design Decisions

**Why JSON strings (not structured columns)?**
- Entities have different fields (Study has protocolId, Site has siteCode)
- JSON is flexible — works for any entity type
- Easy to add new fields without changing the audit table schema

**Why no hard deletes?**
- You can't audit something that doesn't exist
- Unassign (remove relationship) is logged, but the entities themselves are never deleted
- This preserves the complete history

**Why actorEmail in the log (not just actorUserId)?**
- Displaying logs doesn't require a JOIN to the users table
- Even if the user is deleted later, the log still shows who did it
- Performance: one less JOIN on every audit query

**Why ADMIN-only access to audit logs?**
- Audit logs may contain sensitive information (who changed what)
- Viewers don't need to see operational history
- `requireAdmin(context)` in the audit resolver

---

### If You Were Building From Scratch

```
1. Create the audit_logs table in migrate.ts
   - Start with just CREATE and UPDATE actions

2. Create auditRepository.ts
   - insertAuditLog (simple INSERT)
   - queryAuditLogs (with pagination)

3. Add logAudit to helpers.ts
   - Simple wrapper that reads actor from context

4. Add logAudit calls to your existing mutation resolvers
   - createStudy → logAudit('CREATE', ...)
   - updateStudy → logAudit('UPDATE', ...)

5. Add ASSIGN/UNASSIGN actions when you build assignments
   - Update the CHECK constraint if needed

6. Create auditService.ts + audit resolver
   - For reading logs (admin only)

7. Build the frontend audit page LAST
   - It's a read-only display of what's already being logged
```

**Key principle: Start logging EARLY. Even before you build the UI to view logs, the data is being captured.**

---

### Key Takeaways

1. **Every mutation logs** — CREATE, UPDATE, ASSIGN, UNASSIGN
2. **Before/after JSON** — captures the complete state change
3. **Actor from context** — no extra DB query, JWT has userId + email
4. **logAudit is one line** — called after the operation succeeds
5. **entityType + entityId** — identifies WHAT was changed
6. **Related entity types** — per-entity history includes junction changes
7. **ADMIN-only access** — audit logs are sensitive
8. **No hard deletes** — preserves complete history
9. **JSON storage** — flexible, works for any entity shape
10. **Log early, display later** — start capturing before building the UI

---

**Lesson 14 done.** Next is **Lesson 15: DataLoaders** — how to prevent the N+1 query problem when resolving nested fields in GraphQL.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 2, Lesson 15: DataLoaders — Preventing N+1 Queries

---

### The Thinking Process

> "My GraphQL API works great for single entities. But when I fetch a list of 10 studies and each study has `sites` and `examiners` fields... that's 10 queries for sites + 10 queries for examiners = 21 total queries for one page. This is the N+1 problem."

**The N+1 Problem Explained:**

```
Query: getStudies { rows { id title sites { name } } }

Without DataLoader:
  1 query: SELECT * FROM studies LIMIT 10           ← The "1"
  1 query: SELECT sites for study 1                 ← 
  1 query: SELECT sites for study 2                 ←  The "N"
  1 query: SELECT sites for study 3                 ←  (10 extra queries)
  ...                                               ←
  1 query: SELECT sites for study 10                ←
  = 11 queries total for 10 studies

With DataLoader:
  1 query: SELECT * FROM studies LIMIT 10
  1 query: SELECT sites WHERE study_id IN (1,2,3,4,5,6,7,8,9,10)  ← BATCHED!
  = 2 queries total for 10 studies
```

**DataLoader batches multiple individual loads into ONE query.**

---

### Let me show you the actual DataLoader file:

---

---

### How DataLoader Works (The Mental Model)

Think of DataLoader as a **smart waiter at a restaurant:**

Without DataLoader (dumb waiter):
```
Table 1: "I want a coffee"  → waiter goes to kitchen, comes back
Table 2: "I want a coffee"  → waiter goes to kitchen, comes back
Table 3: "I want a tea"     → waiter goes to kitchen, comes back
= 3 trips to the kitchen
```

With DataLoader (smart waiter):
```
Table 1: "I want a coffee"  → waiter writes it down
Table 2: "I want a coffee"  → waiter writes it down
Table 3: "I want a tea"     → waiter writes it down
→ waiter goes to kitchen ONCE with all 3 orders, comes back with all 3 drinks
= 1 trip to the kitchen
```

**DataLoader collects all `.load(id)` calls within a single tick of the event loop, then executes ONE batch function.**

---

### Two Types of Loaders in This Project

#### Type 1: Entity-by-ID Loaders

```typescript
studyById: new DataLoader<number, StudyRow | null>(async (ids) => {
  const rows = findStudiesByIds(ids);           // SELECT * FROM studies WHERE id IN (1,2,3,4,5)
  const map = new Map(rows.map((r) => [r.id, r]));
  return ids.map((id) => map.get(id) ?? null);  // Return in same order as requested
});
```

**How it works:**
1. Multiple resolvers call `loader.studyById.load(1)`, `loader.studyById.load(2)`, `loader.studyById.load(3)`
2. DataLoader collects all IDs: `[1, 2, 3]`
3. Batch function runs: `findStudiesByIds([1, 2, 3])` → one SQL query
4. Results are mapped back: each `.load()` call gets its specific result

**Critical rule:** The batch function must return results in the SAME ORDER as the input IDs. That's why we use a Map:
```typescript
const map = new Map(rows.map((r) => [r.id, r]));  // id → row
return ids.map((id) => map.get(id) ?? null);       // Preserve order
```

#### Type 2: Relation Loaders

```typescript
sitesByStudyId: new DataLoader<number, SiteRow[]>(async (studyIds) => {
  return studyIds.map((id) => findSitesByStudyId(id));
}, { cache: false }),
```

**What this does:** When 10 studies each need their sites resolved, instead of 10 separate calls happening at random times, DataLoader batches them into one tick.

**`cache: false`** — relation data shouldn't be cached within a request because it might change (e.g., after an assignment mutation in the same request).

---

### Where Loaders Are Created and Used

**Created per-request in app.ts:**
```typescript
// app.ts context function
context: async ({ req, res }) => {
  const user = token ? verifyToken(token) : null;
  return { user, req, res, requestId: req.requestId, loaders: createLoaders() };
  //                                                  ^^^^^^^^^^^^^^^^^^^^^^^^
  //                                                  Fresh loaders per request
},
```

**Why per-request?** 
- Each request gets its own DataLoader instances
- Prevents data from one user's request leaking into another's
- Cache is scoped to a single request (no stale data)

**Used in type resolvers:**
```typescript
Study: {
  sites(parent: StudyRow, _: unknown, context: GraphQLContext) {
    return context.loaders.sitesByStudyId.load(parent.id);
    //     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    //     Uses the per-request loader from context
  },
  examiners(parent: StudyRow, _: unknown, context: GraphQLContext) {
    return context.loaders.examinersByStudyId.load(parent.id);
  },
},
```

---

### The N+1 Problem Visualized

**Without DataLoader:**
```
getStudies returns 10 studies
  → Study.sites resolver called for study 1  → SELECT ... WHERE study_id = 1
  → Study.sites resolver called for study 2  → SELECT ... WHERE study_id = 2
  → Study.sites resolver called for study 3  → SELECT ... WHERE study_id = 3
  → ... (7 more)
  → Study.examiners resolver called for study 1  → SELECT ... WHERE study_id = 1
  → Study.examiners resolver called for study 2  → SELECT ... WHERE study_id = 2
  → ... (8 more)
= 1 + 10 + 10 = 21 queries
```

**With DataLoader:**
```
getStudies returns 10 studies
  → Study.sites resolver called for study 1  → loader.load(1)  ← queued
  → Study.sites resolver called for study 2  → loader.load(2)  ← queued
  → Study.sites resolver called for study 3  → loader.load(3)  ← queued
  → ... (7 more)                             → loader.load(4-10) ← queued
  → BATCH: findSitesByStudyId for all 10 at once
  → Study.examiners resolver called for all 10 → BATCH
= 1 + 1 + 1 = 3 queries (or slightly more depending on batching)
```

---

### The Loaders Interface (TypeScript)

```typescript
export interface Loaders {
  // Entity-by-ID (returns single entity or null)
  studyById: DataLoader<number, StudyRow | null>;
  siteById: DataLoader<number, SiteRow | null>;
  examinerById: DataLoader<number, ExaminerRow | null>;
  
  // Relations (returns arrays)
  sitesByStudyId: DataLoader<number, SiteRow[]>;
  examinersByStudyId: DataLoader<number, ExaminerRow[]>;
  studiesBySiteId: DataLoader<number, StudyRow[]>;
  examinersBySiteId: DataLoader<number, ExaminerRow[]>;
  studiesByExaminerId: DataLoader<number, StudyRow[]>;
  sitesByExaminerId: DataLoader<number, SiteRow[]>;
  certificatesByExaminerId: DataLoader<number, ExaminerCertificateRow[]>;
}
```

This is added to `GraphQLContext`:
```typescript
export interface GraphQLContext {
  user: JwtPayload | null;
  req: Request;
  res: Response;
  requestId: string;
  loaders: Loaders;  // ← Available in every resolver
}
```

---

### When DataLoader Helps vs When It Doesn't

**Helps (list pages with nested fields):**
```graphql
query {
  getStudies(page: 1, pageSize: 10) {
    rows {
      id title
      sites { name }       ← 10 studies × sites = N+1 without loader
      examiners { name }   ← 10 studies × examiners = N+1 without loader
    }
  }
}
```

**Doesn't help (single entity detail page):**
```graphql
query {
  getStudy(id: "5") {
    title
    sites { name }      ← Only 1 study, so only 1 sites query anyway
  }
}
```

For single entities, DataLoader adds minimal overhead but doesn't hurt. The real win is on list pages.

---

### If You Were Building From Scratch

```
1. Build your app WITHOUT DataLoaders first
   - Get everything working with direct repository calls in type resolvers
   - It will work fine for small datasets

2. Notice the N+1 problem when:
   - List pages get slow
   - You see many similar queries in your logs
   - Page load time increases with more items

3. Add DataLoaders:
   - Create loaders/index.ts with createLoaders()
   - Add `loaders` to your GraphQLContext type
   - Call createLoaders() in the context function
   - Replace direct calls in type resolvers with loader.load()

4. Add batch-fetch functions to repositories:
   - findStudiesByIds(ids: number[])
   - findSitesByIds(ids: number[])
   - These use WHERE id IN (?,?,?) queries
```

**DataLoaders are an OPTIMIZATION. Get it working first, then optimize.**

---

### Key Takeaways

1. **N+1 problem** — list of N items, each needing a sub-query = N+1 total queries
2. **DataLoader batches** — collects multiple `.load()` calls, executes ONE batch function
3. **Per-request** — `createLoaders()` called in context function, fresh per request
4. **Order matters** — batch function must return results in same order as input IDs
5. **Two types** — entity-by-ID (returns single) and relation (returns array)
6. **`cache: false`** for relations — prevents stale data within a request
7. **Used in type resolvers** — `context.loaders.sitesByStudyId.load(parent.id)`
8. **Optimization, not requirement** — app works without them, just slower
9. **Biggest win on list pages** — where N items each need related data
10. **Repository support** — need `findByIds` functions that accept arrays

---

**Phase 2 complete!** 🎉 You now understand the entire backend:
- ✅ Entry point (server.ts, app.ts)
- ✅ Middleware (security, logging, rate limiting)
- ✅ Database (schema, migrations, seeds)
- ✅ Repository layer (raw SQL, typed helpers)
- ✅ Service layer (business rules, domain logic)
- ✅ GraphQL schema (API contract)
- ✅ Resolvers (request handlers)
- ✅ Authentication (JWT, cookies, refresh tokens)
- ✅ Authorization (role guards)
- ✅ Validation (Zod, error flow)
- ✅ Audit logging (before/after snapshots)
- ✅ DataLoaders (N+1 prevention)

**Next: Phase 3 — Frontend.** We'll start with how React + Vite is set up, then how Apollo Client connects to the backend.

Say **"next"** to continue, or ask questions about anything in Phase 2.

---

next

---

## Phase 3, Lesson 16: Vite + React Setup

---

### The Thinking Process

> "Backend is done. Now I need a UI. How do I create a React project? What's Vite? How do I configure it?"

**Vite** (French for "fast") is a build tool that:
- Starts a dev server in milliseconds (not seconds like Webpack)
- Hot-reloads changes instantly
- Builds optimized production bundles

You'd start with: `npm create vite@latest frontend -- --template react-ts`

This gives you a working React + TypeScript project in seconds.

---

### Let me show you the actual setup files:

---

---

### Breaking Down the Setup

#### package.json — Your Dependencies

**Runtime dependencies (what the app uses):**
| Package | Purpose |
|---------|---------|
| `react` + `react-dom` | UI framework |
| `@apollo/client` + `graphql` | GraphQL client (talks to backend) |
| `@mui/material` + `@emotion/*` | UI component library (buttons, tables, dialogs) |
| `@mui/x-data-grid` | Advanced data table component |
| `@mui/icons-material` | Icon library |
| `react-router-dom` | Client-side routing (pages) |
| `react-hook-form` + `@hookform/resolvers` | Form management |
| `zod` | Validation (same as backend) |
| `notistack` | Toast notifications |
| `chart.js` + `react-chartjs-2` | Dashboard charts |

**Dev dependencies (only for development/testing):**
| Package | Purpose |
|---------|---------|
| `vite` + `@vitejs/plugin-react` | Build tool |
| `typescript` | Type checking |
| `vitest` + `@vitest/coverage-v8` | Testing |
| `@testing-library/react` | Component testing utilities |
| `jsdom` | Browser simulation for tests |

#### Scripts:
```json
"dev": "vite"              // Start dev server (hot reload)
"build": "tsc && vite build"  // Type-check then build for production
"test": "vitest run"       // Run tests once
```

---

#### vite.config.ts — Minimal Configuration

```typescript
export default defineConfig({
  plugins: [react()],        // Enable React JSX support
  server: { port: 5173 },   // Dev server port
});
```

That's it. Vite needs almost no configuration. The `react()` plugin handles JSX transformation.

---

#### tsconfig.json — TypeScript Configuration

Key settings:
```json
"strict": true          // No implicit any, strict null checks
"jsx": "react-jsx"     // Modern JSX transform (no need to import React in every file)
"noEmit": true          // TypeScript only checks types; Vite handles the actual build
"module": "ESNext"      // Use ES modules (import/export)
```

---

#### main.tsx — The Entry Point

```typescript
ReactDOM.createRoot(document.getElementById('root')!).render(
  <React.StrictMode>
    <ErrorBoundary>
      <SnackbarProvider maxSnack={3} autoHideDuration={4000}>
        <App />
      </SnackbarProvider>
    </ErrorBoundary>
  </React.StrictMode>
);
```

**The wrapping order matters (outside → inside):**

1. `React.StrictMode` — catches common mistakes during development
2. `ErrorBoundary` — catches any unhandled errors, shows fallback UI instead of white screen
3. `SnackbarProvider` — makes toast notifications available to any component
4. `App` — your actual application (routing, pages, etc.)

**Why this order?**
- ErrorBoundary must wrap everything so it catches errors from anywhere
- SnackbarProvider must wrap App so any page can show toasts
- App is innermost because it's the actual content

---

#### theme.ts — MUI Theme (Visual Identity)

```typescript
const theme = createTheme({
  palette: {
    primary: { main: '#0f766e' },  // Teal — used for buttons, links, active states
    background: { default: '#f1f5f9' },  // Light gray page background
  },
  typography: {
    fontFamily: "'Poppins', system-ui, sans-serif",  // Modern font
  },
  shape: { borderRadius: 8 },  // Rounded corners everywhere
  components: {
    MuiButton: {
      styleOverrides: {
        root: { textTransform: 'none', fontWeight: 600 },  // No UPPERCASE buttons
      },
    },
  },
});
```

**What a theme does:** Instead of styling every button individually, you define the look ONCE in the theme. Every MUI component automatically uses these settings.

Without theme: `<Button style={{ color: '#0f766e', borderRadius: 8, textTransform: 'none' }}>` (repeated everywhere)

With theme: `<Button>` (automatically styled)

---

### The index.html (Where React Mounts)

---

---

### How It All Connects

```
Browser loads index.html
  → <div id="root"></div> is empty
  → <script src="/src/main.tsx"> loads
  → main.tsx calls ReactDOM.createRoot(document.getElementById('root'))
  → React renders the entire app inside that div
  → Everything from here is JavaScript-controlled (Single Page Application)
```

**SPA (Single Page Application):** The browser loads ONE HTML page. React handles all "page navigation" by swapping components in and out — no full page reloads.

---

### If You Were Building From Scratch

```
1. npm create vite@latest frontend -- --template react-ts
   → Gives you: index.html, main.tsx, App.tsx, vite.config.ts, tsconfig.json

2. Install core dependencies:
   npm install @apollo/client graphql react-router-dom

3. Install UI library:
   npm install @mui/material @emotion/react @emotion/styled @mui/icons-material

4. Install form + validation:
   npm install react-hook-form @hookform/resolvers zod

5. Install extras:
   npm install notistack chart.js react-chartjs-2 @mui/x-data-grid

6. Create theme.ts (define your colors/fonts)

7. Wrap App in providers (main.tsx):
   ErrorBoundary → SnackbarProvider → App

8. Run: npm run dev → see blank page at localhost:5173
   → Now start building components
```

---

### Key Takeaways

1. **Vite** — fast build tool, minimal config, hot reload
2. **main.tsx** — entry point, wraps App in providers (ErrorBoundary, SnackbarProvider)
3. **theme.ts** — define visual identity once, applied everywhere
4. **index.html** — single HTML file with `<div id="root">` where React mounts
5. **SPA** — one page load, React handles all navigation
6. **Provider order** — outermost catches errors, innermost is your app
7. **`strict: true`** in tsconfig — catches bugs at compile time
8. **`"type": "module"`** in package.json — use ES module imports

---

**Lesson 16 done.** Next is **Lesson 17: Apollo Client** — how the frontend connects to the GraphQL backend, handles errors, and manages the auth cookie.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 3, Lesson 17: Apollo Client — Connecting Frontend to Backend

---

### The Thinking Process

> "My React app is running. My backend has a GraphQL API at localhost:4040/graphql. How do I connect them? How do I send queries? How do I handle errors globally?"

Answer: **Apollo Client.** It's the GraphQL client library that:
- Sends queries/mutations to your backend
- Caches responses (so repeated queries don't hit the server)
- Handles errors globally (auth failures, server errors)
- Manages loading/error states for every query

---

### Let me show you the actual Apollo Client setup:

---

---

### Breaking Down the Apollo Client

There are 3 main pieces:

```
apolloClient = httpLink + errorLink + cache
```

---

#### Piece 1: httpLink — "Where to send requests"

```typescript
const httpLink = createHttpLink({
  uri: import.meta.env.VITE_GRAPHQL_URL,  // "http://localhost:4040/graphql"
  credentials: 'include',                  // Send cookies with every request
});
```

- `uri` — the backend GraphQL endpoint
- `credentials: 'include'` — **CRITICAL.** Without this, the browser won't send the HttpOnly cookies. Your auth would break silently.

`import.meta.env.VITE_GRAPHQL_URL` reads from `frontend/.env`:
```
VITE_GRAPHQL_URL=http://localhost:4040/graphql
```

---

#### Piece 2: InMemoryCache — "Remember previous responses"

```typescript
cache: new InMemoryCache()
```

Apollo caches query results. If you fetch `getStudy(id: "5")` and then navigate away and come back, Apollo can serve the cached result instantly (while optionally refetching in the background).

---

#### Piece 3: errorLink — "Handle errors globally"

This is the most complex and important part. It intercepts EVERY error before it reaches your components.

---

### The Error Link — Handling Each Error Type

#### UNAUTHENTICATED (Token Expired)

```typescript
if (code === 'UNAUTHENTICATED') {
  // Don't refresh if we're already on the login page
  if (onLoginPage) return;
  
  // Don't refresh the refresh mutation itself (infinite loop!)
  if (operation.operationName === 'RefreshSession') {
    redirectToLogin();
    return;
  }

  // Try to refresh the token, then retry the original request
  return new Observable((observer) => {
    doRefresh().then((success) => {
      if (!success) {
        redirectToLogin();  // Refresh failed → go to login
        return;
      }
      // Retry the original operation (now with fresh cookie)
      forward(operation).subscribe(observer);
    });
  });
}
```

**The flow:**
```
1. User's access token expires (after 15 min)
2. Next query returns UNAUTHENTICATED
3. errorLink catches it
4. Calls refreshSession mutation (uses refresh_token cookie)
5. If refresh succeeds → new access token cookie is set → retry original query
6. If refresh fails → redirect to /login
7. User never notices (seamless)
```

#### The Single-Promise Pattern (Preventing Refresh Storms)

```typescript
let refreshPromise: Promise<boolean> | null = null;

function doRefresh(): Promise<boolean> {
  if (refreshPromise) return refreshPromise;  // ← Reuse existing promise
  
  refreshPromise = apolloClient.mutate({ mutation: REFRESH_SESSION_MUTATION })
    .then(...)
    .finally(() => { refreshPromise = null; });
  
  return refreshPromise;
}
```

**Why?** Imagine 5 queries fire simultaneously, all get UNAUTHENTICATED. Without this, you'd send 5 refresh requests. With this, all 5 wait on the SAME refresh promise.

#### FORBIDDEN (Wrong Role)

```typescript
if (code === 'FORBIDDEN') {
  showToastOnce("You don't have permission to perform this action.", 'error', 'FORBIDDEN');
}
```

Shows a toast. Doesn't redirect — user is still logged in, just wrong role.

#### INTERNAL_SERVER_ERROR (Bug on Server)

```typescript
if (code === 'INTERNAL_SERVER_ERROR') {
  console.error('[GraphQL INTERNAL_SERVER_ERROR]', err);
  showToastOnce('Something went wrong. Please try again.', 'error', 'INTERNAL_SERVER_ERROR');
}
```

Logs to console (for debugging), shows generic toast (don't leak details to user).

#### BAD_USER_INPUT (Validation Error)

```typescript
// BAD_USER_INPUT handled per-mutation in components — no global toast.
```

**Not handled here!** Each form component handles its own validation errors by mapping `fieldErrors` to form fields. A global toast would be confusing.

#### Network Errors (Server Down)

```typescript
if (status === 503 || status === 502 || status === 504) {
  showToastOnce('Server temporarily unavailable.', 'error', 'SERVER_UNAVAILABLE');
}
if (!status) {
  showToastOnce('Network error — check your connection.', 'error', 'NETWORK_ERROR');
}
```

---

### Toast Deduplication (Preventing Spam)

```typescript
let lastToastKey = '';
let lastToastTime = 0;

function showToastOnce(message: string, variant: 'error' | 'warning', key: string) {
  const now = Date.now();
  if (key === lastToastKey && now - lastToastTime < 3000) return;  // Skip if same toast within 3s
  lastToastKey = key;
  lastToastTime = now;
  enqueueSnackbar(message, { variant });
}
```

**Why?** If 5 queries fail simultaneously with FORBIDDEN, you don't want 5 identical toasts stacking up. This shows only ONE within a 3-second window.

---

### How Apollo Client Is Used in the App

---

---

### The Provider Stack (App.tsx)

```typescript
<ThemeProvider theme={theme}>        // MUI theme (colors, fonts)
  <CssBaseline />                    // Reset browser default styles
  <ApolloProvider client={apolloClient}>  // Makes Apollo available to all components
    <AuthProvider>                   // Auth context (who's logged in?)
      <BrowserRouter>                // React Router (URL-based navigation)
        <Routes>...</Routes>
      </BrowserRouter>
    </AuthProvider>
  </ApolloProvider>
</ThemeProvider>
```

**Why this order?**
- `ThemeProvider` outermost — everything needs styling
- `ApolloProvider` wraps `AuthProvider` — because AuthProvider uses Apollo queries (ME_QUERY)
- `AuthProvider` wraps `BrowserRouter` — because routes need to know the user's role
- `BrowserRouter` wraps `Routes` — enables URL-based navigation

---

### How Components Use Apollo

Once `ApolloProvider` wraps your app, any component can use Apollo hooks:

```typescript
// In any component:
import { useQuery, useMutation } from '@apollo/client';

// Fetch data:
const { data, loading, error } = useQuery(GET_STUDIES_QUERY, {
  variables: { page: 1, pageSize: 10 }
});

// Mutate data:
const [createStudy] = useMutation(CREATE_STUDY_MUTATION);
await createStudy({ variables: { input: { ... } } });
```

Apollo handles:
- Sending the request to the backend
- Including cookies (credentials: 'include')
- Caching the response
- Providing loading/error states
- Triggering re-renders when data arrives

---

### The Link Chain (How Requests Flow)

```typescript
export const apolloClient = new ApolloClient({
  link: from([errorLink, httpLink]),  // ← Chain: errorLink → httpLink
  cache: new InMemoryCache(),
});
```

**`from([errorLink, httpLink])`** creates a chain:

```
Component calls useQuery/useMutation
  → errorLink (intercepts errors on the way BACK)
  → httpLink (sends the actual HTTP request)
  → Backend responds
  → errorLink checks for errors
  → If error: handle it (refresh, toast, redirect)
  → If success: pass data to component
```

---

### The Refresh Flow Visualized

```
Time 0:00  — User logs in, gets access token (15 min) + refresh token (7 days)
Time 0:14  — User is working normally, all queries succeed
Time 0:15  — Access token expires
Time 0:15  — User clicks something → query sent → backend returns UNAUTHENTICATED
Time 0:15  — errorLink catches UNAUTHENTICATED
Time 0:15  — errorLink calls doRefresh() → sends refreshSession mutation
Time 0:15  — Backend validates refresh cookie → issues new access token + new refresh token
Time 0:15  — New cookies set in browser
Time 0:15  — errorLink retries the original query with new cookie
Time 0:15  — Query succeeds → user sees their data
Time 0:15  — User never noticed anything happened ✨
```

---

### If You Were Building From Scratch

```
1. Install: npm install @apollo/client graphql

2. Create utils/apolloClient.ts with JUST:
   const httpLink = createHttpLink({ uri: '...', credentials: 'include' });
   export const apolloClient = new ApolloClient({ link: httpLink, cache: new InMemoryCache() });

3. Wrap App in ApolloProvider (App.tsx)

4. Test: write a simple useQuery in a component → verify data comes back

5. Add errorLink LATER when you need:
   - Global error handling (FORBIDDEN toast)
   - Token refresh (UNAUTHENTICATED → refresh → retry)
   - Network error handling

6. Add toast deduplication when you notice spam
```

**Start simple. Add error handling as you encounter each case.**

---

### Key Takeaways

1. **Apollo Client** = httpLink (where to send) + errorLink (error handling) + cache (remember responses)
2. **`credentials: 'include'`** — MUST have this for HttpOnly cookies to work
3. **errorLink** — global error interceptor, handles auth refresh, toasts, redirects
4. **Single refresh promise** — prevents multiple simultaneous refresh requests
5. **Toast deduplication** — same error within 3s shows only one toast
6. **BAD_USER_INPUT not handled globally** — each form handles its own field errors
7. **UNAUTHENTICATED → refresh → retry** — seamless to the user
8. **Provider stack order** — Theme → Apollo → Auth → Router → Routes
9. **`from([errorLink, httpLink])`** — chain of links, errors intercepted on the way back
10. **`ApolloProvider`** — makes `useQuery`/`useMutation` available in all components

---

**Lesson 17 done.** Next is **Lesson 18: Routing** — how React Router handles navigation, protected routes, and the admin vs viewer separation.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 3, Lesson 18: Routing — Protected Routes + Admin vs Viewer

---

### The Thinking Process

> "I have multiple pages — login, dashboard, studies list, study detail, etc. How does the browser know which page to show? How do I prevent a viewer from accessing admin pages? How do I redirect unauthenticated users to login?"

Answer: **React Router** handles URL → component mapping. **Route guards** (AdminRoute, ProtectedRoute) handle access control.

---

### The Route Structure (Already Seen in App.tsx)

```
/login                          → Public (anyone)
/admin/*                        → AdminRoute (must be ADMIN)
/viewer/*                       → ProtectedRoute (must be logged in, any role)
/*                              → Redirect to /login
```

**The key insight:** Admin and Viewer see DIFFERENT pages for the same data. Admin sees CRUD buttons, Viewer sees read-only. They're completely separate page components with separate routes.

---

### Let me show you the route guard components:

---

---

### The AuthContext — "Who Am I?"

```typescript
export function AuthProvider({ children }) {
  const { loading, data, error } = useQuery(ME_QUERY, { fetchPolicy: 'network-only' });

  const isLoggedIn = !loading && !error && !!data?.me;
  const role = data?.me?.role ?? null;

  return (
    <AuthContext.Provider value={{ isLoggedIn, isChecking: loading, role }}>
      {children}
    </AuthContext.Provider>
  );
}
```

**What happens when the app loads:**
1. `AuthProvider` mounts
2. It sends `ME_QUERY` to the backend (which reads the auth cookie)
3. While waiting → `isChecking = true` (show loading spinner)
4. If cookie is valid → backend returns user → `isLoggedIn = true`, `role = 'ADMIN'`
5. If no cookie or expired → backend returns error → `isLoggedIn = false`

**`fetchPolicy: 'network-only'`** — always ask the server, never use cached data. Auth state must be fresh.

**`useAuth()` hook** — any component can call this to get `{ isLoggedIn, isChecking, role }`.

---

### ProtectedRoute — "Must Be Logged In"

```typescript
export function ProtectedRoute({ children }) {
  const { isLoggedIn, isChecking } = useAuth();
  
  if (isChecking) return <CircularProgress />;           // Still checking → show spinner
  return isLoggedIn ? <>{children}</> : <Navigate to="/login" replace />;
}
```

**Three states:**
1. `isChecking = true` → show loading spinner (don't flash login page)
2. `isLoggedIn = true` → render the page
3. `isLoggedIn = false` → redirect to /login

**`replace`** — replaces the current history entry. So pressing "Back" doesn't go to the protected page (which would just redirect again).

---

### AdminRoute — "Must Be ADMIN"

```typescript
export function AdminRoute({ children }) {
  const { isLoggedIn, isChecking, role } = useAuth();
  
  if (isChecking) return <CircularProgress />;
  if (!isLoggedIn) return <Navigate to="/login" replace />;
  if (role !== 'ADMIN') return <Navigate to="/viewer/dashboard" replace />;
  return <>{children}</>;
}
```

**Four states:**
1. `isChecking` → spinner
2. Not logged in → redirect to /login
3. Logged in but VIEWER → redirect to /viewer/dashboard (not login!)
4. Logged in AND ADMIN → render the page

**Key difference from ProtectedRoute:** A VIEWER who tries to access `/admin/studies` gets redirected to their own dashboard, not kicked to login.

---

### How Routes Work in App.tsx

```typescript
<Route path="/admin/studies" element={<AdminRoute><AdminStudiesPage /></AdminRoute>} />
```

This means:
1. User navigates to `/admin/studies`
2. React Router matches this route
3. It renders `<AdminRoute>` which wraps `<AdminStudiesPage />`
4. AdminRoute checks auth → if ADMIN, renders AdminStudiesPage
5. If not ADMIN, redirects away

**The pattern:** Route guard wraps the page component.

---

### Route Organization

```
/login                    → LoginPage (no guard — public)

/admin/dashboard          → AdminRoute → AdminDashboardPage
/admin/studies            → AdminRoute → AdminStudiesPage
/admin/studies/:id        → AdminRoute → AdminStudyDetailPage
/admin/studies/:id/history → AdminRoute → StudyAuditHistoryPage
/admin/sites              → AdminRoute → AdminSitesPage
/admin/sites/:id          → AdminRoute → AdminSiteDetailPage
/admin/examiners          → AdminRoute → AdminExaminersPage
/admin/examiners/:id      → AdminRoute → AdminExaminerDetailPage
/admin/search             → AdminRoute → AdminSearchPage
/admin/audit-logs         → AdminRoute → AuditLogsPage

/viewer/dashboard         → ProtectedRoute → ViewerDashboardPage
/viewer/studies           → ProtectedRoute → ViewerStudiesPage
/viewer/studies/:id       → ProtectedRoute → ViewerStudyDetailPage
/viewer/sites             → ProtectedRoute → ViewerSitesPage
/viewer/examiners         → ProtectedRoute → ViewerExaminersPage
/viewer/search            → ProtectedRoute → ViewerSearchPage

/*                        → Navigate to /login (catch-all)
```

**`:id`** is a URL parameter. React Router extracts it:
```typescript
// Inside AdminStudyDetailPage:
const { id } = useParams();  // id = "5" from URL /admin/studies/5
```

---

### Legacy Redirects

```typescript
<Route path="/dashboard" element={<Navigate to="/viewer/dashboard" replace />} />
<Route path="/studies" element={<Navigate to="/viewer/studies" replace />} />
```

**Why?** If someone bookmarked `/studies` from an older version of the app, they get redirected to the new `/viewer/studies` path instead of seeing a 404.

---

### The Login Flow (Route Perspective)

```
1. User opens app → hits /* catch-all → redirected to /login
2. User logs in → useLogin hook → on success:
   - If role === 'ADMIN' → navigate('/admin/dashboard')
   - If role === 'VIEWER' → navigate('/viewer/dashboard')
3. User is now on a protected route → AdminRoute/ProtectedRoute allows it
4. User clicks Logout → cookies cleared → ME_QUERY fails → isLoggedIn = false
5. Route guard detects isLoggedIn = false → redirects to /login
```

Let me show you the login hook:

---

---

### The Login Hook — Connecting Auth to Routing

```typescript
export function useLogin() {
  const [loginMutation] = useMutation(LOGIN_MUTATION);
  const client = useApolloClient();
  const navigate = useNavigate();

  async function submitLogin(email: string, password: string) {
    const { data } = await loginMutation({ variables: { email, password } });
    
    // After login, refetch ME_QUERY so AuthContext updates
    await client.refetchQueries({ include: [ME_QUERY] });
    
    // Navigate based on role
    const role = data?.login?.user?.role;
    navigate(role === 'ADMIN' ? '/admin/dashboard' : '/viewer/dashboard');
  }
}
```

**The critical step:** `client.refetchQueries({ include: [ME_QUERY] })`

After login, the cookie is set. But `AuthContext` still has the old state (isLoggedIn = false). By refetching ME_QUERY, the AuthContext updates → `isLoggedIn = true`, `role = 'ADMIN'` → route guards now allow access.

---

### How Navigation Works (No Page Reloads)

```typescript
import { useNavigate } from 'react-router-dom';

const navigate = useNavigate();
navigate('/admin/studies');      // Go to studies page
navigate('/admin/studies/5');    // Go to study detail
navigate(-1);                    // Go back (like browser back button)
```

**This is client-side navigation.** The browser doesn't reload the page. React Router just swaps the component being rendered. This is why SPAs feel fast.

**For links in JSX:**
```typescript
import { Link } from 'react-router-dom';
<Link to="/admin/studies/5">View Study</Link>
```

---

### URL Parameters (Dynamic Routes)

```typescript
// Route definition:
<Route path="/admin/studies/:id" element={...} />

// Inside the component:
import { useParams } from 'react-router-dom';
const { id } = useParams();  // "5" from /admin/studies/5
```

This is how detail pages know WHICH entity to fetch.

---

### If You Were Building From Scratch

```
1. Install: npm install react-router-dom

2. Create App.tsx with BrowserRouter + Routes:
   - Just /login and one protected route initially
   - <Route path="/login" element={<LoginPage />} />
   - <Route path="/dashboard" element={<DashboardPage />} />

3. Create AuthContext:
   - useQuery(ME_QUERY) → derive isLoggedIn + role
   - Wrap App in AuthProvider

4. Create ProtectedRoute:
   - Check isLoggedIn → render children or redirect to /login
   - Wrap your dashboard route

5. Create AdminRoute (when you add admin features):
   - Check role === 'ADMIN' → render or redirect

6. Add more routes as you build pages:
   - /admin/studies, /admin/studies/:id, etc.

7. Add legacy redirects last (when you refactor URLs)
```

---

### Key Takeaways

1. **AuthContext** — single source of truth for "who's logged in" (uses ME_QUERY)
2. **ProtectedRoute** — any logged-in user can access
3. **AdminRoute** — only ADMIN role can access; VIEWER gets redirected to their dashboard
4. **`isChecking` state** — prevents flash of login page while auth is being verified
5. **`replace`** — prevents back-button loops
6. **`useParams()`** — extracts `:id` from URL for detail pages
7. **`navigate()`** — programmatic navigation (after login, after create, etc.)
8. **`refetchQueries([ME_QUERY])`** — updates auth state after login
9. **Client-side navigation** — no page reloads, just component swaps
10. **Catch-all route `/*`** — anything unmatched goes to /login

---

**Lesson 18 done.** Next is **Lesson 19: Auth Context** — a deeper look at how the app manages auth state, the useAuth hook, and how components react to login/logout.

Actually, we've already covered AuthContext in depth in this lesson. Let me skip ahead to **Lesson 20: Layouts & Navigation** — how the sidebar, header, and page structure work for admin vs viewer.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 3, Lesson 19: Layouts & Navigation

---

### The Thinking Process

> "I have routes and pages. But every page needs a sidebar, a header, and a main content area. Do I copy-paste the sidebar into every page? No — I create a LAYOUT component that wraps the page content."

Answer: **Layout components.** Admin pages use `AdminLayout`, Viewer pages use `ViewerLayout`. Each layout provides the header + sidebar + content area. Individual pages only worry about their own content.

---

### Let me show you the layout files:

---

---

### The Layout Pattern — Visual Structure

```
┌─────────────────────────────────────────────────────────────┐
│  AppHeader (fixed at top, full width)                        │
│  [Logo] SNA Clinical Studies                    [Avatar] [Logout] │
├──────────┬──────────────────────────────────────────────────┤
│          │                                                   │
│  Sidebar │   Main Content Area                              │
│          │   (your page component renders here)             │
│  Dashboard│                                                  │
│  Studies  │   ┌─────────────────────────────────────┐       │
│  Sites    │   │  AdminStudiesPage                    │       │
│  Examiners│   │  (DataGrid, Create button, etc.)    │       │
│  Search   │   └─────────────────────────────────────┘       │
│  Audit    │                                                  │
│          │                                                   │
├──────────┴──────────────────────────────────────────────────┤
│  AppFooter                                                   │
└─────────────────────────────────────────────────────────────┘
```

---

### AdminLayout — The Wrapper

```typescript
export function AdminLayout({ children }: { children: ReactNode }) {
  return (
    <Box sx={{ display: 'flex', flexDirection: 'column', minHeight: '100vh' }}>
      <AppHeader showLogout />
      <Box sx={{ display: 'flex', flex: 1, mt: `${APPBAR_HEIGHT}px` }}>
        <AdminSidebar />
        <Box component="main" sx={{ flex: 1, p: 3, bgcolor: 'background.default' }}>
          {children}    {/* ← Your page content goes here */}
        </Box>
      </Box>
      <AppFooter />
    </Box>
  );
}
```

**How pages use it:**
```typescript
// Inside AdminStudiesPage:
export function AdminStudiesPage() {
  return (
    <AdminLayout>
      {/* Only the page-specific content */}
      <Typography variant="h5">Studies</Typography>
      <DataGrid ... />
    </AdminLayout>
  );
}
```

The page doesn't know about the header or sidebar — it just renders its content inside `AdminLayout`.

---

### AdminSidebar — Collapsible Navigation

Key features:

**1. Navigation items defined as data:**
```typescript
const navItems = [
  { label: 'Dashboard',  path: '/admin/dashboard',  icon: <DashboardIcon /> },
  { label: 'Studies',    path: '/admin/studies',    icon: <ScienceIcon /> },
  { label: 'Sites',      path: '/admin/sites',      icon: <LocationOnIcon /> },
  { label: 'Examiners',  path: '/admin/examiners',  icon: <PersonSearchIcon /> },
  { label: 'Search',     path: '/admin/search',     icon: <SearchIcon /> },
  { label: 'Audit Logs', path: '/admin/audit-logs', icon: <HistoryIcon /> },
];
```

**Why data-driven?** Adding a new nav item = adding one object to the array. No JSX changes needed.

**2. Active state detection:**
```typescript
function isActive(path: string) {
  return location.pathname === path || location.pathname.startsWith(path + '/');
}
```

If you're on `/admin/studies/5`, the "Studies" nav item is highlighted because `/admin/studies/5` starts with `/admin/studies/`.

**3. Collapsible (expand/collapse):**
```typescript
const [open, setOpen] = useState(true);
const width = open ? EXPANDED_WIDTH : COLLAPSED_WIDTH;  // 220px or 60px
```

When collapsed, only icons show. Tooltips appear on hover to show the label.

**4. Permanent drawer:**
```typescript
<Drawer variant="permanent" ...>
```

`variant="permanent"` means the sidebar is always visible (not a slide-out overlay). It's part of the page layout.

---

### AppHeader — Fixed Top Bar

```typescript
export function AppHeader({ showLogout = false }) {
  // Shows: Logo + App Name + User Avatar + Logout button
  
  async function handleLogout() {
    await logoutMutation();        // Tell backend to revoke refresh token
    await client.resetStore();     // Clear Apollo cache (remove all cached data)
    enqueueSnackbar('Signed out successfully.', { variant: 'info' });
    navigate('/login');            // Go to login page
  }
}
```

**`client.resetStore()`** — clears ALL cached data from Apollo. Important because after logout, you don't want the next user to see the previous user's data from cache.

**`position="fixed"`** — header stays at the top even when you scroll. That's why the content area has `mt: APPBAR_HEIGHT` (margin-top to avoid being hidden behind the header).

---

### Viewer Layout (Same Pattern, Different Sidebar)

---

---

### Admin vs Viewer Sidebar — The Differences

| Feature | Admin Sidebar | Viewer Sidebar |
|---------|--------------|----------------|
| Dashboard | ✅ `/admin/dashboard` | ✅ `/viewer/dashboard` |
| Studies | ✅ `/admin/studies` | ✅ `/viewer/studies` |
| Sites | ✅ `/admin/sites` | ✅ `/viewer/sites` |
| Examiners | ✅ `/admin/examiners` | ✅ `/viewer/examiners` |
| Search | ✅ `/admin/search` | ✅ `/viewer/search` |
| Audit Logs | ✅ `/admin/audit-logs` | ❌ Not available |
| Label | "Admin" | "Viewer" |

Same component structure, different nav items and paths. Viewer doesn't see Audit Logs because they don't have access.

---

### How a Page Uses the Layout

```typescript
// pages/admin/StudiesPage.tsx
export function AdminStudiesPage() {
  return (
    <AdminLayout>
      <Box sx={{ display: 'flex', justifyContent: 'space-between', mb: 2 }}>
        <Typography variant="h5">Studies</Typography>
        <Button onClick={() => setCreateOpen(true)}>+ New Study</Button>
      </Box>
      <DataGrid rows={studies} columns={columns} ... />
      <CreateStudyDialog open={createOpen} onClose={() => setCreateOpen(false)} />
    </AdminLayout>
  );
}

// pages/viewer/StudiesPage.tsx
export function ViewerStudiesPage() {
  return (
    <ViewerLayout>
      <Typography variant="h5">Studies</Typography>
      {/* No "New Study" button — read only */}
      <DataGrid rows={studies} columns={columns} ... />
    </ViewerLayout>
  );
}
```

**The pattern:**
- Admin page: Layout + CRUD buttons + DataGrid + Dialogs
- Viewer page: Layout + DataGrid (read-only, no buttons)

---

### The Logout Flow (From Header)

```typescript
async function handleLogout() {
  await logoutMutation();        // 1. Backend revokes refresh token + clears cookies
  await client.resetStore();     // 2. Clear all cached data from Apollo
  enqueueSnackbar('Signed out.'); // 3. Show toast
  navigate('/login');            // 4. Go to login page
}
```

After this:
- Cookies are gone (backend cleared them)
- Apollo cache is empty (no stale data)
- User is on /login page
- If they try to go back, ProtectedRoute redirects them to /login again

---

### If You Were Building From Scratch

```
1. Create AppHeader (just logo + app name)
   - Add logout button later when auth works

2. Create a simple Layout component:
   - Header at top
   - Content area below
   - No sidebar yet

3. Add sidebar when you have multiple pages:
   - Start with a static list of links
   - Add active state highlighting
   - Add collapse/expand later (polish)

4. Split into AdminLayout + ViewerLayout when you add roles:
   - Different nav items
   - Different paths

5. Add AppFooter last (it's just cosmetic)
```

---

### Key Takeaways

1. **Layout = Header + Sidebar + Content area** — pages only render their content
2. **AdminLayout vs ViewerLayout** — different sidebars, same structure
3. **Data-driven nav items** — array of objects, easy to add/remove
4. **Active state** — `pathname.startsWith(path)` highlights current section
5. **Collapsible sidebar** — `useState(true)` toggles between 220px and 60px
6. **Fixed header** — `position="fixed"` + content has `margin-top`
7. **Permanent drawer** — always visible, not an overlay
8. **Logout clears everything** — mutation + resetStore + navigate
9. **`{children}` pattern** — layout accepts any content via React children
10. **Viewer has no Audit Logs** — sidebar reflects what the role can access

---

**Lesson 19 done.** Next is **Lesson 20: List Pages** — how DataGrid works with server-side pagination, the useUrlPagination hook, and how admin list pages are structured.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 3, Lesson 20: List Pages — DataGrid + Server-Side Pagination

---

### The Thinking Process

> "I need to show a table of studies (or sites, or examiners). There could be hundreds of records. I can't load them all at once — I need pagination. And the page/pageSize should be in the URL so the user can bookmark or share the link."

Answer: **MUI DataGrid** for the table + **server-side pagination** (backend returns one page at a time) + **useUrlPagination** hook to persist page state in the URL.

---

### Let me show you a complete list page:

---

---

### The Complete List Page Pattern

Every admin list page follows this structure:

```
┌─────────────────────────────────────────────────────────────┐
│  [Title]                                    [+ New Entity]  │
│  Subtitle text                                              │
├─────────────────────────────────────────────────────────────┤
│  ┌─────────────────────────────────────────────────────┐    │
│  │  DataGrid (server-paginated table)                   │    │
│  │  Protocol ID | Study Name | Sponsor | Status | Edit  │    │
│  │  ─────────────────────────────────────────────────── │    │
│  │  PROT-001   | COVID Trial | Pfizer | Planned | [Edit]│    │
│  │  PROT-002   | Flu Study   | Roche  | Active  | [Edit]│    │
│  │  ...                                                 │    │
│  │  ─────────────────────────────────────────────────── │    │
│  │  < 1 2 3 ... 5 >    Rows per page: [10 ▼]          │    │
│  └─────────────────────────────────────────────────────┘    │
└─────────────────────────────────────────────────────────────┘

+ CreateStudyDialog (modal, 2-step stepper)
+ EditStudyDialog (modal, 2-step stepper)
```

---

### Key Piece 1: useUrlPagination Hook

```typescript
export function useUrlPagination(defaultPageSize = 10): [GridPaginationModel, setter] {
  const [searchParams, setSearchParams] = useSearchParams();
  
  const page = Math.max(0, Number(searchParams.get('page') ?? 0));
  const pageSize = VALID_PAGE_SIZES.includes(rawPageSize) ? rawPageSize : defaultPageSize;
  
  function setPaginationModel(model: GridPaginationModel) {
    setSearchParams((prev) => {
      const next = new URLSearchParams(prev);
      next.set('page', String(model.page));
      next.set('pageSize', String(model.pageSize));
      return next;
    }, { replace: true });
  }
  
  return [paginationModel, setPaginationModel];
}
```

**What this does:**
- Reads `?page=2&pageSize=20` from the URL
- When user changes page → updates the URL
- `replace: true` → back button doesn't go through every page change

**Why URL pagination?**
- User can bookmark `/admin/studies?page=3&pageSize=20`
- Browser back button restores exact pagination state
- Shareable links

---

### Key Piece 2: useStudies Hook (Data Fetching)

```typescript
export function useStudies(page = 1, pageSize = 10) {
  const { data, loading, error } = useQuery(GET_STUDIES_QUERY, {
    variables: { page, pageSize },
  });
  const studies: Study[] = data?.getStudies?.rows ?? [];
  const total: number = data?.getStudies?.total ?? 0;
  return { studies, total, loading, error };
}
```

**Simple wrapper around Apollo's useQuery:**
- Sends page + pageSize to backend
- Returns `{ studies, total, loading, error }`
- `?? []` fallback prevents crashes when data is still loading

---

### Key Piece 3: DataGrid with Server-Side Pagination

```typescript
<DataGrid
  rows={studies}                    // Data for current page
  columns={columns}                // Column definitions
  rowCount={total}                 // Total rows (for pagination display)
  paginationMode="server"         // ← KEY: tells DataGrid "I handle pagination"
  paginationModel={paginationModel}
  onPaginationModelChange={setPaginationModel}
  pageSizeOptions={[10, 20]}
  autoHeight
  onRowClick={(p) => navigate(`/admin/studies/${p.row.id}`)}
/>
```

**`paginationMode="server"`** is the critical prop. It tells DataGrid:
- "Don't try to paginate the data yourself"
- "I'll give you one page at a time via `rows`"
- "Use `rowCount` to calculate total pages"
- "Call `onPaginationModelChange` when user clicks next/prev"

**Without `paginationMode="server"`:** DataGrid expects ALL data upfront and paginates client-side. Fine for 50 rows, terrible for 10,000.

---

### Key Piece 4: Column Definitions

```typescript
const columns: GridColDef[] = [
  { field: 'protocolId', headerName: 'Protocol ID', width: 120 },
  { field: 'title', headerName: 'Study Name', flex: 1, minWidth: 180 },
  { field: 'status', headerName: 'Status', width: 120, 
    renderCell: (p) => <StatusChip status={p.value} />  // Custom render
  },
  { field: 'actions', headerName: 'Actions', width: 100, sortable: false,
    renderCell: (p) => (
      <Button onClick={(e) => { e.stopPropagation(); setEditingStudy(p.row); }}>
        Edit
      </Button>
    ),
  },
];
```

- `field` — maps to the property name on the row object
- `flex: 1` — takes remaining space
- `renderCell` — custom rendering (chips, buttons, etc.)
- `e.stopPropagation()` — prevents row click when clicking Edit button

---

### Key Piece 5: The Page Component (Putting It Together)

```typescript
export function AdminStudiesPage() {
  // 1. Pagination state (from URL)
  const [paginationModel, setPaginationModel] = useUrlPagination(10);
  
  // 2. Fetch data (page + 1 because DataGrid is 0-indexed, backend is 1-indexed)
  const { studies, total, loading, error } = useStudies(
    paginationModel.page + 1,  // DataGrid: page 0 = first page. Backend: page 1 = first page
    paginationModel.pageSize
  );
  
  // 3. Dialog state
  const [createOpen, setCreateOpen] = useState(false);
  const [editingStudy, setEditingStudy] = useState<Study | null>(null);

  return (
    <AdminLayout>
      {/* Header with title + Create button */}
      {/* DataGrid with data */}
      {/* Create dialog (conditional) */}
      {/* Edit dialog (conditional) */}
    </AdminLayout>
  );
}
```

**The 0-indexed vs 1-indexed conversion:**
- DataGrid uses 0-indexed pages (page 0 = first page)
- Backend uses 1-indexed pages (page 1 = first page)
- `paginationModel.page + 1` converts between them

---

### The Three States

```typescript
{loading && <TableSkeleton />}                    // Loading → show skeleton
{error && <Alert severity="error">{error.message}</Alert>}  // Error → show alert
{!loading && !error && <DataGrid ... />}          // Success → show table
```

Every list page handles these three states. Users always see something meaningful.

---

### If You Were Building From Scratch

```
1. Create the hook first (useStudies):
   - Just useQuery + return { studies, total, loading, error }

2. Create a basic page with DataGrid:
   - Hardcode page=1, pageSize=10
   - Get the table rendering

3. Add useUrlPagination:
   - Replace hardcoded values with URL-based state
   - Now pagination works + URL updates

4. Add Create button + dialog:
   - useState for open/close
   - Form inside dialog
   - Mutation on submit

5. Add Edit button + dialog:
   - useState for which entity is being edited
   - Pre-fill form with existing values

6. Add loading/error states:
   - TableSkeleton for loading
   - Alert for errors
```

---

### Key Takeaways

1. **Server-side pagination** — backend returns one page, DataGrid displays it
2. **`paginationMode="server"`** — tells DataGrid not to paginate client-side
3. **useUrlPagination** — persists page/pageSize in URL for bookmarking + back button
4. **0-indexed vs 1-indexed** — DataGrid is 0-based, backend is 1-based, convert with `+1`
5. **Three states** — loading (skeleton), error (alert), success (DataGrid)
6. **Column definitions** — declarative, with custom renderCell for chips/buttons
7. **Row click → navigate** — `onRowClick` goes to detail page
8. **Edit button stops propagation** — prevents row click from firing
9. **Dialogs as state** — `useState(false)` for create, `useState<Study | null>(null)` for edit
10. **refetchQueries** — after create/update mutation, refetch the list to show changes

---

**Lesson 20 done.** We've covered the core list page pattern. The CRUD dialogs (2-step stepper, react-hook-form, error handling) were already visible in this file. 

Next is **Lesson 21: Detail Pages** — how single-entity pages work with related data, assignment panels, and the DetailPageHeader component.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 3, Lesson 21: Detail Pages — Single Entity + Related Data

---

### The Thinking Process

> "User clicks a row in the studies table → goes to `/admin/studies/5`. Now I need to show all the details of study 5: its info, assigned sites, assigned examiners per site, and actions like assign/unassign."

Answer: **Detail pages** fetch a single entity with all its relations in ONE GraphQL query, then display them in sections.

---

### Let me show you the study detail page:

---

---

### The Detail Page Structure

Every detail page follows this layout:

```
┌─────────────────────────────────────────────────────────────┐
│  ← Studies                                      [History]   │
│  [PROT-001] COVID Vaccine Trial  [Active]                   │
│  Pfizer · Phase III                                         │
├─────────────────────────────────────────────────────────────┤
│  Study Details (Paper card)                                 │
│  Protocol ID: PROT-001  │  Sponsor: Pfizer  │  Phase: III  │
│  Start Date: 2024-01-01 │  End Date: 2024-12-31            │
│  Description: A phase III clinical trial...                 │
├─────────────────────────────────────────────────────────────┤
│  Assigned Sites (RelatedDataGrid)                           │
│  Code | Site Name | City | Country | Status | [Unassign]   │
│  SITE-001 | Apollo Hospital | Mumbai | India | Active       │
├─────────────────────────────────────────────────────────────┤
│  Assign a Site (Autocomplete picker)                        │
│  [Search site code or name...  ▼]  [Assign]               │
├─────────────────────────────────────────────────────────────┤
│  Examiner Assignment per Site (StudySitePanel)              │
│  ┌─ Apollo Hospital ─────────────────────────────────┐     │
│  │  ☑ Dr. Smith (GCP-CERT-001, expires 2025-06-15)  │     │
│  │  ☐ Dr. Jones (available)                          │     │
│  └───────────────────────────────────────────────────┘     │
├─────────────────────────────────────────────────────────────┤
│  All Study Examiners (union across sites)                   │
│  Code | Name | Specialty | Role | Status                    │
└─────────────────────────────────────────────────────────────┘
```

---

### Breaking Down the Key Patterns

#### Pattern 1: Fetch Single Entity with Relations

```typescript
// hooks/useStudy.ts
export function useStudy(id: string | undefined) {
  const { data, loading, error } = useQuery(GET_STUDY_QUERY, {
    variables: { id },
    skip: !id,  // Don't fetch if id is undefined
  });
  const study: Study | null = data?.getStudy ?? null;
  return { study, loading, error };
}
```

The `GET_STUDY_QUERY` fetches EVERYTHING in one request:
```graphql
query GetStudy($id: ID!) {
  getStudy(id: $id) {
    id protocolId title sponsor phase startDate endDate status description
    sites { id siteCode name city country status }
    examiners { id examinerCode name specialty role status }
    studySites {
      site { id siteCode name status }
      examiners { id name certificate { certificateId expiresOn } }
      availableExaminers { id name }
    }
  }
}
```

**One query, all the data.** This is GraphQL's strength — nested data in a single request.

#### Pattern 2: DetailPageHeader (Reusable)

```typescript
<DetailPageHeader
  backTo="/admin/studies"
  backLabel="Studies"
  title={study.title}
  status={study.status}
  badge={study.protocolId}
  subtitle={`${study.sponsor} · ${study.phase}`}
/>
```

Shows: back button + badge + title + status chip + subtitle. Used on ALL detail pages.

**`navigate(-1)` for back button** — goes to previous page in browser history. This preserves the exact pagination state the user was on (e.g., page 3 of studies).

#### Pattern 3: InfoField (Reusable Label + Value)

```typescript
<InfoField label="Protocol ID" value={study.protocolId} />
<InfoField label="Sponsor" value={study.sponsor} />
```

Simple component: uppercase label + value below. `value || '—'` shows a dash for empty fields.

#### Pattern 4: RelatedDataGrid (Reusable Related Data Table)

```typescript
<RelatedDataGrid
  title="Assigned Sites"
  rows={study.sites ?? []}
  columns={siteColumns}
  emptyMessage="No sites assigned to this study"
  emptySubMessage="Use the picker below to assign a site."
/>
```

Shows a title + count chip + DataGrid (or empty state if no data). Reused for sites, examiners, studies — any related entity list.

#### Pattern 5: Autocomplete Picker (Assign)

```typescript
<Autocomplete
  options={unassignedSites}
  value={selectedSite}
  onOpen={() => loadSites()}           // Lazy load: fetch all sites when dropdown opens
  onChange={(_, value) => setSelectedSite(value)}
  getOptionLabel={(o) => `${o.siteCode} — ${o.name}`}
  renderInput={(params) => <TextField {...params} placeholder="Search..." />}
/>
<Button onClick={handleAssignSite} disabled={!selectedSite}>Assign</Button>
```

**How it works:**
1. User opens the dropdown → `onOpen` triggers lazy fetch of all sites
2. Already-assigned sites are filtered out: `allSites.filter(s => !assignedSiteIds.has(s.id))`
3. User selects a site → `selectedSite` state updates
4. User clicks Assign → mutation fires → refetch study query → UI updates

#### Pattern 6: Completed Study Lock

```typescript
const isCompleted = study?.status === 'Completed';

{isCompleted && (
  <Alert severity="info" icon={<LockIcon />}>
    This study is Completed — assignments are locked.
  </Alert>
)}

{!isCompleted && (
  // Show assign picker + unassign buttons
)}
```

When a study is Completed:
- Lock banner shown
- Assign picker hidden
- Unassign buttons hidden
- StudySitePanel checkboxes disabled (`readOnly={isCompleted}`)

#### Pattern 7: Refetch After Mutation

```typescript
const refetchQuery = { query: GET_STUDY_QUERY, variables: { id } };
const [assignSite] = useMutation(ASSIGN_SITE_TO_STUDY, {
  refetchQueries: [refetchQuery],
});
```

After assigning a site, Apollo automatically re-runs `GET_STUDY_QUERY` → the page updates with the new site in the list. No manual state management needed.

---

### The Four States (Detail Pages)

```typescript
{loading && <DetailPageSkeleton infoFields={6} relatedSections={3} />}
{error && <Alert severity="error">{error.message}</Alert>}
{!loading && !error && !study && <Alert severity="warning">Study not found.</Alert>}
{!loading && !error && study && (
  // Render the actual content
)}
```

1. **Loading** → skeleton (placeholder shapes)
2. **Error** → red alert
3. **Not found** → yellow warning (valid ID but no data)
4. **Success** → render everything

---

### If You Were Building From Scratch

```
1. Create useStudy hook (single entity fetch)
   - useQuery with skip: !id

2. Create a basic detail page:
   - useParams() to get id
   - useStudy(id) to fetch data
   - Display basic fields (title, status, etc.)

3. Add DetailPageHeader (reusable):
   - Back button + title + status chip
   - Use on all detail pages

4. Add InfoField (reusable):
   - Label + value display

5. Add RelatedDataGrid (reusable):
   - Title + DataGrid or empty state

6. Add assignment functionality:
   - Autocomplete picker
   - Assign/Unassign mutations
   - refetchQueries to update UI

7. Add lock logic for terminal states:
   - isCompleted → hide actions, show banner
```

---

### Key Takeaways

1. **One query fetches everything** — entity + all relations in a single GraphQL request
2. **`skip: !id`** — don't fetch until we have the ID from URL params
3. **Four states** — loading, error, not found, success
4. **Reusable components** — DetailPageHeader, InfoField, RelatedDataGrid used across all detail pages
5. **`navigate(-1)`** — back button preserves list page pagination state
6. **Autocomplete picker** — lazy-loaded, filters out already-assigned items
7. **`refetchQueries`** — after mutation, re-fetch the detail query to update UI
8. **Lock pattern** — terminal status hides all action buttons/pickers
9. **StudySitePanel** — per-site examiner checkboxes (complex sub-component)
10. **History button** — links to `/admin/studies/:id/history` for audit trail

---

**Lesson 21 done.** We've now covered the major frontend patterns. Let me skip ahead to **Phase 4: Full Flows** where we trace complete user actions end-to-end.

Next is **Phase 4, Lesson 22: Login Flow (End to End)** — tracing a complete login from button click to dashboard render.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 4, Lesson 22: Login Flow — End to End

---

### The Thinking Process

Now we connect EVERYTHING. Let's trace a complete login from the moment the user clicks "Sign In" to the moment they see their dashboard. Every file, every function, every layer.

---

### The Complete Flow (Visual)

```
User clicks "Sign In"
  │
  ▼
LoginPage.tsx (react-hook-form validates email/password)
  │
  ▼
useLogin.ts hook → calls LOGIN_MUTATION
  │
  ▼
apolloClient.ts → httpLink sends POST to localhost:4040/graphql
  │                (credentials: 'include' → sends any existing cookies)
  ▼
═══════════════════════ NETWORK ═══════════════════════════════
  │
  ▼
app.ts → middleware chain (helmet → requestId → morgan → cors → json → cookieParser)
  │
  ▼
app.ts → loginRateLimit middleware (checks if too many attempts)
  │
  ▼
app.ts → Apollo Server context function (no auth_token cookie yet → user = null)
  │
  ▼
resolvers/auth.ts → login resolver
  │  1. parseOrThrow(loginSchema, { email, password })
  │  2. loginUser(email, password)
  │
  ▼
services/authService.ts → loginUser()
  │  1. findUserByEmail(email) → repository → DB
  │  2. verifyPassword(password, user.password) → bcrypt compare
  │  3. signToken({ userId, role, email }) → JWT (15 min)
  │  4. generateRefreshToken() → random 96-char hex
  │  5. hashToken(refreshToken) → SHA-256
  │  6. insertRefreshToken(userId, hash, expiresAt) → DB
  │
  ▼
resolvers/auth.ts → sets cookies on response
  │  setAccessCookie(res, accessToken)   → auth_token (HttpOnly, 15 min)
  │  setRefreshCookie(res, refreshToken) → refresh_token (HttpOnly, 7 days)
  │  return { user: { id, email, role } }
  │
  ▼
═══════════════════════ NETWORK ═══════════════════════════════
  │
  ▼
apolloClient.ts → receives response (browser stores cookies automatically)
  │
  ▼
useLogin.ts → receives { data: { login: { user: { role: 'ADMIN' } } } }
  │  1. client.refetchQueries({ include: [ME_QUERY] })
  │     → sends query { me { id email role } } with new auth_token cookie
  │     → backend verifies JWT → returns user
  │     → AuthContext updates: isLoggedIn=true, role='ADMIN'
  │  2. enqueueSnackbar('Signed in successfully.')
  │  3. navigate('/admin/dashboard')
  │
  ▼
React Router → matches /admin/dashboard
  │
  ▼
AdminRoute component
  │  useAuth() → { isLoggedIn: true, role: 'ADMIN' }
  │  role === 'ADMIN' ✅ → render children
  │
  ▼
AdminDashboardPage renders inside AdminLayout
  │  AdminLayout = AppHeader + AdminSidebar + main content
  │
  ▼
User sees the dashboard ✨
```

---

### Let me show you the LoginPage to complete the picture:

---

---

### Tracing Each Step in Detail

#### Step 1: User Fills Form + Clicks Submit

```typescript
// LoginPage.tsx
const { register, handleSubmit, setError, formState: { errors } } = useForm<LoginFormValues>({
  resolver: zodResolver(loginSchema),
  defaultValues: { email: 'viewer@test.com', password: 'password123' },
});
```

- Form pre-filled with viewer credentials (for demo convenience)
- `zodResolver(loginSchema)` validates before submit:
  - email must be valid email format
  - password must be non-empty
- If validation fails → errors show under fields instantly (no network request)
- If validation passes → `onSubmit` runs

#### Step 2: onSubmit Calls useLogin Hook

```typescript
async function onSubmit(values: LoginFormValues) {
  const errMsg = await submitLogin(values.email, values.password);
  if (errMsg) {
    setError('root', { message: errMsg });  // Shows error above the button
  }
}
```

- `submitLogin` returns `null` on success, error message string on failure
- `setError('root', ...)` shows a general error (not tied to a specific field)

#### Step 3: useLogin Sends the Mutation

```typescript
// useLogin.ts
const { data } = await loginMutation({ variables: { email, password } });
```

This sends:
```graphql
mutation Login($email: String!, $password: String!) {
  login(email: $email, password: $password) {
    user { id email role }
  }
}
```

#### Step 4: Backend Processes the Login

```
app.ts context: user = null (no cookie yet)
  → loginRateLimit: checks IP+email combo (20 attempts/15 min)
  → auth resolver: parseOrThrow(loginSchema, args)
  → authService.loginUser(email, password):
      findUserByEmail('admin@test.com') → { id:1, email:'admin@test.com', password:'$2a$10$...', role:'ADMIN' }
      verifyPassword('password123', '$2a$10$...') → true ✅
      signToken({ userId:1, role:'ADMIN', email:'admin@test.com' }) → 'eyJhbG...' (JWT)
      generateRefreshToken() → 'a3f7b2c1...' (96 chars)
      hashToken('a3f7b2c1...') → '7f83b165...' (SHA-256)
      insertRefreshToken(1, '7f83b165...', '2024-06-22T10:30:00Z') → saved to DB
  → auth resolver: setAccessCookie + setRefreshCookie
  → returns: { user: { id:1, email:'admin@test.com', role:'ADMIN' } }
```

#### Step 5: Browser Receives Response + Cookies

The HTTP response includes:
```
Set-Cookie: auth_token=eyJhbG...; HttpOnly; Path=/; Max-Age=900; SameSite=Lax
Set-Cookie: refresh_token=a3f7b2c1...; HttpOnly; Path=/; Max-Age=604800; SameSite=Lax
```

Browser stores these automatically. JavaScript can't read them (HttpOnly).

#### Step 6: useLogin Refetches ME_QUERY

```typescript
await client.refetchQueries({ include: [ME_QUERY] });
```

This sends:
```graphql
query Me { me { id email role } }
```

Now the `auth_token` cookie is included automatically. Backend verifies it:
```
context function: token = req.cookies.auth_token → verifyToken → { userId:1, role:'ADMIN', email:'...' }
  → context.user = { userId:1, role:'ADMIN', email:'...' }
  → me resolver: requireAuth(context) ✅ → getUserById(1) → returns user
```

AuthContext receives the response → updates:
```
isLoggedIn = true
role = 'ADMIN'
isChecking = false
```

#### Step 7: Navigate to Dashboard

```typescript
const role = data?.login?.user?.role;  // 'ADMIN'
navigate(role === 'ADMIN' ? '/admin/dashboard' : '/viewer/dashboard');
```

React Router renders `/admin/dashboard` → `AdminRoute` checks auth → passes → `AdminDashboardPage` renders.

---

### What Happens on Login FAILURE

```
User enters wrong password
  → Frontend Zod: passes (email format valid, password non-empty)
  → Mutation sent to backend
  → authService.loginUser:
      findUserByEmail('admin@test.com') → found
      verifyPassword('wrongpass', '$2a$10$...') → false ❌
      throw GraphQLError('Invalid credentials', { code: 'UNAUTHENTICATED' })
  → Response: { errors: [{ message: 'Invalid credentials', extensions: { code: 'UNAUTHENTICATED' } }] }
  → useLogin catches error:
      const { message } = parseGqlError(err);  // 'Invalid credentials'
      return message;
  → LoginPage: setError('root', { message: 'Invalid credentials' })
  → User sees: red Alert box with "Invalid credentials"
```

---

### What Happens on Rate Limit

```
User tries 21st login attempt within 15 minutes
  → Request hits loginRateLimit middleware
  → Middleware returns 429 status with:
      { errors: [{ message: 'Too many login attempts...', extensions: { code: 'RATE_LIMITED' } }] }
  → Apollo receives networkError with statusCode: 429
  → useLogin catches:
      const networkStatus = (err.networkError as { statusCode?: number })?.statusCode;
      if (networkStatus === 429) return 'Too many sign-in attempts...';
  → User sees: "Too many sign-in attempts for this account. Please wait 15 minutes."
```

---

### The Files Involved (In Order of Execution)

| # | File | Role |
|---|------|------|
| 1 | `frontend/src/pages/LoginPage.tsx` | Form UI + submit handler |
| 2 | `frontend/src/validation/authSchemas.ts` | Frontend Zod validation |
| 3 | `frontend/src/hooks/useLogin.ts` | Mutation + navigation logic |
| 4 | `frontend/src/services/authService.ts` | LOGIN_MUTATION definition |
| 5 | `frontend/src/utils/apolloClient.ts` | Sends HTTP request |
| 6 | `backend/src/app.ts` | Middleware chain + context |
| 7 | `backend/src/middleware/security.ts` | Rate limiting |
| 8 | `backend/src/graphql/resolvers/auth.ts` | Login resolver |
| 9 | `backend/src/validation/authSchemas.ts` | Backend Zod validation |
| 10 | `backend/src/services/authService.ts` | loginUser business logic |
| 11 | `backend/src/repositories/authRepository.ts` | findUserByEmail |
| 12 | `backend/src/utils/password.ts` | verifyPassword (bcrypt) |
| 13 | `backend/src/utils/jwt.ts` | signToken (JWT) |
| 14 | `backend/src/utils/token.ts` | generateRefreshToken + hashToken |
| 15 | `backend/src/repositories/refreshTokenRepository.ts` | insertRefreshToken |
| 16 | `frontend/src/contexts/AuthContext.tsx` | Updates isLoggedIn + role |
| 17 | `frontend/src/components/AdminRoute.tsx` | Allows access |
| 18 | `frontend/src/pages/admin/DashboardPage.tsx` | Renders dashboard |

**18 files touched in one login flow.** But each file does ONE thing. That's why the layered architecture works — you can trace any flow by following the chain.

---

### The Mental Model for Tracing ANY Flow

```
1. Start at the UI (which component? which button?)
2. Follow the hook/handler (what function runs on click?)
3. Find the mutation/query (what GraphQL operation is sent?)
4. Jump to the resolver (which resolver handles it?)
5. Follow the service (what business logic runs?)
6. Check the repository (what SQL executes?)
7. Trace back up (what does the resolver return?)
8. Back to the UI (how does the component update?)
```

This works for EVERY feature in the app. And in ANY codebase you'll ever work on.

---

### Key Takeaways

1. **18 files, one flow** — but each file has a single responsibility
2. **Frontend validates first** (instant UX), **backend validates second** (security)
3. **Cookies set by backend** — browser stores them automatically
4. **refetchQueries(ME_QUERY)** — updates AuthContext after login
5. **Role determines navigation** — ADMIN → /admin/dashboard, VIEWER → /viewer/dashboard
6. **Error handling at every level** — Zod, service, rate limit, network
7. **Rate limiting** — 20 attempts per 15 min per IP+email
8. **No token in JavaScript** — HttpOnly cookies, never in localStorage
9. **Trace the chain** — UI → hook → mutation → resolver → service → repository → DB → back
10. **Same pattern for every feature** — once you understand one flow, you understand all

---

**Lesson 22 done.** Next is **Lesson 23: Create Study Flow (End to End)** — tracing a complete CRUD operation from form submission to database write to UI update.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 4, Lesson 23: Create Study Flow — End to End

---

### The Complete Flow (Visual)

```
Admin clicks "+ New Study" button
  │
  ▼
CreateStudyDialog opens (2-step stepper)
  │  Step 1: Protocol ID, Title, Sponsor, Phase
  │  Step 2: Start Date, End Date, Description
  │
  ▼
User fills Step 1 → clicks "Next"
  │  trigger(['protocolId', 'title', 'sponsor', 'phase']) → validates only Step 1 fields
  │  If valid → setActiveStep(1)
  │
  ▼
User fills Step 2 → clicks "Create"
  │  handleSubmit(onSubmit) → Zod validates ALL fields (createStudySchema)
  │  Frontend checks: startDate ≥ today? endDate ≥ startDate?
  │  If invalid → errors show under fields, stays on form
  │  If valid → onSubmit runs
  │
  ▼
onSubmit: strips empty endDate, calls createStudy mutation
  │
  ▼
apolloClient → POST to /graphql (with auth_token cookie)
  │
  ▼
═══════════════════════ BACKEND ═══════════════════════════════
  │
  ▼
app.ts context: verifyToken(cookie) → user = { userId:1, role:'ADMIN', email:'admin@test.com' }
  │
  ▼
resolvers/study.ts → createStudy resolver
  │  1. requireAdmin(context) → role === 'ADMIN' ✅
  │  2. parseOrThrow(createStudySchema, input)
  │     → validates all fields
  │     → transforms protocolId: "prot-001" → "PROT-001"
  │     → checks date format, phase enum, etc.
  │  3. createStudy(validated) → service
  │
  ▼
services/studyService.ts → createStudy(input)
  │  1. todayUTC() → "2024-06-15"
  │  2. input.startDate < today? → throw BAD_USER_INPUT (D1)
  │  3. input.endDate < input.startDate? → throw BAD_USER_INPUT (D2)
  │  4. protocolIdExists(input.protocolId)? → throw BAD_USER_INPUT (S8)
  │  5. All rules pass → insertStudy(...)
  │
  ▼
repositories/studyRepository.ts → insertStudy(...)
  │  INSERT INTO studies (protocolId,title,sponsor,phase,startDate,endDate,status,description)
  │  VALUES ('PROT-001','COVID Trial','Pfizer','Phase III','2024-07-01','','Planned','...')
  │  → returns lastInsertRowid = 5
  │
  ▼
services/studyService.ts → findStudyById(5) → returns full StudyRow
  │
  ▼
resolvers/study.ts
  │  4. logAudit(context, 'CREATE', 'Study', 5, null, JSON.stringify(study))
  │     → insertAuditLog(1, 'admin@test.com', 'CREATE', 'Study', 5, null, '{"id":5,...}')
  │  5. return study
  │
  ▼
═══════════════════════ RESPONSE ══════════════════════════════
  │
  ▼
apolloClient receives: { data: { createStudy: { id:"5", title:"COVID Trial", status:"Planned", ... } } }
  │
  ▼
Apollo executes refetchQueries: [GET_STUDIES_QUERY]
  │  → re-fetches the studies list → DataGrid updates with new row
  │
  ▼
onSubmit success path:
  │  enqueueSnackbar('Study created successfully.', { variant: 'success' })
  │  handleClose() → reset form, setActiveStep(0), close dialog
  │
  ▼
User sees: ✅ success toast + new study in the table
```

---

### What Happens on FAILURE (Backend Rejects)

Let's say the protocol ID already exists:

```
User submits: { protocolId: "PROT-001", ... }
  │
  ▼
Frontend Zod: passes ✅ (format is valid)
  │
  ▼
Backend Zod (parseOrThrow): passes ✅ (transforms to "PROT-001")
  │
  ▼
Service: protocolIdExists("PROT-001") → true ❌
  │  throw new GraphQLError('Protocol ID already exists', {
  │    extensions: { code: 'BAD_USER_INPUT', fieldErrors: { protocolId: 'Protocol ID must be unique' } }
  │  })
  │
  ▼
═══════════════════════ RESPONSE ══════════════════════════════
  │
  ▼
apolloClient: error response
  │  errorLink: code is BAD_USER_INPUT → NOT handled globally (no toast)
  │
  ▼
onSubmit catch block:
  │  const { code, message, fieldErrors } = parseGqlError(err);
  │  // code = 'BAD_USER_INPUT'
  │  // fieldErrors = { protocolId: 'Protocol ID must be unique' }
  │
  │  Object.entries(fieldErrors).forEach(([field, msg]) => {
  │    setError(field as keyof CreateStudyFormValues, { message: msg });
  │  });
  │  // → protocolId field now shows red border + "Protocol ID must be unique"
  │
  │  // Navigate to the step containing the error:
  │  const step1Keys = ['protocolId', 'title', 'sponsor', 'phase'];
  │  if (errorKeys.some(k => step1Keys.includes(k))) setActiveStep(0);
  │  // → Dialog jumps back to Step 1 where protocolId is
  │
  │  enqueueSnackbar('Please correct the highlighted fields.', { variant: 'warning' });
  │
  ▼
User sees: ⚠️ warning toast + Step 1 with red error under Protocol ID
```

---

### The parseGqlError Utility

---

---

### The Error Bridge (Backend → Frontend Form Fields)

This is the key pattern that connects backend validation to frontend form UX:

```
Backend throws:
  GraphQLError('...', { extensions: { code: 'BAD_USER_INPUT', fieldErrors: { protocolId: '...' } } })
      │
      ▼
Network response:
  { errors: [{ message: '...', extensions: { code: 'BAD_USER_INPUT', fieldErrors: { protocolId: '...' } } }] }
      │
      ▼
Frontend parseGqlError(err):
  { code: 'BAD_USER_INPUT', message: '...', fieldErrors: { protocolId: 'Protocol ID must be unique' } }
      │
      ▼
Frontend setError('protocolId', { message: 'Protocol ID must be unique' }):
  → react-hook-form shows error under the protocolId TextField
```

**The field names MUST match between backend fieldErrors keys and frontend form field names.** That's why both use the same names: `protocolId`, `title`, `startDate`, etc.

---

### The 2-Step Stepper Pattern

```
Step 1 (Identity):          Step 2 (Schedule):
┌─────────────────────┐    ┌─────────────────────┐
│ ● Identity ○ Schedule│    │ ✓ Identity ● Schedule│
├─────────────────────┤    ├─────────────────────┤
│ Protocol ID: [____] │    │ Start Date: [____]  │
│ Title: [__________] │    │ End Date: [______]  │
│ Sponsor: [________] │    │ Status: [Planned]   │
│ Phase: [Phase II ▼] │    │ Description: [____] │
├─────────────────────┤    ├─────────────────────┤
│ [Cancel]     [Next] │    │ [Cancel] [Back] [Create] │
└─────────────────────┘    └─────────────────────┘
```

**Why 2 steps?**
- Reduces cognitive load (fewer fields visible at once)
- Groups related fields (identity vs schedule)
- Step validation: can't proceed to Step 2 with invalid Step 1 fields

**Step validation:**
```typescript
async function handleNext() {
  const step1Fields: (keyof CreateStudyFormValues)[] = ['protocolId', 'title', 'sponsor', 'phase'];
  const valid = await trigger(step1Fields);  // Validate ONLY these fields
  if (valid) setActiveStep(1);
}
```

`trigger(fields)` validates specific fields without submitting the form. If any fail, errors show and the user stays on Step 1.

---

### The Mutation Definition

---

---

### All Mutations in One File (adminService.ts)

Notice: **ALL mutations live in `adminService.ts`**. This is a design decision:
- Queries live in domain service files (`studyService.ts`, `siteService.ts`)
- Mutations ALL live in `adminService.ts`

**Why?** Only admins can mutate. Keeping all mutations in one file makes it easy to audit "what can admins do?" — just read one file.

---

### The refetchQueries Pattern

```typescript
const [createStudy] = useMutation(CREATE_STUDY_MUTATION, {
  refetchQueries: [GET_STUDIES_QUERY],
});
```

After the mutation succeeds, Apollo automatically re-runs `GET_STUDIES_QUERY`. This means:
- The studies list page will show the new study
- No manual state management needed
- The cache is always fresh

**Alternative: cache update** — you could manually add the new study to the cache. But `refetchQueries` is simpler and guarantees consistency with the server.

---

### The Files Involved (Create Study)

| # | File | What Happens |
|---|------|-------------|
| 1 | `pages/admin/StudiesPage.tsx` | CreateStudyDialog renders |
| 2 | `validation/studySchemas.ts` (frontend) | Zod validates form fields |
| 3 | `services/adminService.ts` | CREATE_STUDY_MUTATION definition |
| 4 | `utils/apolloClient.ts` | Sends request with cookie |
| 5 | `app.ts` | Middleware + context (extracts user from JWT) |
| 6 | `resolvers/study.ts` | requireAdmin + parseOrThrow + calls service + logAudit |
| 7 | `validation/studySchemas.ts` (backend) | Zod validates + transforms |
| 8 | `services/studyService.ts` | Business rules (D1, D2, S8) |
| 9 | `repositories/studyRepository.ts` | INSERT SQL |
| 10 | `repositories/auditRepository.ts` | INSERT audit log |
| 11 | `utils/gqlErrors.ts` | Parses error on failure |
| 12 | `services/studyService.ts` (query) | GET_STUDIES_QUERY refetch |

---

### The Same Pattern for Sites and Examiners

Every CRUD operation follows the EXACT same pattern:

```
Dialog (2-step stepper)
  → react-hook-form + zodResolver (frontend validation)
  → useMutation (send to backend)
  → resolver: requireAdmin → parseOrThrow → service → logAudit
  → service: business rules → repository: SQL
  → success: refetchQueries + toast + close dialog
  → failure: parseGqlError → setError on fields → navigate to error step
```

The only differences are:
- Which fields are in the form
- Which Zod schema validates
- Which business rules apply
- Which table gets the INSERT

---

### Key Takeaways

1. **2-step stepper** — reduces cognitive load, validates per-step with `trigger()`
2. **Frontend Zod** — instant validation (format, required fields, date logic)
3. **Backend Zod** — authoritative validation + transforms (trim, uppercase)
4. **Service rules** — business logic (uniqueness, date constraints)
5. **fieldErrors bridge** — backend error keys match frontend form field names
6. **Step navigation on error** — dialog jumps to the step containing the error
7. **refetchQueries** — auto-refreshes the list after successful create
8. **All mutations in adminService.ts** — single source of truth for write operations
9. **Status hardcoded** — createStudy always sets "Planned" (not user-controlled)
10. **Audit logged** — every create is recorded with afterJson snapshot

---

**Lesson 23 done.** Next is **Lesson 24: Assignment Flow (End to End)** — tracing how assigning a site to a study works, including the domain rules that can reject it.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 4, Lesson 24: Assignment Flow — Assign Site to Study (End to End)

---

### The Complete Flow (Visual)

```
Admin is on Study Detail Page (/admin/studies/5)
  │
  ▼
Opens Autocomplete picker → types "Apollo"
  │  onOpen → useSitesPickerLazy().load() → fetches all sites (pageSize:1000)
  │  Filters out already-assigned sites
  │  Shows: "SITE-003 — Apollo Hospital"
  │
  ▼
Selects "Apollo Hospital" → clicks "Assign"
  │
  ▼
handleAssignSite() runs
  │  assignSite({ variables: { studyId: "5", siteId: "3" } })
  │
  ▼
apolloClient → POST to /graphql (with auth_token cookie)
  │
  ▼
═══════════════════════ BACKEND ═══════════════════════════════
  │
  ▼
resolvers/study.ts → assignSiteToStudy resolver
  │  1. requireAdmin(context) → ✅
  │  2. parseOrThrow(assignmentSchema, { studyId: "5", siteId: "3" })
  │     → validates both are numeric strings ✅
  │  3. assignSiteToStudy(5, 3) → service
  │
  ▼
services/studyService.ts → assignSiteToStudy(studyId=5, siteId=3)
  │  1. findStudyById(5) → exists ✅
  │  2. findSiteForStudy(3) → { id:3, status:'Active', name:'Apollo Hospital' }
  │  3. site.status !== 'Active'? → status IS 'Active' ✅ (SI1 passes)
  │  4. insertStudySite(5, 3) → repository
  │
  ▼
repositories/studyRepository.ts → insertStudySite(5, 3)
  │  INSERT OR IGNORE INTO study_sites (study_id, site_id) VALUES (5, 3)
  │
  ▼
resolvers/study.ts
  │  4. logAudit(context, 'ASSIGN', 'StudySite', 5, null, '{"studyId":5,"siteId":3}')
  │  5. return true
  │
  ▼
═══════════════════════ RESPONSE ══════════════════════════════
  │
  ▼
Apollo executes refetchQueries: [GET_STUDY_QUERY with id:"5"]
  │  → re-fetches study with all relations
  │  → DataGrid now shows Apollo Hospital in "Assigned Sites"
  │
  ▼
handleAssignSite success:
  │  enqueueSnackbar('Apollo Hospital assigned to study.', { variant: 'success' })
  │  setSelectedSite(null) → clears the picker
  │
  ▼
User sees: ✅ toast + new site in the table + site removed from picker options
```

---

### What Happens When Assignment FAILS

#### Scenario 1: Site is not Active (SI1)

```
Admin tries to assign a "Planned" site
  │
  ▼
Service: site.status !== 'Active' → status is 'Planned' ❌
  │  throw GraphQLError('Cannot assign a Planned site to a study. Only Active sites can be assigned.', {
  │    extensions: { code: 'BAD_USER_INPUT', fieldErrors: { siteId: 'Site is Planned. Only Active sites...' } }
  │  })
  │
  ▼
Frontend catch:
  │  const { message } = parseGqlError(err);
  │  enqueueSnackbar(message || 'Failed to assign site.', { variant: 'error' })
  │
  ▼
User sees: ❌ error toast "Cannot assign a Planned site to a study..."
```

#### Scenario 2: Study is Active + trying to unassign (D9)

```
Admin tries to unassign a site from an Active study
  │
  ▼
Service: STRICT_NO_SITE_UNASSIGN_WHEN_STUDY_ACTIVE && study.status === 'Active' ❌
  │  throw GraphQLError('Cannot unassign a site from an Active study.')
  │
  ▼
User sees: ❌ error toast
```

#### Scenario 3: Site has SSE rows (SI2)

```
Admin tries to unassign a site that has examiners assigned to it for this study
  │
  ▼
Service: countSSEForStudySite(5, 3) > 0 ❌
  │  throw GraphQLError('Cannot unassign this site: it has examiner assignments...')
  │
  ▼
User sees: ❌ error toast "Remove those study assignments first."
```

---

### The Unassign Flow

```
Admin clicks "Unassign" button next to a site
  │
  ▼
handleUnassignSite(siteId="3", siteName="Apollo Hospital")
  │  1. isCompleted? → show warning toast, return (lock check)
  │  2. unassignSite({ variables: { studyId: "5", siteId: "3" } })
  │
  ▼
Backend:
  │  resolver: requireAdmin → parseOrThrow → unassignSiteFromStudy(5, 3)
  │  service:
  │    - study.status === 'Active'? → blocked (D9)
  │    - countSSEForStudySite(5, 3) > 0? → blocked (SI2)
  │    - All clear → deleteStudySite(5, 3)
  │  resolver: logAudit('UNASSIGN', 'StudySite', 5, '{"studyId":5,"siteId":3}', null)
  │
  ▼
Frontend:
  │  refetchQueries → site disappears from table
  │  enqueueSnackbar('Apollo Hospital unassigned from study.', { variant: 'info' })
```

---

### The Picker Pattern (Lazy Loading)

---

---

### Lazy vs Eager Loading

```typescript
// Eager: fetches immediately when component mounts
const { sites } = useSitesPicker();

// Lazy: fetches only when you call load()
const { load, sites } = useSitesPickerLazy();
// Used with: onOpen={() => load()}
```

**Why lazy for the picker?**
- The study detail page might have 100 sites in the database
- No point fetching them until the user actually opens the dropdown
- `onOpen={() => loadSites()}` triggers the fetch only when needed

**Why pageSize: 1000?**
- Pickers need ALL options for autocomplete to work (client-side filtering)
- 1000 is the max allowed by `pickerPaginationSchema`
- For most apps, you won't have more than 1000 sites

---

### Filtering Out Already-Assigned Sites

```typescript
const assignedSiteIds = new Set((study?.sites ?? []).map((s) => s.id));
const unassignedSites = allSites.filter((s) => !assignedSiteIds.has(s.id));
```

**What this does:**
1. Get IDs of sites already assigned to this study
2. Filter the full site list to show only unassigned ones
3. User can only pick from sites NOT already assigned

This is client-side filtering — simple and fast since we have all sites loaded.

---

### The SSE Assignment Flow (More Complex)

Now let's trace the 3-way assignment: assigning an examiner to a study at a specific site.

---

---

### The SSE Assignment Flow (Checkbox Toggle)

```
Admin checks the checkbox next to "Dr. Smith" at "Apollo Hospital"
  │
  ▼
handleToggle(examiner=DrSmith, currentlyAssigned=false)
  │  1. readOnly? → No (study not Completed)
  │  2. currentlyAssigned? → No (assigning, not unassigning)
  │  3. Does examiner have valid certificates?
  │     → validCerts = examiner.certificates.filter(c => isCertValid(c.expiresOn))
  │
  ▼
IF validCerts.length >= 1:
  │  setCertPickerExaminer(examiner) → opens CertificatePickerDialog
  │  User selects a certificate → handleCertSelected(certId)
  │  → doAssign(examinerId, certId)
  │
IF validCerts.length === 0:
  │  → doAssign(examinerId) → backend auto-selects or rejects
  │
  ▼
doAssign(examinerId="7", certificateId="12")
  │  assignExaminer({ variables: { studyId:"5", siteId:"3", examinerId:"7", certificateId:"12" } })
  │
  ▼
═══════════════════════ BACKEND ═══════════════════════════════
  │
  ▼
resolvers/study.ts → assignExaminerToStudySite resolver
  │  1. requireAdmin ✅
  │  2. parseOrThrow(studySiteExaminerSchema, { studyId, siteId, examinerId, certificateId })
  │  3. assignExaminerToStudySite(5, 3, 7, 12) → service
  │
  ▼
services/studyService.ts → assignExaminerToStudySite(5, 3, 7, 12)
  │  SI5a: studySiteExists(5, 3)? → Yes ✅ (site is assigned to study)
  │  SI5b: site.status === 'Closed'? → No ✅ (site is Active)
  │  SI5c: siteExaminerExists(3, 7)? → Yes ✅ (examiner is assigned to site)
  │  
  │  certificateId provided (12):
  │    SI7: getCertificateById(12) → { id:12, examiner_id:7, expiresOn:'2025-06-15' }
  │    cert.examiner_id !== examinerId? → 7 === 7 ✅ (belongs to this examiner)
  │    cert.expiresOn < today? → '2025-06-15' >= '2024-06-15' ✅ (not expired)
  │    resolvedCertId = 12
  │  
  │  insertSSE(5, 3, 7, 12) → repository
  │
  ▼
repositories/studyRepository.ts → insertSSE(5, 3, 7, 12)
  │  INSERT OR IGNORE INTO study_site_examiners (study_id, site_id, examiner_id, certificate_id)
  │  VALUES (5, 3, 7, 12)
  │
  ▼
resolvers/study.ts
  │  logAudit('ASSIGN', 'StudySiteExaminer', 5, null, '{"studyId":5,"siteId":3,"examinerId":7,"certificateId":12}')
  │  return true
  │
  ▼
═══════════════════════ RESPONSE ══════════════════════════════
  │
  ▼
refetchQueries → GET_STUDY_QUERY re-runs
  │  → studySites now includes Dr. Smith with certificate info
  │  → Checkbox shows as checked ✅
  │  → Certificate info displayed: "Cert: GCP-CERT-001 (exp 2025-06-15)"
  │
  ▼
User sees: ✅ toast + checkbox checked + certificate info shown
```

---

### The Certificate Picker Dialog

```
┌─────────────────────────────────────────────┐
│  Select Certificate for Dr. Smith           │
├─────────────────────────────────────────────┤
│  ○ GCP-CERT-001 (expires 2025-06-15) ✓ Valid│
│  ○ GCP-CERT-003 (expires 2025-12-01) ✓ Valid│
├─────────────────────────────────────────────┤
│  [Cancel]                    [Select]       │
└─────────────────────────────────────────────┘
```

**When does it appear?**
- Examiner has ≥1 valid certificate
- User needs to choose which one to link to this assignment

**When does it NOT appear?**
- Examiner has 0 valid certificates → backend rejects with error
- (In theory, if examiner had exactly 1 valid cert, you could auto-select — but the UI always shows the picker for transparency)

---

### The Prerequisites Chain (SI5)

For an SSE assignment to succeed, ALL of these must be true:

```
1. Site must be assigned to the study (study_sites table)
   └── SI5a: studySiteExists(studyId, siteId)

2. Site must not be Closed
   └── SI5b: site.status !== 'Closed'

3. Examiner must be assigned to the site (site_examiners table)
   └── SI5c: siteExaminerExists(siteId, examinerId)

4. Examiner must have a valid certificate
   └── SI7: explicit cert validated OR auto-selected from valid certs
```

**This is why the UI shows only "available examiners" (those already on the site).** The frontend pre-filters to prevent impossible selections.

---

### If You Were Building From Scratch

```
1. Start with simple assign/unassign (study ↔ site):
   - Autocomplete picker
   - Assign mutation
   - Unassign button
   - refetchQueries

2. Add domain rules one by one:
   - SI1: only Active sites
   - D9: can't unassign from Active study
   - SI2: can't unassign if SSE exists

3. Then build SSE (3-way assignment):
   - StudySitePanel with checkboxes
   - handleToggle logic
   - Certificate picker dialog

4. Add certificate validation:
   - SI7: check cert ownership + expiry
   - Auto-select if only one valid cert
   - Show picker if multiple

5. Add lock for Completed studies:
   - readOnly prop
   - Disable checkboxes
   - Show lock banner
```

---

### Key Takeaways

1. **Autocomplete picker** — lazy-loaded, filters out already-assigned items
2. **INSERT OR IGNORE** — idempotent assignment (safe to call twice)
3. **Domain rules enforced in service** — SI1, SI2, SI5, SI7, D9
4. **Certificate picker** — shown when examiner has valid certs to choose from
5. **3-way junction (SSE)** — study + site + examiner + certificate linked together
6. **Prerequisites chain** — site→study, examiner→site, cert→examiner all must exist
7. **refetchQueries** — UI updates automatically after mutation
8. **readOnly prop** — Completed studies disable all assignment actions
9. **Error handling** — toast for failures, field-level errors where applicable
10. **Audit logged** — ASSIGN/UNASSIGN with full relationship JSON

---

**Lesson 24 done.** Next is **Lesson 25: Token Refresh Flow** — what happens when the access token expires mid-session and how the app seamlessly refreshes it.

Say **"next"** to continue, or let me know if you want to jump to a different topic. We've covered the major flows — the remaining lessons (refresh, search, testing, build order) follow the same tracing pattern.

---

next

---


## Phase 4, Lesson 25: Token Refresh Flow — Seamless Session Extension

---

### The Thinking Process

> "User has been working for 16 minutes. Their access token (15 min) expired. They click something. What happens? Do they get kicked to login? No — the app silently refreshes the token and retries their request."

This is the most elegant flow in the app — the user NEVER notices it happening.

---

### The Complete Flow (Visual)

```
Time 0:00 — User logged in. Access token expires at 0:15. Refresh token expires at Day 7.

Time 0:16 — User clicks "Studies" in sidebar
  │
  ▼
useStudies hook → useQuery(GET_STUDIES_QUERY)
  │  Apollo sends request with expired auth_token cookie
  │
  ▼
═══════════════════════ BACKEND ═══════════════════════════════
  │
  ▼
app.ts context function:
  │  token = req.cookies.auth_token → verifyToken(token)
  │  → jwt.verify throws (token expired)
  │  → returns null
  │  context.user = null
  │
  ▼
resolvers/study.ts → getStudies resolver:
  │  requireAuth(context) → context.user is null ❌
  │  throw GraphQLError('Unauthorized', { code: 'UNAUTHENTICATED' })
  │
  ▼
═══════════════════════ RESPONSE ══════════════════════════════
  │  { errors: [{ message: 'Unauthorized', extensions: { code: 'UNAUTHENTICATED' } }] }
  │
  ▼
apolloClient.ts → errorLink catches the error
  │
  ▼
errorLink logic:
  │  code === 'UNAUTHENTICATED'? → Yes
  │  onLoginPage? → No (we're on /admin/studies)
  │  isRefreshOp? → No (operation is GetStudies, not RefreshSession)
  │  → Attempt refresh!
  │
  ▼
return new Observable((observer) => {
  │  doRefresh().then((success) => { ... })
  │
  ▼
doRefresh():
  │  refreshPromise already exists? → No (first refresh attempt)
  │  → Create new promise:
  │     apolloClient.mutate({ mutation: REFRESH_SESSION_MUTATION })
  │
  ▼
═══════════════════════ REFRESH REQUEST ═══════════════════════
  │  mutation RefreshSession { refreshSession }
  │  (browser sends refresh_token cookie automatically)
  │
  ▼
app.ts context: user = null (no valid access token, but that's okay)
  │
  ▼
resolvers/auth.ts → refreshSession resolver:
  │  rawRefresh = req.cookies.refresh_token → "a3f7b2c1..."
  │  rawRefresh exists? → Yes
  │  → refreshSession(rawRefresh) → service
  │
  ▼
services/authService.ts → refreshSession("a3f7b2c1..."):
  │  1. hashToken("a3f7b2c1...") → "7f83b165..."
  │  2. findRefreshToken("7f83b165...") → row found
  │  3. row.revoked_at !== null? → null ✅ (not revoked)
  │  4. new Date(row.expires_at) <= new Date()? → No ✅ (not expired, 7 days)
  │  5. findUserById(row.user_id) → user found ✅
  │  6. ROTATION:
  │     - createRefreshTokenRecord(userId) → new token + hash + expiry
  │     - revokeRefreshToken(oldHash, newHash) → old token marked revoked
  │  7. signToken({ userId, role, email }) → new access token (fresh 15 min)
  │  8. return { accessToken, refreshToken, refreshExpiresAt }
  │
  ▼
resolvers/auth.ts:
  │  setAccessCookie(res, result.accessToken)   → new auth_token (15 min)
  │  setRefreshCookie(res, result.refreshToken) → new refresh_token (7 days)
  │  return true
  │
  ▼
═══════════════════════ REFRESH RESPONSE ══════════════════════
  │  { data: { refreshSession: true } }
  │  + Set-Cookie: auth_token=NEW_JWT; HttpOnly; Max-Age=900
  │  + Set-Cookie: refresh_token=NEW_RANDOM; HttpOnly; Max-Age=604800
  │
  ▼
doRefresh() resolves → success = true
  │
  ▼
errorLink Observable:
  │  success? → Yes!
  │  → forward(operation).subscribe(observer)
  │  → RETRY the original GetStudies query (now with fresh cookie)
  │
  ▼
═══════════════════════ RETRY REQUEST ═════════════════════════
  │  query GetStudies { ... }
  │  (browser sends NEW auth_token cookie)
  │
  ▼
app.ts context: verifyToken(newToken) → user = { userId:1, role:'ADMIN' } ✅
  │
  ▼
resolvers/study.ts → getStudies:
  │  requireAuth(context) → ✅
  │  → returns studies data
  │
  ▼
═══════════════════════ FINAL RESPONSE ════════════════════════
  │  { data: { getStudies: { rows: [...], total: 42 } } }
  │
  ▼
useStudies hook receives data → component re-renders → user sees studies list
  │
  ▼
User never noticed anything happened ✨
Total time: ~100-200ms (imperceptible)
```

---

### The Concurrent Request Problem (And Solution)

**Problem:** What if 5 queries fire at the same time and ALL get UNAUTHENTICATED?

```
Without single-promise pattern:
  Query 1 → UNAUTHENTICATED → refresh attempt 1
  Query 2 → UNAUTHENTICATED → refresh attempt 2
  Query 3 → UNAUTHENTICATED → refresh attempt 3
  = 3 refresh requests! Token rotation means only the FIRST succeeds.
  The other 2 use an already-revoked token → fail → user gets kicked to login!
```

**Solution: Single in-flight promise**

```typescript
let refreshPromise: Promise<boolean> | null = null;

function doRefresh(): Promise<boolean> {
  if (refreshPromise) return refreshPromise;  // ← All concurrent callers share ONE promise
  
  refreshPromise = apolloClient.mutate({ mutation: REFRESH_SESSION_MUTATION })
    .then(({ data }) => !!(data?.refreshSession))
    .catch(() => false)
    .finally(() => { refreshPromise = null; });  // ← Reset after completion
  
  return refreshPromise;
}
```

```
With single-promise pattern:
  Query 1 → UNAUTHENTICATED → doRefresh() → creates promise → sends refresh
  Query 2 → UNAUTHENTICATED → doRefresh() → returns SAME promise (no new request)
  Query 3 → UNAUTHENTICATED → doRefresh() → returns SAME promise (no new request)
  
  Refresh succeeds → all 3 queries retry with new token → all succeed ✅
```

---

### What Happens When Refresh FAILS

#### Scenario 1: Refresh token expired (after 7 days)

```
doRefresh() → sends refreshSession mutation
  → Backend: row.expires_at <= now → return null
  → Resolver: clearAuthCookies, return false
  → Response: { data: { refreshSession: false } }
  → doRefresh() resolves with false
  → errorLink: success = false → redirectToLogin()
  → apolloClient.clearStore() → window.location.href = '/login'
  → User sees login page
```

#### Scenario 2: Refresh token was revoked (security event)

```
doRefresh() → sends refreshSession mutation
  → Backend: row.revoked_at !== null → return null
  → Same as above → user redirected to login
```

#### Scenario 3: Refresh token is garbage/tampered

```
doRefresh() → sends refreshSession mutation
  → Backend: findRefreshToken(hash) → null (not found)
  → Same as above → user redirected to login
```

#### Scenario 4: RefreshSession itself returns UNAUTHENTICATED

```
errorLink catches UNAUTHENTICATED for RefreshSession operation
  → isRefreshOp = operation.operationName === 'RefreshSession' → true
  → Don't try to refresh again (infinite loop!)
  → redirectToLogin()
```

---

### The Infinite Loop Prevention

```typescript
// Never try to refresh the refreshSession mutation itself
const isRefreshOp = operation.operationName === 'RefreshSession';
if (isRefreshOp) {
  redirectToLogin();  // Give up, go to login
  return;
}
```

Without this check:
```
refreshSession fails with UNAUTHENTICATED
  → errorLink: "Oh, UNAUTHENTICATED! Let me refresh!"
  → calls refreshSession again
  → fails again with UNAUTHENTICATED
  → errorLink: "Oh, UNAUTHENTICATED! Let me refresh!"
  → infinite loop 💀
```

---

### Token Rotation Security

```
Before refresh:
  DB: { token_hash: "abc123", revoked_at: null, replaced_by: null }

After refresh:
  DB: { token_hash: "abc123", revoked_at: "2024-06-15T10:30:00", replaced_by: "def456" }  ← OLD (revoked)
  DB: { token_hash: "def456", revoked_at: null, replaced_by: null }  ← NEW (active)
```

**Why rotate?**
- If an attacker steals the old refresh token and tries to use it → it's revoked → rejected
- The `replaced_by_token_hash` creates an audit chain: you can trace token lineage
- Each refresh gives a fresh 7-day window (sliding expiration)

---

### The Login Page Exception

```typescript
const onLoginPage = window.location.pathname === '/login';
if (onLoginPage) return;  // Don't try to refresh on the login page
```

**Why?** On the login page, getting UNAUTHENTICATED is EXPECTED (user hasn't logged in yet). Trying to refresh would be pointless and could cause confusing behavior.

---

### The redirectToLogin Function

```typescript
function redirectToLogin() {
  apolloClient.clearStore().finally(() => {
    window.location.href = '/login';
  });
}
```

**Why `clearStore()` before redirect?**
- Removes all cached data from Apollo
- Prevents the next user from seeing the previous user's data
- `window.location.href` (not `navigate()`) forces a full page reload — ensures clean state

---

### Timeline of a Long Session

```
0:00  — Login. Access: 15min. Refresh: 7 days.
0:15  — Access expires. Next request triggers refresh. New access: 15min.
0:30  — Access expires again. Refresh again. New access: 15min.
...
Day 6, 23:45 — Access expires. Refresh succeeds (refresh token still valid).
Day 7, 0:00  — Refresh token expires. Next refresh attempt fails.
Day 7, 0:00  — User redirected to login. Must re-authenticate.
```

**Effective session length: 7 days of activity.** As long as the user uses the app at least once every 7 days, they stay logged in.

---

### If You Were Building From Scratch

```
1. Start WITHOUT refresh tokens:
   - Just access token (15 min)
   - When it expires → redirect to login
   - This works! Just annoying for users.

2. Add refresh token (backend):
   - generateRefreshToken + hashToken utilities
   - refresh_tokens table
   - refreshSession service function
   - refreshSession resolver

3. Add refresh token (frontend):
   - REFRESH_SESSION_MUTATION
   - errorLink: catch UNAUTHENTICATED → call refreshSession → retry
   - Single-promise pattern for concurrent requests

4. Add rotation:
   - revokeRefreshToken(oldHash, newHash)
   - replaced_by_token_hash column

5. Add edge cases:
   - Don't refresh on login page
   - Don't refresh the refresh operation itself
   - clearStore before redirect
```

---

### Key Takeaways

1. **Seamless to user** — token refresh + retry happens in ~100ms, invisible
2. **Single in-flight promise** — prevents concurrent refresh storms
3. **Token rotation** — old token revoked, new one issued, audit chain preserved
4. **Infinite loop prevention** — never refresh the refresh operation itself
5. **Login page exception** — UNAUTHENTICATED is expected there
6. **clearStore before redirect** — no stale data for next user
7. **7-day sliding window** — refresh token renews on each use
8. **SHA-256 hashing** — raw tokens never stored in DB
9. **Three failure modes** — expired, revoked, not found → all redirect to login
10. **Build incrementally** — basic JWT first, add refresh later

---

**Lesson 25 done.** Next is **Lesson 26: Search Flow** — how debounced search works with lazy queries and filter-only mode.

Say **"next"** to continue, or would you like me to jump to **Phase 5 (Build Order + Testing)** since we've covered all the major flows?

---

next

---

## Phase 4, Lesson 26: Search Flow — Debounced + Lazy Query + Filters

---

### The Thinking Process

> "I need a search page where users can type a keyword and find studies, sites, or examiners. But I can't send a request on every keystroke — that would flood the server. And I need filters (by entity type, phase, country, etc.)."

Answer: **Debounced input** (wait 400ms after user stops typing) + **useLazyQuery** (only fires when triggered) + **filters** that can work with or without a keyword.

---

### Let me show you the search page:

---

---

### The Debounce Pattern (Core Concept)

```typescript
useEffect(() => {
  if (debounceRef.current) clearTimeout(debounceRef.current);  // Cancel previous timer

  const trimmed = keyword.trim();

  // Rule 2: filter-only (no keyword) → fire immediately
  if (trimmed.length === 0) {
    if (hasActiveFilter) fireSearch('');
    return;
  }

  // Rule 1: keyword too short → don't search
  if (trimmed.length < MIN_KEYWORD_LENGTH) return;

  // Rule 1: keyword valid → wait 400ms then search
  debounceRef.current = setTimeout(() => {
    fireSearch(trimmed);
  }, DEBOUNCE_MS);

  return () => { if (debounceRef.current) clearTimeout(debounceRef.current); };
}, [keyword, entityType, studyStatus, studyPhase, siteCity, siteCountry, examinerRole]);
```

**What debouncing does:**

Without debounce:
```
User types "COVID"
  → "C" → search fires
  → "CO" → search fires
  → "COV" → search fires
  → "COVI" → search fires
  → "COVID" → search fires
  = 5 requests! Wasteful.
```

With 400ms debounce:
```
User types "COVID" (takes ~300ms total)
  → "C" → timer starts (400ms)
  → "CO" → timer RESET (400ms from now)
  → "COV" → timer RESET
  → "COVI" → timer RESET
  → "COVID" → timer RESET
  → 400ms passes with no more typing...
  → search fires ONCE with "COVID"
  = 1 request! Efficient.
```

---

### The Three Search Modes

| Mode | Keyword | Filters | What happens |
|------|---------|---------|-------------|
| **Idle** | empty | none | Show placeholder, no query |
| **Keyword search** | ≥2 chars | optional | Debounce 400ms, then search |
| **Filter-only** | empty | ≥1 active | Fire immediately, send `%%` as keyword |

**The `%%` trick:**
```typescript
keyword: kw || '%%',  // Empty keyword → send '%%'
```

Backend requires keyword ≥ 2 chars. `%%` satisfies this and in SQL `LIKE '%%%%'` matches everything. So filter-only search returns all records matching the filters.

---

### The Backend Search

---


---

### The Complete Search Flow

```
User types "COVID" with entityType="Study" and studyPhase="Phase III"
  │
  ▼
useEffect fires → debounce 400ms → fireSearch("COVID")
  │  builds filters: { entityType: "Study", studyPhase: "Phase III" }
  │  runSearch({ variables: { keyword: "COVID", filters: {...} } })
  │
  ▼
═══════════════════════ BACKEND ═══════════════════════════════
  │
  ▼
search resolver:
  │  requireAuth(context) ✅
  │  parseOrThrow(searchSchema, { keyword: "COVID", filters }) ✅ (≥2 chars)
  │  globalSearch("COVID", { entityType: "Study", studyPhase: "Phase III" })
  │
  ▼
searchService.ts → globalSearch:
  │  kw = "%covid%"  (lowercase + wrapped in %)
  │  entityType = "Study" → only search studies (skip sites, examiners)
  │  searchStudies("%covid%", undefined, "Phase III")
  │
  ▼
searchRepository.ts → searchStudies:
  │  SQL: SELECT * FROM studies 
  │       WHERE (LOWER(title) LIKE '%covid%' OR LOWER(sponsor) LIKE '%covid%' OR LOWER(protocolId) LIKE '%covid%')
  │       AND phase = 'Phase III'
  │       ORDER BY id ASC
  │  → Returns matching rows
  │
  ▼
Response: { studies: [{id:5, title:"COVID Vaccine Trial", phase:"Phase III", ...}], sites: [], examiners: [] }
  │
  ▼
═══════════════════════ FRONTEND ══════════════════════════════
  │
  ▼
results render:
  │  studyCount = 1, siteCount = 0, examCount = 0
  │  "1 result for "COVID""
  │  Shows study card: "COVID Vaccine Trial" [PROT-001 · Pfizer · Phase III] [Active]
  │  Click → navigate('/admin/studies/5')
```

---

### The Shared Component Pattern

```typescript
// SearchPage accepts layout + baseRoute props
interface SearchPageProps {
  layout: (children: ReactNode) => ReactNode;
  baseRoute: '/admin' | '/viewer';
}
```

**Used by both admin and viewer:**
```typescript
// pages/admin/SearchPage.tsx
export function AdminSearchPage() {
  return <SearchPage layout={(c) => <AdminLayout>{c}</AdminLayout>} baseRoute="/admin" />;
}

// pages/viewer/SearchPage.tsx
export function ViewerSearchPage() {
  return <SearchPage layout={(c) => <ViewerLayout>{c}</ViewerLayout>} baseRoute="/viewer" />;
}
```

Same search logic, different layout and navigation paths. One component, two uses.

---

### Context-Aware Filters

```typescript
{(entityType === 'All' || entityType === 'Study') && (
  // Show study filters: Status, Phase
)}
{(entityType === 'All' || entityType === 'Site') && (
  // Show site filters: City, Country
)}
{(entityType === 'All' || entityType === 'Examiner') && (
  // Show examiner filters: Role
)}
```

When user selects "Sites" toggle → only site-relevant filters show (City, Country). Study and examiner filters hide. This prevents confusion.

---

### useLazyQuery vs useQuery

```typescript
// useQuery — fires immediately when component mounts
const { data } = useQuery(QUERY);

// useLazyQuery — fires only when you call the function
const [runSearch, { data }] = useLazyQuery(QUERY);
// Later: runSearch({ variables: { ... } })
```

**Why lazy for search?**
- Search page starts idle (no results)
- Query only fires after user types or selects a filter
- `called` flag tells us if a search has been performed yet

---

### If You Were Building From Scratch

```
1. Start with a basic search:
   - Text input + button
   - On button click → useQuery with keyword
   - Display results

2. Add debounce:
   - useEffect + setTimeout
   - Cancel previous timer on each keystroke
   - Fire after 400ms of silence

3. Switch to useLazyQuery:
   - Don't search on mount
   - Show idle state until first search

4. Add entity type toggle:
   - Filter results client-side first
   - Then pass entityType to backend for efficiency

5. Add domain filters:
   - Status, Phase, City, Country, Role
   - Context-aware (show/hide based on entity type)

6. Add filter-only search:
   - Empty keyword + active filter → send '%%'
   - Immediate (no debounce needed)

7. Make it reusable:
   - Accept layout + baseRoute props
   - Thin wrappers for admin/viewer
```

---

### Key Takeaways

1. **Debounce 400ms** — prevents flooding server with requests on every keystroke
2. **useLazyQuery** — search only fires when triggered, not on mount
3. **MIN_KEYWORD_LENGTH = 2** — prevents expensive single-char searches
4. **`%%` trick** — satisfies backend validation, matches everything via LIKE
5. **Context-aware filters** — only show relevant filters for selected entity type
6. **LIKE with lowercase** — case-insensitive search via `LOWER(column) LIKE ?`
7. **Shared component** — same SearchPage for admin and viewer (different layout/routes)
8. **Three modes** — idle, keyword search (debounced), filter-only (immediate)
9. **Results grouped by entity** — Studies section, Sites section, Examiners section
10. **Click to navigate** — each result links to its detail page

---

**Lesson 26 done.** We've now covered all major flows in Phase 4. 

Next is **Phase 5: Building Order & Testing** — the exact order you'd build this project from Day 1, and how testing works.

Say **"next"** to continue, or ask questions.

---

next

---


## Phase 5, Lesson 27: Building Order — Day by Day from Scratch

---

### The Thinking Process

> "If I had to build this entire project from an empty folder, no AI, no copy-paste — what would I do first? Second? Third? What's the order that makes each step testable and buildable?"

**The principle:** Build in layers. Each day's work should produce something you can RUN and VERIFY before moving to the next.

---

### The Complete Build Order

---

### Week 1: Foundation + Auth + First Entity

#### Day 1: Project Setup

```
1. Create root folder: SNA-y2/
2. mkdir backend && cd backend && npm init -y
3. Install: express typescript ts-node-dev @types/express @types/node
4. Create tsconfig.json (strict: true, target: ES2020)
5. Create .env (PORT=4040, JWT_SECRET=..., DB_PATH=./data/app.db)
6. Create src/server.ts:
     import express from 'express';
     const app = express();
     app.get('/health', (_, res) => res.json({ status: 'ok' }));
     app.listen(4040, () => console.log('running'));
7. Add script: "dev": "ts-node-dev --respawn src/server.ts"
8. Run: npm run dev → verify http://localhost:4040/health returns { status: 'ok' }
```

**Checkpoint: Server runs. Health endpoint works. ✅**

#### Day 2: Database + Users Table

```
1. Install: better-sqlite3 @types/better-sqlite3 dotenv
2. Create src/db/connection.ts (getDb + initConnection)
3. Create src/db/query.ts (queryAll + queryOne)
4. Create src/db/migrate.ts (CREATE TABLE users + seedUsers)
5. Create src/utils/password.ts (hashPassword + verifyPassword)
6. Create src/types/index.ts (UserRow)
7. Call initConnection + initDb in server.ts
8. Run → verify data/app.db file appears with users table
```

**Checkpoint: Database created. 2 users seeded. ✅**

#### Day 3: JWT + Login Resolver

```
1. Install: jsonwebtoken @types/jsonwebtoken cookie-parser @types/cookie-parser cors @types/cors
2. Create src/utils/jwt.ts (signToken + verifyToken)
3. Create src/types/index.ts → add JwtPayload, GraphQLContext
4. Install: @apollo/server graphql
5. Create src/graphql/schema/auth.ts (User type, login mutation, me query)
6. Create src/graphql/schema/index.ts
7. Create src/repositories/authRepository.ts (findUserByEmail, findUserById)
8. Create src/services/authService.ts (loginUser — just access token for now)
9. Create src/graphql/resolvers/helpers.ts (requireAuth)
10. Create src/graphql/resolvers/auth.ts (login, me, logout)
11. Create src/graphql/resolvers/index.ts
12. Update src/app.ts: add Apollo Server + context function
13. Test: open http://localhost:4040/graphql → run login mutation → verify cookie set
```

**Checkpoint: Can log in via GraphQL. Cookie works. me query returns user. ✅**

#### Day 4: First Entity — Studies (Schema + CRUD)

```
1. Add studies table to migrate.ts
2. Create src/types/index.ts → add StudyRow
3. Create src/repositories/studyRepository.ts (findById, findPaged, insert, update)
4. Create src/services/studyService.ts (getStudiesPaged, createStudy — minimal rules)
5. Create src/validation/helpers.ts (parseOrThrow)
6. Create src/validation/studySchemas.ts (createStudySchema, updateStudySchema)
7. Create src/graphql/schema/study.ts (Study type, StudyPage, queries, mutations)
8. Create src/graphql/resolvers/study.ts (getStudies, getStudy, createStudy, updateStudy)
9. Add requireAdmin to helpers.ts
10. Test: create a study via GraphQL playground → verify it appears in getStudies
```

**Checkpoint: Full CRUD for studies works via GraphQL. ✅**

#### Day 5: Sites + Examiners (Same Pattern)

```
1. Repeat Day 4 pattern for sites:
   - Table, types, repository, service, validation, schema, resolver
2. Repeat for examiners
3. Test each: create, list, get by ID, update
```

**Checkpoint: All 3 entities have working CRUD. ✅**

---

### Week 2: Relationships + Business Rules + Frontend Start

#### Day 6: Junction Tables + Assignments

```
1. Add study_sites, site_examiners tables to migrate.ts
2. Add junction functions to studyRepository (insertStudySite, deleteStudySite)
3. Add junction functions to siteRepository (insertSiteExaminer, deleteSiteExaminer)
4. Add assignSiteToStudy, unassignSiteFromStudy to studyService
5. Add assignExaminerToSite, unassignExaminerFromSite to siteService
6. Add assignment mutations to schema + resolvers
7. Add type resolvers: Study.sites, Study.examiners, Site.studies, etc.
8. Test: assign a site to a study → verify it appears in getStudy response
```

**Checkpoint: Relationships work. Can assign/unassign. ✅**

#### Day 7: Business Rules (Status Transitions)

```
1. Add enforceStatusTransition to studyService
2. Add rules one by one: S2 (forward-only), S3 (need sites), S4 (need examiners)
3. Add date rules: D1 (startDate ≥ today), D4 (startDate ≤ today for Active)
4. Add site rules: P1 (Active needs examiner), P2 (auto-downgrade)
5. Add assignment rules: SI1 (only Active sites), SI3 (not Closed)
6. Test each rule: try to violate it → verify correct error returned
```

**Checkpoint: All domain rules enforced. Invalid operations rejected with clear errors. ✅**

#### Day 8: Audit Logging

```
1. Add audit_logs table to migrate.ts
2. Create auditRepository.ts (insertAuditLog, queryAuditLogs)
3. Add logAudit to helpers.ts
4. Add logAudit calls to ALL existing mutation resolvers
5. Create auditService.ts + audit resolver (getAuditLogs, ADMIN only)
6. Add audit schema
7. Test: create a study → verify audit log appears
```

**Checkpoint: Every mutation is logged. Audit query works. ✅**

#### Day 9: Frontend Setup + Login Page

```
1. cd .. && npm create vite@latest frontend -- --template react-ts
2. Install: @apollo/client graphql react-router-dom @mui/material @emotion/react @emotion/styled
3. Install: react-hook-form @hookform/resolvers zod notistack
4. Create theme.ts, apolloClient.ts (just httpLink for now)
5. Create AuthContext (ME_QUERY)
6. Create LoginPage (form + useLogin hook)
7. Create App.tsx with BrowserRouter + /login route
8. Test: npm run dev → login → verify cookie set → me query works
```

**Checkpoint: Frontend login works. Auth context knows who's logged in. ✅**

#### Day 10: Frontend — Protected Routes + First List Page

```
1. Create ProtectedRoute, AdminRoute components
2. Create AdminLayout + AdminSidebar
3. Create useStudies hook + AdminStudiesPage (DataGrid)
4. Add routes to App.tsx
5. Test: login as admin → see studies list → login as viewer → redirected
```

**Checkpoint: Role-based routing works. Studies list renders. ✅**

---

### Week 3: Frontend CRUD + Detail Pages

#### Day 11: Create/Edit Dialogs

```
1. Create frontend validation/studySchemas.ts
2. Create CreateStudyDialog (2-step stepper + react-hook-form)
3. Create EditStudyDialog
4. Add mutations to adminService.ts
5. Wire up error handling (parseGqlError → setError)
6. Test: create study → appears in list. Edit → changes saved.
```

#### Day 12: Detail Pages

```
1. Create useStudy hook
2. Create AdminStudyDetailPage (info + related sites + related examiners)
3. Create DetailPageHeader, InfoField, RelatedDataGrid (reusable)
4. Add Autocomplete picker for site assignment
5. Test: click row → see detail → assign site → appears in list
```

#### Day 13: Sites + Examiners Pages (Same Pattern)

```
1. Repeat Day 11-12 for sites (list + create + edit + detail)
2. Repeat for examiners
3. Add examiner assignment to site detail page
```

#### Day 14: Viewer Pages

```
1. Create ViewerLayout + ViewerSidebar
2. Create ViewerStudiesPage, ViewerSitesPage, ViewerExaminersPage (read-only)
3. Create viewer detail pages (no CRUD buttons)
4. Test: login as viewer → can see data → no create/edit buttons
```

---

### Week 4: Advanced Features

#### Day 15: Certificates + SSE

```
1. Add examiner_certificates table
2. Add study_site_examiners table
3. Create certificate service + repository
4. Create StudySitePanel + CertificatePickerDialog
5. Add SSE mutations (assignExaminerToStudySite, etc.)
6. Test: assign examiner to study at site with certificate
```

#### Day 16: Refresh Tokens

```
1. Add refresh_tokens table
2. Create token.ts (generateRefreshToken + hashToken)
3. Create refreshTokenRepository
4. Update authService (dual tokens, refreshSession, rotation)
5. Update auth resolver (setRefreshCookie, refreshSession mutation)
6. Add errorLink to apolloClient (UNAUTHENTICATED → refresh → retry)
7. Test: wait 15 min (or shorten TTL) → verify seamless refresh
```

#### Day 17: Search + Audit UI

```
1. Create searchRepository + searchService + search resolver
2. Create SearchPage (shared, debounced, filters)
3. Create AuditLogsPage (MUI Table, expandable rows, entity filter)
4. Create EntityAuditHistoryPage (per-entity history)
5. Test: search works, audit logs display with diffs
```

#### Day 18: Dashboard + Polish

```
1. Create AdminDashboardPage (charts, stats)
2. Create ViewerDashboardPage (read-only charts)
3. Add loading skeletons (DashboardSkeleton, DetailPageSkeleton)
4. Add ErrorBoundary
5. Add DataLoaders (optimize N+1)
6. Add security middleware (helmet, rate limiting, requestId, logging)
```

#### Day 19: Testing

```
1. Backend unit tests (services, repositories)
2. Backend integration tests (supertest)
3. Frontend component tests (@testing-library/react)
4. E2E tests (Playwright)
```

#### Day 20: Documentation + Final Polish

```
1. Write docs/architecture.md
2. Write docs/auth.md
3. Write docs/database.md
4. Write docs/TESTING.md
5. Final review, fix edge cases
```

---

### The Key Principles Behind This Order

| Principle | Why |
|-----------|-----|
| **Backend before frontend** | Frontend needs an API to talk to |
| **Auth before features** | Every feature needs auth |
| **One entity first, then replicate** | Prove the pattern works, then copy it |
| **Simple CRUD before rules** | Get data flowing, then add constraints |
| **Rules before UI** | Backend must be correct; UI is just presentation |
| **Admin before viewer** | Admin has all features; viewer is a subset |
| **Core before advanced** | Basic CRUD before certificates, SSE, refresh tokens |
| **Testing last** | Test what's stable, not what's still changing |

---

### The "Prove It Works" Checkpoints

After each day, you should be able to:
1. **Run the server** (no crashes)
2. **Test the new feature** (via GraphQL playground or browser)
3. **Verify previous features still work** (nothing broken)

If you can't do all 3, don't move to the next day.

---

### Key Takeaways

1. **20 days** to build the entire project from scratch (experienced developer)
2. **Backend first** — always have a working API before building UI
3. **Auth is Day 3** — everything depends on it
4. **One entity proves the pattern** — then replicate for others
5. **Business rules come AFTER basic CRUD** — get data flowing first
6. **Advanced features last** — refresh tokens, SSE, certificates are Week 4
7. **Each day has a checkpoint** — something runnable and verifiable
8. **Testing comes after stability** — don't test code that's still changing
9. **Documentation last** — document what exists, not what you plan
10. **Same patterns everywhere** — once you build studies, sites and examiners are copy-paste

---

**Lesson 27 done.** Next is **Lesson 28: Testing Strategy** — how tests are structured, what to test, and how to read existing tests in any codebase.

Say **"next"** to continue, or ask questions.

---

next

---

## Phase 5, Lesson 28: Testing Strategy — Unit, Integration, E2E

---

### The Thinking Process

> "I've built the app. It works when I test manually. But how do I make sure it KEEPS working when I change things? How do I catch bugs before users do?"

Answer: **Three levels of testing**, each catching different types of bugs:

```
                    ┌─────────────┐
                    │    E2E      │  ← Few tests, slow, test real user flows
                    │  (Playwright)│
                   ┌┴─────────────┴┐
                   │  Integration   │  ← Medium tests, test API contracts
                   │  (supertest)   │
                  ┌┴───────────────┴┐
                  │     Unit         │  ← Many tests, fast, test logic in isolation
                  │   (vitest)       │
                  └──────────────────┘
```

| Level | What it tests | Speed | Count in this project |
|-------|--------------|-------|----------------------|
| Unit | One function in isolation | ~1ms each | 155 backend tests |
| Integration | Full API request (HTTP → DB → response) | ~50ms each | Included in 155 |
| E2E | Real browser, real clicks, real flows | ~5s each | 3 spec files |
| Frontend | Component rendering + interactions | ~20ms each | 63 tests |

---

### Let me show you actual test files:

---

---

### Unit Tests — Testing Business Logic in Isolation

**What you're looking at:** Tests for `studyService.ts` — the business rules.

**The pattern:**

```typescript
import { describe, it, expect, beforeEach } from 'vitest';
import { setupTestDb } from '../testHelpers';

beforeEach(() => { setupTestDb(); });  // Fresh in-memory DB for each test

describe('createStudy', () => {
  it('S1: always creates with status Planned', () => {
    const s = createStudy({ protocolId: 'P001', title: 'T', ... });
    expect(s.status).toBe('Planned');
  });

  it('D1: rejects startDate in the past', () => {
    expect(() => createStudy({ ..., startDate: pastDate(1) })).toThrow('Start date');
  });
});
```

**Key elements:**
1. `beforeEach(() => setupTestDb())` — fresh database for EVERY test (no test pollution)
2. `setupTestDb()` uses `:memory:` SQLite — no file, no cleanup needed, blazing fast
3. Each test verifies ONE rule (named by rule ID: S1, D1, D2, S8, etc.)
4. `expect(...).toThrow('...')` — verifies the error message contains expected text
5. Helper functions (`todayUTC`, `futureDate`, `pastDate`) make dates easy

**Why test services (not resolvers)?**
- Services contain the business logic
- If the service is correct, the resolver just passes data through
- Services are easier to test (no HTTP, no GraphQL, no context)

---

### Integration Tests — Testing the Full API

---

---

### Integration Tests — What's Different

**Unit tests** call service functions directly:
```typescript
const s = createStudy({ ... });
expect(s.status).toBe('Planned');
```

**Integration tests** send real HTTP requests:
```typescript
const res = await request(app)
  .post('/graphql')
  .set('Cookie', withCookie(adminToken))
  .send(gql(`mutation { createStudy(input: {...}) { id status } }`));

expect(res.body.data.createStudy.status).toBe('Planned');
```

**What integration tests verify that unit tests don't:**
- Middleware works (CORS, cookie parsing, rate limiting)
- GraphQL schema is correct (types match)
- Resolver wiring is correct (schema → resolver → service)
- Auth cookies work end-to-end
- Error codes are returned correctly in HTTP response

---

### Frontend Tests — Component Testing

---

---

### Frontend Tests — The Pattern

```typescript
function renderPage(mocks: object[]) {
  return render(
    <MockedProvider mocks={mocks} addTypename={false}>  // Mock Apollo responses
      <MemoryRouter initialEntries={['/viewer/studies']}>  // Mock routing
        <Routes>
          <Route path="/viewer/studies" element={<ViewerStudiesPage />} />
        </Routes>
      </MemoryRouter>
    </MockedProvider>
  );
}
```

**Key concepts:**
- `MockedProvider` — replaces real Apollo Client with mock responses (no backend needed)
- `MemoryRouter` — simulates URL routing without a real browser
- `mocks` array — defines what data each query returns
- `vi.mock(...)` — replaces complex components (layout) with simple wrappers

**What frontend tests verify:**
- Component renders correctly with data
- Loading/error states display properly
- User interactions work (click, type, navigate)
- Read-only mode has no CRUD buttons
- Navigation happens on row click

---

### E2E Tests — Real Browser, Real Everything

---


---

### E2E Tests — What's Different

**E2E tests use a REAL browser (Chromium via Playwright):**
- Real frontend running on port 5173
- Real backend running on port 4040
- Real database
- Real cookies, real network requests

**What E2E tests verify that other tests don't:**
- Full user workflow works end-to-end
- Frontend and backend are correctly integrated
- Cookies work in a real browser
- Navigation works
- Toasts appear
- Dialogs open and close
- Data persists across page navigations

**The `RUN_ID` pattern:**
```typescript
const RUN_ID = Date.now().toString(36).slice(-5);
// Generates unique codes like "e2e-S-k7x2f" so tests don't conflict with each other
```

---

### What to Test (Decision Framework)

| What | Test Level | Why |
|------|-----------|-----|
| Business rules (status transitions, date logic) | Unit | Fast, isolated, many edge cases |
| Uniqueness checks, assignment prerequisites | Unit | Service logic |
| Auth guards (RBAC) | Integration | Need full request pipeline |
| Validation errors (fieldErrors format) | Integration | Need GraphQL response format |
| Cookie handling | Integration | Need HTTP layer |
| Component renders correctly | Frontend | Visual correctness |
| User interactions (click, type) | Frontend | UX works |
| Full user workflow | E2E | Everything works together |

**What NOT to test:**
- Don't test library code (MUI renders correctly, Apollo sends requests)
- Don't test trivial getters (repository functions that just run SQL)
- Don't test the same thing at multiple levels (if unit test covers it, skip integration)

---

### The Test File Organization

```
backend/src/__tests__/
├── testHelpers.ts              ← setupTestDb, seedUser
├── unit/
│   ├── studyService.test.ts    ← Business rules for studies
│   ├── siteService.test.ts     ← Business rules for sites
│   ├── examinerService.test.ts ← Certificate logic
│   ├── authService.test.ts     ← Login, refresh, revoke
│   ├── auditService.test.ts    ← Audit log queries
│   ├── searchService.test.ts   ← Search matching
│   ├── certificateService.test.ts ← Certificate CRUD
│   ├── sseIntegrity.test.ts    ← 3-way junction rules
│   ├── resolverHelpers.test.ts ← requireAuth, requireAdmin, logAudit
│   └── refreshTokenRepository.test.ts ← Token storage
└── integration/
    ├── graphql.test.ts         ← RBAC, basic CRUD, health check
    ├── graphqlExpanded.test.ts ← More RBAC, audit, validation
    ├── graphqlRefresh.test.ts  ← Refresh token flow
    └── graphqlSearch.test.ts   ← Search API

frontend/src/__tests__/
├── setup.ts                    ← @testing-library/jest-dom matchers
├── unit/
│   ├── AdminRoute.test.tsx     ← Route guard logic
│   ├── ProtectedRoute.test.tsx ← Route guard logic
│   ├── ErrorBoundary.test.tsx  ← Error fallback
│   └── login.smoke.test.tsx    ← Login page renders
└── integration/
    ├── ViewerStudiesPage.test.tsx    ← Read-only list
    ├── AdminStudyDetailPage.test.tsx ← SSE panel, cert picker
    ├── AdminSitesPage.test.tsx       ← Create dialog
    ├── SearchPage.test.tsx           ← Debounce, results
    └── ...

e2e/
├── admin-workflow.spec.ts      ← Create study/site/examiner, add cert
├── refresh-smoke.spec.ts       ← Token refresh or redirect
└── viewer-smoke.spec.ts        ← Read-only navigation
```

---

### If You Were Building From Scratch

```
1. Set up test infrastructure FIRST:
   - Install vitest
   - Create testHelpers.ts (setupTestDb)
   - Verify one simple test runs

2. Write unit tests AS you build services:
   - Build createStudy → write test for S1, D1, D2, S8
   - Build updateStudy → write tests for S2, S3, D4, D6
   - Each rule gets a test IMMEDIATELY

3. Write integration tests after resolvers are stable:
   - Test RBAC (viewer can't mutate)
   - Test validation errors (fieldErrors format)
   - Test auth flow (login, cookie, protected query)

4. Write frontend tests after pages are stable:
   - Test that pages render
   - Test that interactions work
   - Test error states

5. Write E2E tests LAST:
   - Test the happy path (create study, create site, etc.)
   - Test auth flows (refresh, logout)
   - Keep them minimal (slow, fragile)
```

---

### Key Takeaways

1. **Three levels** — unit (fast, many), integration (medium), E2E (slow, few)
2. **In-memory SQLite** — `:memory:` gives fresh DB per test, no cleanup
3. **beforeEach(setupTestDb)** — every test starts with clean state
4. **Test business rules in unit tests** — fast feedback, easy to add edge cases
5. **Test API contracts in integration** — RBAC, validation format, cookies
6. **Test user flows in E2E** — real browser, real everything
7. **MockedProvider for frontend** — no backend needed for component tests
8. **RUN_ID for E2E** — unique data per run prevents conflicts
9. **Don't over-test** — test logic, not libraries
10. **Write tests as you build** — not after, not before, but alongside

---

## Phase 5, Lesson 29: How to Read Any Existing Codebase

---

### Your Manager's Question Answered

> "If you can't understand this simple SNA website, how will you work in existing codebases?"

Here's the mental model that works for ANY project:

### Step 1: Identify the Tech (5 minutes)
```
Read package.json → What framework? What database? What API style?
```

### Step 2: Find the Entry Point (2 minutes)
```
Backend: server.ts / index.ts / app.ts → How does it start?
Frontend: main.tsx / index.tsx → What wraps the app?
```

### Step 3: Trace ONE Feature (30 minutes)
```
Pick the simplest feature (e.g., login, or list page)
Follow it: UI → hook → API call → resolver → service → DB → back
```

### Step 4: Identify the Layers (10 minutes)
```
Where's the API? Where's the business logic? Where's the DB access?
What's the naming convention? How are files organized?
```

### Step 5: Read the Tests (15 minutes)
```
Tests tell you WHAT the code is supposed to do.
Test names are documentation: "S1: always creates with status Planned"
```

---

### The Universal Pattern (Every Web App)

```
Frontend (UI) → API Layer → Business Logic → Data Access → Database
     ↑                                                        │
     └────────────────── Response ────────────────────────────┘
```

The tech changes. The pattern doesn't.

| This Project | Other Projects |
|---|---|
| React | Angular, Vue, Svelte |
| Apollo Client | axios, fetch, tRPC |
| GraphQL | REST, gRPC |
| Express | Fastify, Koa, NestJS |
| SQLite | PostgreSQL, MongoDB |
| Zod | Joi, Yup, class-validator |
| JWT cookies | Session tokens, OAuth |

**Same layers. Same flow. Different names.**

---

**Teaching complete.** 🎉

You now understand:
- ✅ The domain (studies, sites, examiners, certificates)
- ✅ Every technology choice and why
- ✅ The folder structure and naming conventions
- ✅ Every backend layer (server → middleware → resolver → service → repository → DB)
- ✅ Every frontend layer (App → routing → pages → hooks → services → Apollo)
- ✅ Authentication (JWT + cookies + refresh token rotation)
- ✅ Authorization (requireAuth + requireAdmin)
- ✅ Validation (Zod on both sides, fieldErrors bridge)
- ✅ Audit logging (before/after snapshots)
- ✅ DataLoaders (N+1 prevention)
- ✅ Complete flows (login, create, assign, refresh, search)
- ✅ Build order (what to create first)
- ✅ Testing strategy (unit, integration, E2E)
- ✅ How to read any codebase

Ask me anything if you need deeper explanation on any specific part.