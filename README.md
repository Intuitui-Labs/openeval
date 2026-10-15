# OpenEval (`@intuitui-labs/openeval`)

[![CI](https://github.com/intuitui-labs/openeval/actions/workflows/ci.yml/badge.svg)](https://github.com/intuitui-labs/openeval/actions/workflows/ci.yml)
[![npm](https://img.shields.io/npm/v/@intuitui-labs/openeval?style=flat-square&color=blue)](https://www.npmjs.com/package/@intuitui-labs/openeval)
[![TypeScript](https://img.shields.io/badge/TypeScript-7.0.2-blue.svg?style=flat-square)](https://www.typescriptlang.org/)
[![Vitest 5](https://img.shields.io/badge/tested%20with-Vitest%205-729B1B.svg?style=flat-square)](https://vitest.dev/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)

> **Transparent, participatory evaluation, trade-off analysis, and recommendation framework for complex software ecosystems.**  
> Grounded in **Conceptual Topology** (Neev, University of Moratuwa).

---

## 🎯 The Philosophy

Most discovery platforms present **inventory rather than capability**. They produce popularity rankings and black-box leaderboards while leaving the user to guess:
- What does this option actually do?
- Which trade-offs matter for my specific constraints?
- What evidence supports this recommendation?
- Is this data fresh, or running on inertia?

**OpenEval provides orientation, not mere information.** It connects multi-source evidence (provenance, freshness, confidence) directly to user goals and priorities.

---

## 📦 Installation & Usage

```bash
pnpm add @intuitui-labs/openeval
```

### Tree-Shakable Subpath Exports
```typescript
import { 
  evaluateOffers, 
  decodeShareState, 
  type UserProfile, 
  type AtlasOffer 
} from '@intuitui-labs/openeval';

// Ingestion pipelines can be imported independently:
import { 
  collectSource, 
  HttpSourceFetcher, 
  FileSnapshotStore 
} from '@intuitui-labs/openeval/ingestion';
```

---

## 🧪 Quality & Verification

```bash
# Run strict TypeScript verification
pnpm run check-types

# Run Vitest 5 suite with v8 coverage
pnpm run test:coverage

# Build clean distribution bundle
pnpm run build
```

---

## 📚 Documentation
- [Publishing Runbook (`docs/publishing.md`)](./docs/publishing.md)
- [Testing Architecture & G0 Claims (`docs/testing.md`)](./docs/testing.md)
- [Badges & Metrics Specification (`docs/badges-and-metrics.md`)](./docs/badges-and-metrics.md)

---

## 📄 License
MIT © Intuitui Labs.
