# GraphQuest: Exploring and Implementing GraphQL

## Project Overview

The Rick and Morty GraphQL API Explorer is a multi-phase project designed to help learners gain proficiency in GraphQL, from writing basic queries to integrating them into a full-stack React application. The Rick and Morty API serves as the data source for practice and exploration.

---

## Learning Objectives

### Level 0 – GraphQL Fundamentals

- Construct precise GraphQL queries.
- Use arguments (e.g., `id`, `page`) to filter and paginate results.
- Fetch only necessary fields to avoid over-fetching.
- Differentiate between single-item queries and paginated lists.

### Level 1 & 2 – Frontend Integration

- Set up a Next.js application with TypeScript, Apollo Client, and Tailwind CSS.
- Configure Apollo Client to connect React components to a GraphQL endpoint.
- Use queries to fetch and manage data.
- Manage local component state, such as pagination.
- Structure the React application with clear separation of concerns (queries, interfaces, components).

---

## Key Concepts

- **GraphQL Query Language:** Allows precise data fetching in a single request.
- **Schema & Types:** Defines data structures like `Character`, `Episode`, and `Info`.
- **Arguments:** Filter queries (e.g., by `id` or `page`).
- **Pagination:** Navigate large datasets with fields like `pages`, `next`, and `prev`.
- **Apollo Client:** Handles data fetching, caching, and state management.
- **React Integration:** Uses ApolloProvider and hooks to manage queries and state.
- **TypeScript:** Adds static typing for safer and more maintainable code.

---

## Tools & Libraries

- **Runtime/Environment:** Node.js
- **Framework:** Next.js
- **Language:** TypeScript
- **GraphQL Client:** Apollo Client
- **GraphQL Library:** `graphql`
- **Styling:** Tailwind CSS
- **Linting:** ESLint
- **API:** [Rick and Morty GraphQL API](https://rickandmortyapi.com/graphql)

---

## Project Tasks

### 1. Query Specific Characters by ID

- Write queries to fetch character information for multiple IDs.
- Focus on fields like name, status, species, type, and gender.

### 2. Query Paginated Character Lists

- Retrieve lists of characters in pages.
- Include fields like name, status, and image.

### 3. Query Specific Episodes by ID

- Fetch detailed episode information such as name, air date, and episode code.

### 4. Frontend Integration with React

- Set up a React application using Next.js.
- Integrate Apollo Client to query the GraphQL API.
- Display data in a clean, paginated interface.
- Use components for better structure and reusability.

### 5. Manual Review

- Ensure all queries and frontend integration are functional.
- Submit all required files and directories for review.

---

## File Structure Example

```bash
alx-graphql-0x00/
├── character/
│ ├── README.md
│ ├── character-id-1.graphql
│ ├── character-id-1-output.json
│ ├── character-id-2.graphql
│ ├── character-id-2-output.json
│ ├── character-id-3.graphql
│ ├── character-id-3-output.json
│ ├── character-id-4.graphql
│ └── character-id-4-output.json
└── episode/
├── README.md
├── episode-id-1.graphql
├── episode-id-1-output.json
├── episode-id-2.graphql
├── episode-id-2-output.json
├── episode-id-3.graphql
└── episode-id-3-output.json

alx-graphql-0x01/
└── alx-rick-and-morty-app/
├── README.md
├── graphql/
│ ├── apolloClient.ts
│ └── queries.ts
└── pages/
└── _app.tsx

alx-graphql-0x02/
└── alx-rick-and-morty-app/
├── README.md
├── interfaces/
│ └── index.ts
├── components/
│ └── common/
│ └── EpisodeCard.tsx
└── pages/
└── index.tsx
```

## Developer Information

- **Name:** Feven Zeray
- **Email:** fevenzeray2028@gmail.com
- **Role:** Full-Stack Developer
- **Skills:** React, Next.js, TypeScript, Tailwind CSS, Apollo Client, GraphQL, Node.js
- **GitHub:** [https://github.com/Feven-Zeray](https://github.com/Feven-Zeray)

---
