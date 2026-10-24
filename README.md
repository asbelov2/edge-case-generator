# Edge Case Generator

**Break your UI with the data your test fixtures forgot.**

Generate reproducible edge-case variations of existing JSON data to discover UI bugs before your users do.

### Why?

Real-world data is messy. Long strings, empty arrays, unexpected nulls, and boundary values can break otherwise well-tested interfaces.

### Proposed API

```ts
const cases = generateEdgeCases({
  name: 'Alex',
  age: 30,
  tags: ['developer']
}, {
  preset: 'ui',
  maxCases: 40
});
```

Each generated scenario identifies the modified field and provides a complete mutated fixture.

### MVP

- String boundary cases
- Numeric edge cases
- Empty arrays and null values
- Nested object traversal
- Deterministic scenario generation
- Human-readable scenario descriptions
- Immutable input data

**Status:** Planning. API subject to change.

**License:** MIT (planned).
