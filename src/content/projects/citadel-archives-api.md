---
title: "Citadel Archives API"
description: "A RESTful API providing programmatic access to the Citadel Council's historical records, species databases, and codex entries."
pubDate: 2026-01-15
tags: ["REST API", "Go", "PostgreSQL"]
url: "https://github.com/commander-spaceman/citadel-api"
image: "https://placehold.co/600x300/1a1a2e/90a4ae?text=Citadel+API"
status: "archived"
---

The Citadel Archives API was a project to provide structured, programmatic access to the Citadel Council's vast historical databases. It served researchers, journalists, and developers who needed reliable data about galactic species, events, and political records.

## Motivation

The Citadel Archives contain over 50,000 years of recorded galactic history, but accessing that data has always required navigating a bureaucratic labyrinth of access requests, terminal reservations, and format conversions. The Archives API was built to democratize access to public records.

## Endpoints

```
GET    /api/v1/species
GET    /api/v1/species/:id
GET    /api/v1/events?era=prothean
GET    /api/v1/systems/:name/planets
GET    /api/v1/codex/search?q=eezo
POST   /api/v1/codex/entries         (authenticated)
```

## Technical Stack

- **Language:** Go
- **Database:** PostgreSQL with full-text search
- **Cache:** Redis for frequently accessed records
- **Auth:** OAuth 2.0 via Citadel Identity Service
- **Rate limiting:** 1,000 requests/hour for public access, 10,000 for registered researchers

## Sample Response

```json
{
  "id": "SPE-QUA-001",
  "name": "Quarian",
  "homeworld": "Rannoch",
  "biology": "dextro-amino",
  "population": 17000000,
  "government": "Admiralty Board",
  "council_status": "none",
  "notable_events": [
    "Creation of the Geth",
    "Morning War",
    "Establishment of the Migrant Fleet"
  ]
}
```

## Usage Statistics

At its peak, the API served over 2 million requests per day from 14,000 registered applications across Council space.

## Status

Archived. The Citadel Archives migrated to a new internal platform in 2186 CE. The API source code remains available for reference.
