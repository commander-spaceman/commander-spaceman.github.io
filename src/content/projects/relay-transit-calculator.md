---
title: "Relay Transit Calculator"
description: "An open-source tool implementing the Teks-Solarin invariant for calculating optimal mass relay transit routes and fuel efficiency."
pubDate: 2026-05-08
tags: ["TypeScript", "Physics", "Open Source"]
url: "https://github.com/commander-spaceman/relay-calc"
image: "https://placehold.co/600x300/0d2137/64b5f6?text=Relay+Calculator"
status: "active"
---

The Relay Transit Calculator (RTC) is an open-source implementation of Dr. Palon Teks' corrected transit equations for mass relay travel. It provides accurate fuel consumption estimates and optimal route planning using the Teks-Solarin invariant.

## Background

For centuries, relay transit calculations have been based on Matriarch Dilinaga's classical field equations. While adequate for short-range travel, these equations produce increasingly inaccurate results at transit speeds exceeding 10,000c due to their assumption of Euclidean corridor geometry.

Dr. Teks' 2186 paper demonstrated that correcting for non-Euclidean curvature yields measurable improvements in transit efficiency, up to 12.8% fuel savings on long-distance routes.

This tool makes those corrections accessible to any pilot or fleet navigator.

## Features

- **Route planning** between any two mapped relay pairs
- **Fuel estimation** using both classical and corrected equations
- **Side-by-side comparison** showing efficiency gains
- **Corridor stability** predictions for planned transits
- **Bulk calculation** for fleet-wide route optimization

## Usage

```typescript
import { RelayCalculator } from "@cmdr/relay-calc";

const calc = new RelayCalculator();

const route = calc.plan({
  origin: "Serpent Nebula",
  destination: "Exodus Cluster",
  method: "teks-solarin",
});

console.log(route.fuelSavings); // "1.39%"
console.log(route.transitTime); // "0.34s"
console.log(route.stability); // 0.9971
```

## Accuracy

RTC's calculations have been validated against the experimental data published in Dr. Teks' paper. All 47 primary relay pairs in Council space produce results within 0.02% of the published values.

## Status

Actively maintained. Version 2.0 added support for secondary relay pairs and custom corridor geometry inputs.
