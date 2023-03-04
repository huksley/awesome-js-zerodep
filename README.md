# awesome-js-zerodep

Awesome JavaScript &amp; TypeScript modules which have zero dependencies.

You can check your project for used packages which have zero dependencies with this bash script:

```bash
for N in $(npm list --omit peer --omit dev --omit optional --depth 0 --json | jq ".dependencies" | jq 'keys[]' -r); do COUNT=$(cat node_modules/$N/package.json | jq ".dependencies" | jq length); if [ "$COUNT" == "0" ]; then echo $N; fi; done
```

### React & Web

| npm | repo | package | types | dependency count | last update |
| - | - | - | - | - | - |
| `npm i usehooks-ts` | [GitHub](https://github.com/juliencrn/usehooks-ts) | [![https://img.shields.io/badge/npm/v/usehooks-js-blue](https://img.shields.io/npm/v/usehooks-ts?label=usehooks-ts)](https://npmjs.com/package/usehooks-ts) | ![types](https://badgen.net/npm/types/usehooks-ts) | ![dependenices](https://badgen.net/bundlephobia/dependency-count/usehooks-ts?label=usehooks-ts) | ![last update](https://badgen.net/github/last-commit/juliencrn/usehooks-ts) |
| `npm i swr` | [GitHub](https://github.com/vercel/swr) | [![https://img.shields.io/badge/npm/v/swr-blue](https://img.shields.io/npm/v/swr?label=swr)](https://npmjs.com/package/swr) | ![types](https://badgen.net/npm/types/swr) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/swr?label=swr)](https://bundlephobia.com/package/swr) | [![last update](https://badgen.net/github/last-commit/vercel/swr)](https://github.com/vercel/swr) |
| `npm i date-fns` | [GitHub](https://github.com/date-fns/date-fns) | [![https://img.shields.io/badge/npm/v/date-fns-blue](https://img.shields.io/npm/v/date-fns?label=date-fns)](https://npmjs.com/package/date-fns) | ![types](https://badgen.net/npm/types/date-fns) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/date-fns?label=date-fns)](https://bundlephobia.com/package/date-fns) | [![last update](https://badgen.net/github/last-commit/)](https://github.com/date-fns/date-fns) |
| `npm i ramda` | [GitHub](https://github.com/ramda/ramda) | [![https://img.shields.io/badge/npm/v/ramda-blue](https://img.shields.io/npm/v/ramda?label=ramda)](https://npmjs.com/package/ramda) | ![types](https://badgen.net/npm/types/ramda) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/ramda?label=ramda)](https://bundlephobia.com/package/ramda) | [![last update](https://badgen.net/github/last-commit/ramda/ramda)](https://github.com/ramda/ramda) |
| `npm i validator` | [GitHub](https://github.com/validatorjs/validator) | [![https://img.shields.io/badge/npm/v/validator-blue](https://img.shields.io/npm/v/validator?label=validator)](https://npmjs.com/package/validator) | ![types](https://badgen.net/npm/types/validator) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/validator?label=validator)](https://bundlephobia.com/package/validator) | [![last update](https://badgen.net/github/last-commit/validatorjs/validator)](https://github.com/validatorjs/validator) |
| `npm i nanoid` | [GitHub](https://github.com/ai/nanoid) | [![https://img.shields.io/badge/npm/v/nanoid-blue](https://img.shields.io/npm/v/nanoid?label=nanoid)](https://npmjs.com/package/nanoid) | ![types](https://badgen.net/npm/types/nanoid) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/nanoid?label=nanoid)](https://bundlephobia.com/package/nanoid) | [![last update](https://badgen.net/github/last-commit/ai/nanoid)](https://github.com/ai/nanoid) |
| `npm i dequal` | [GitHub](https://github.com/lukeed/dequal) | [![https://img.shields.io/badge/npm/v/dequal-blue](https://img.shields.io/npm/v/dequal?label=dequal)](https://npmjs.com/package/dequal) | ![types](https://badgen.net/npm/types/dequal) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/dequal?label=dequal)](https://bundlephobia.com/package/dequal) | [![last update](https://badgen.net/github/last-commit/lukeed/dequal)](https://github.com/lukeed/dequal) |
| `npm i compare-versions` | [GitHub](https://github.com/omichelsen/compare-versions) | [![https://img.shields.io/badge/npm/v/compare-versions-blue](https://img.shields.io/npm/v/compare-versions?label=compare-versions)](https://npmjs.com/package/compare-versions) | ![types](https://badgen.net/npm/types/compare-versions) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/compare-versions?label=compare-versions)](https://bundlephobia.com/package/compare-versions) | [![last update](https://badgen.net/github/last-commit/omichelsen/compare-versions)](https://github.com/omichelsen/compare-versions) |
| `npm i @fontsource/open-sans` | [GitHub](https://github.com/fontsource/fontsource) | [![https://img.shields.io/badge/npm/v/@fontsource/open-sans-blue](https://img.shields.io/npm/v/@fontsource/open-sans?label=@fontsource/open-sans)](https://npmjs.com/package/@fontsource/open-sans) | ![types](https://badgen.net/npm/types/@fontsource/open-sans) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/@fontsource/open-sans?label=@fontsource/open-sans)](https://bundlephobia.com/package/@fontsource/open-sans) | [![last update](https://badgen.net/github/last-commit/fontsource/fontsource)](https://github.com/fontsource/fontsource) |
