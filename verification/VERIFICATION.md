# Verification record — JSP-000301

Toolchain: leanprover/lean4:v4.20.0 (no Mathlib dependency)
Verified: 2026-10-08

## Clean build
```
$ lake build
Build completed successfully.
```

## Axiom audit
```
Jsp000301Lean/JSP000301.lean:266:0: 'jsp_000301' depends on axioms: [propext, Quot.sound]
Jsp000301Lean/JSP000301.lean:267:0: 'jsp_000301_counterexample' depends on axioms: [propext, Quot.sound]
```

No `sorry`, `admit`, `native_decide`, or added `axiom` declarations.
The file contains both `#print axioms` calls; the lines above are the
verbatim build output for them.

