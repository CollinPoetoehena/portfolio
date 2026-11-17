# Java Code Quality and Clone Detection Tool

A Java code quality tool that computes and visualizes SIG-based maintainability metrics, including volume, complexity, duplication, testing, and coupling. The supplied project description identifies custom AST traversal and automated risk scoring implemented in Rascal. No source repository or project documentation was available here to verify additional implementation details.

## Main techniques and lessons

- **AST-based analysis**: A shared traversal of Java syntax can provide the structural basis for extracting multiple code-quality signals.
- **Metrics as signals, not verdicts**: Combining measures such as complexity, duplication, and testing can help direct attention to code that merits review; a risk score should support, not replace, engineering judgment.
- **Likely lesson (inferred)**: Making metrics useful to developers depends on presenting the underlying signals clearly enough that a score can be understood and acted on.

These lessons are inferred from the supplied project description; they are not independently verified project findings.

## Illustrative high-level organization

The tree is conceptual, based on the supplied description, and does not represent an inspected source layout.

```text
Java code quality and clone detection tool
├── Java source analysis
│   └── Custom AST traversal in Rascal
├── Maintainability metrics
│   ├── Volume and complexity
│   ├── Duplication and testing
│   └── Coupling
├── Risk scoring
└── Metric visualization
```
