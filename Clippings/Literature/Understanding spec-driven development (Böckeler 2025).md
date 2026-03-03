# Understanding Spec-Driven-Development: Kiro, spec-kit, and Tessl
#articles #ai #codegen #dev

https://martinfowler.com/articles/exploring-gen-ai/sdd-3-tools.html

Definition: "...writing a 'spec' before writing code with AI ('documentation first'). The spec becomes the source of truth for the human and the AI".

Spec-driven development is poorly-defined.

Three possible specific approaches:

1. Spec-first: use a spec for the task at hand, then throw it away.
2. Spec-anchored: spec is kept after the task is complete, to continue evolving & maintaining the feature.
3. Spec-as-source: spec is the main source file, and only the spec is edited by the human, only agents touch the code.

Definition of "spec" is given.

Parallel to work in the past: BDD (behavior-driven development) and MDD (model-driven development)

Drawbacks:

- Lots of markdown to read & maintain, very tedious.
- Even so, the agent often deviates from the script.
- Doesn't seem to work with small, iterative steps (which the past has shown us is the best approach to software development)

Great term: "semantically diffused"

Conclusion: writing an anchoring spec for a piece of code generation makes perfect sense and works well. Using the spec-as-source approach doesn't have good evidence behind it, and appears contrary to best practice for no real benefit.
