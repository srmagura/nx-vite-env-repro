# nx-vite-env-repro

Repro instructions are as follows.

## Development

1. `cd packages/my-app`
2. `npm run dev`

--> App shows "VITE_FOOBAR = development"

## Production without Nx

1. `cd packages/my-app`
2. `npm run build`
3. `npm run preview`

--> App shows "VITE_FOOBAR = production"

## Production with Nx

1. `npx nx run my-app:build`
2. `cd packages/my-app`
3. `npm run preview`

--> App shows "VITE_FOOBAR = development"
