# Engagement Visualization Platform

A web platform for visualizing Degrees of Engagement (DoE) across projects at Amsterdam University of Applied Sciences. The supplied project description identifies secure authentication, role-based access control, and a modular REST API built with Spring Boot and Angular, with JUnit for testing. No source repository or project documentation was available here to verify additional implementation details.

## Main techniques and lessons

- **Keep access control explicit**: Role-based access control makes permissions an important part of API design, not just a concern of the user interface.
- **Connect data and visualization carefully**: Project comparisons are meaningful only when the engagement measure is interpreted consistently across the views that present it.
- **Likely lesson (inferred)**: Testing the API and access boundaries alongside the interface helps preserve a coherent experience for users with different roles.

These lessons are inferred from the supplied project description; they are not independently verified project findings.

## Illustrative high-level organization

The tree is conceptual, based on the supplied description, and does not represent an inspected source layout.

```text
Engagement visualization platform
├── Angular project views
│   └── Degrees of Engagement visualization
├── Spring Boot REST API
│   ├── Authentication
│   └── Role-based access control
└── JUnit tests
```
