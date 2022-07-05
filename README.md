# Vue 3 + TypeScript + Vite

this repo represents an issue of `vite-plugin-vue-type-imports`

## Reproduce

- yarn install
- yarn dev
- open the website, and then you will see
> "[@vue/compiler-sfc] type argument passed to defineProps() must be a literal type, or a reference to an interface or literal type"

- update `HelloWorld.vue`, import `MsgProps` from `msg` instead of `types`.
- it works ok.

## Conclusion
- CAN NOT import types from entry file with multiple exports levels (like `types.ts`)
