# Dragon

Dragon is the umbrella workspace that converges the strongest pieces already present on `D:\`:

- `qflush` as the control plane
- `A11` as the multimodal feature reference
- `a11ba` and `a11frontend` as cleaner extraction candidates
- Funesterie libraries as reusable platform modules

## Workspace

- `apps/dragon-daemon` control-plane oriented service
- `apps/dragon-api` product-facing API shell
- `apps/dragon-web` React cockpit
- `packages/contracts` shared types
- `packages/upstream` manifest loading and local ecosystem probing

## Scripts

```bash
npm install
npm run dev
npm run build
npm run typecheck
```

## Default ports

- `dragon-api`: `4600`
- `dragon-daemon`: `4700`
- `dragon-web`: `5174`

## Notes

This phase intentionally wraps upstream projects instead of copying their business logic.
The goal is to create a stable Dragon shell first, then promote validated slices from `qflush`, `A11`, `a11ba`, and `a11frontend`.
