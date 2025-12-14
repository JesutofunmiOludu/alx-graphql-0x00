# GraphQuest: Exploring and Implementing GraphQL

---

## 📌 Project Overview & Summary  
### The Rick and Morty GraphQL API Explorer

**GraphQuest** is a multi-phase, hands-on learning project designed to help learners master **GraphQL**, starting from writing basic queries and progressing to integrating GraphQL into a modern **React (Next.js)** application using **Apollo Client** and **TypeScript**.

The project uses the popular **Rick and Morty GraphQL API**, providing an engaging and real-world context to explore GraphQL concepts and frontend integration.

The project is organized into progressive stages, each stored in a dedicated directory:

- `alx-graphql-0x00` — GraphQL fundamentals (queries & pagination)
- `alx-graphql-0x01` — GraphQL + React setup
- `alx-graphql-0x02` — Full React integration with pagination and UI

---

## 🎯 Learning Objectives

By completing this project, learners will be able to:

### **Level 0: GraphQL Fundamentals**
- Write precise GraphQL queries
- Use arguments (`id`, `page`) to filter and paginate results
- Avoid over-fetching by requesting only necessary fields
- Distinguish between single-item queries and paginated lists

### **Level 1 & 2: Frontend Integration**
- Set up a **Next.js** application with **TypeScript**, **Apollo Client**, and **Tailwind CSS**
- Connect a React app to a GraphQL endpoint
- Execute queries using the `useQuery` hook
- Manage pagination and component state
- Structure a scalable React project with clear separation of concerns

---

## 🧠 Key Concepts Covered

- **GraphQL Query Language** — Flexible data fetching using a single endpoint
- **Schema & Types** — Understanding `Character`, `Episode`, and `Info` types
- **Arguments** — Filtering data using `id`, `page`, and `filter`
- **Pagination** — Navigating large datasets using `Info { pages, next, prev }`
- **Apollo Client** — Data fetching, caching, and state management
- **React Integration** — `ApolloProvider` and `useQuery`
- **TypeScript** — Strong typing using interfaces and utility types

---

## 🛠 Tools & Technologies

| Category | Tool |
|-------|------|
| Runtime | Node.js |
| Framework | Next.js |
| Language | TypeScript |
| GraphQL Client | Apollo Client |
| GraphQL Core | graphql |
| Styling | Tailwind CSS |
| Linting | ESLint |
| API | Rick and Morty GraphQL API |

🔗 **API Endpoint:**  
https://rickandmortyapi.com/graphql

---

## 🌍 Real-World Use Cases

This project mirrors real-world application architectures such as:

- **E-commerce platforms** — Product listings and details
- **Blogs & News platforms** — Articles with pagination
- **Social Media feeds** — Paginated posts and comments
- **Analytics dashboards** — Structured and filtered datasets

The skills gained are directly transferable to building **scalable**, **performant**, and **maintainable** applications.

---

## 📂 Project Structure & Tasks

---

### **Task 0: Get a Specific Character by ID**
📁 **Repo:** `alx-graphql-0x00`  
📂 **Directory:** `character`  

**Objective:**  
Write GraphQL queries to retrieve a character by ID.

**Instructions:**
- Use `character(id: ID!)`
- IDs: `1, 2, 3, 4`
- Fields:
  - `id`
  - `name`
  - `status`
  - `species`
  - `type`
  - `gender`

**Files:**
- `character-id-1.graphql`
- `character-id-1-output.json`
- `character-id-2.graphql`
- `character-id-2-output.json`
- `character-id-3.graphql`
- `character-id-3-output.json`
- `character-id-4.graphql`
- `character-id-4-output.json`
- `README.md`

---

### **Task 1: Get a Paginated List of Characters**
📁 **Repo:** `alx-graphql-0x00`  
📂 **Directory:** `character`

**Objective:**  
Fetch a paginated list of characters.

**Instructions:**
- Use `characters(page: Int)`
- Pages: `1, 2, 3, 4`
- Fields:
  - `id`
  - `name`
  - `status`
  - `image`

**Files:**
- `characters-page-1.graphql`
- `characters-page-1-output.json`
- `characters-page-2.graphql`
- `characters-page-2-output.json`
- `characters-page-3.graphql`
- `characters-page-3-output.json`
- `characters-page-4.graphql`
- `characters-page-4-output.json`
- `README.md`

---

### **Task 2: Get a Specific Episode by ID**
📁 **Repo:** `alx-graphql-0x00`  
📂 **Directory:** `episode`

**Objective:**  
Fetch episode details by ID.

**Instructions:**
- Use `episode(id: ID!)`
- Fields:
  - `id`
  - `name`
  - `air_date`
  - `episode`

---

### **Task 3: GraphQL in React (Setup)**
📁 **Repo:** `alx-graphql-0x01`  
📂 **Directory:** `alx-rick-and-morty-app`

**Objective:**  
Set up a Next.js project with GraphQL support.

**Steps:**
1. Create a Next.js app with TypeScript
2. Install dependencies:
   ```bash
   npm install @apollo/client graphql
   npm install @types/graphql
