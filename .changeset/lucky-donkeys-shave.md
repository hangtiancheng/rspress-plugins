---
'rspress-plugin-mermaid': patch
---

Fix mermaid rendering by serializing renders through a queue, sanitizing the
React `useId()` render id, skipping redundant re-renders, and resolving the
component path from `import.meta.dirname` under ESM.
