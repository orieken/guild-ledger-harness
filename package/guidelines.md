# H1 coding guidelines

- Prefer the smallest coherent change that satisfies the supplied request. Avoid unrelated refactors and speculative features.
- Follow the surrounding code's naming, structure, and public interfaces. Reuse existing abstractions where they fit; keep new abstractions proportional to the change.
- Make data flow and failure behavior explicit. Handle errors at the layer that can explain or recover from them; avoid silently discarding failures.
- Keep state changes consistent with the guarantees stated in the request and existing interfaces. Do not invent additional business rules to fill missing requirements.
- Treat external input as untrusted. Preserve existing access controls and avoid exposing secrets or sensitive data in logs and responses.
- Prefer readable, typed interfaces and deterministic behavior. Add comments when they explain a constraint or decision that the code cannot make clear.
- Use focused checks for changed behavior when they are useful. Distinguish observed check results from expectations and report uncertainty honestly.
