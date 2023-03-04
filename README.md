# awesome-js-zerodep

Awesome JavaScript &amp; TypeScript modules which have zero dependencies.

You can check your project for used packages which have zero dependencies with this bash script:

```bash
for N in $(npm list --omit peer --omit dev --omit optional --depth 0 --json | jq ".dependencies" | jq 'keys[]' -r); do COUNT=$(cat node_modules/$N/package.json | jq ".dependencies" | jq length); if [ "$COUNT" == "0" ]; then echo $N; fi; done
```

### React & Web

| npm | source | package | types | dependency count | last update |
| - | - | - | - | - | - |
| `npm i usehooks-ts` | [GitHub](https://github.com/juliencrn/usehooks-ts) | [![https://img.shields.io/badge/npm/v/usehooks-js-blue](https://img.shields.io/npm/v/usehooks-ts?label=usehooks-ts)](https://npmjs.com/package/usehooks-ts) | ![types](https://badgen.net/npm/types/usehooks-ts) | ![dependenices](https://badgen.net/bundlephobia/dependency-count/usehooks-ts?label=usehooks-ts) | ![last update](https://badgen.net/github/last-commit/juliencrn/usehooks-ts) |

