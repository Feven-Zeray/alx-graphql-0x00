# Rick and Morty — Episode Queries

This folder contains GraphQL queries and sample outputs for fetching individual Rick and Morty episodes by ID. Use these queries as examples or tests against the public GraphQL API.

Contents
- `episode-id-1.graphql` / `episode-id-1-output.json` — Query and sample response for episode with ID 1
- `episode-id-2.graphql` / `episode-id-2-output.json` — Query and sample response for episode with ID 2
- `episode-id-3.graphql` / `episode-id-3-output.json` — Query and sample response for episode with ID 3
- `episode-id-4.graphql` / `episode-id-4-output.json` — Query and sample response for episode with ID 4

GraphQL endpoint
- Public API: https://rickandmortyapi.com/graphql

Quick usage examples

1) Using GraphiQL / GraphQL Playground
- Open the endpoint in your GraphiQL/Playground client and paste the contents of any `*.graphql` file to run it interactively.

2) Using curl (example with inline query)
- Replace the query body with the contents of a `*.graphql` file if desired:
```
curl -s -H "Content-Type: application/json" \
    -d '{"query":"query { episode(id: 1) { id name air_date episode characters { id name } } }"}' \
    https://rickandmortyapi.com/graphql
```

3) Using a file as the request body
- Create a JSON payload file (e.g. `payload.json`) with:
```
{ "query": "<paste GRAPHQL query here as a single line or escaped string>" }
```
- Then:
```
curl -s -H "Content-Type: application/json" -d @payload.json https://rickandmortyapi.com/graphql
```

Conventions
- Query files: `.graphql` — contain a single query targeting an episode by ID.
- Output files: `.json` — contain the recorded API response for the corresponding query.
- Naming: `episode-id-<N>.*` — where `<N>` is the episode ID used in the query.

Adding a new episode
1. Copy one of the existing `episode-id-*.graphql` files and update the ID and requested fields as needed.
2. Run the query against the endpoint and save the response as `episode-id-<N>-output.json`.

Notes
- The sample outputs are snapshots and may differ from live responses as the API data changes.
- Keep queries minimal to make outputs easier to review and version-control.

License / Source
- Queries target the public Rick and Morty GraphQL API: https://rickandmortyapi.com/graphql
- This repository contains only sample queries and outputs; adapt and reuse as needed.
