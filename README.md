# awesome-js-zerodep

Awesome JavaScript &amp; TypeScript modules which have zero dependencies. Well, almost zero, if it have *1* but really good, list it here.

You can check your project for used packages which have zero dependencies with this bash script:

```bash
for N in $(npm list --omit peer --omit dev --omit optional --depth 0 --json | jq ".dependencies" | jq 'keys[]' -r); do COUNT=$(cat node_modules/$N/package.json | jq ".dependencies" | jq length); if [ "$COUNT" == "0" ]; then echo $N; fi; done
```

#### Generate the line automagically 🪄

Use this script: https://gist.github.com/huksley/0e681e12de92951c7c9d9e83d8e9dbd8

### React & Web

| summary | npm | repo | package | types | dependency count | last update |
| - | - | - | - | - | - | - |
| Useful hooks for React | `npm i usehooks-ts` | [GitHub](https://github.com/juliencrn/usehooks-ts) | [![https://img.shields.io/badge/npm/v/usehooks-js-blue](https://img.shields.io/npm/v/usehooks-ts?label=usehooks-ts)](https://npmjs.com/package/usehooks-ts) | ![types](https://badgen.net/npm/types/usehooks-ts) | ![dependenices](https://badgen.net/bundlephobia/dependency-count/usehooks-ts?label=usehooks-ts) | ![last update](https://badgen.net/github/last-commit/juliencrn/usehooks-ts) |
| Modern fetch for web | `npm i swr` | [GitHub](https://github.com/vercel/swr) | [![https://img.shields.io/badge/npm/v/swr-blue](https://img.shields.io/npm/v/swr?label=swr)](https://npmjs.com/package/swr) | ![types](https://badgen.net/npm/types/swr) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/swr?label=swr)](https://bundlephobia.com/package/swr) | [![last update](https://badgen.net/github/last-commit/vercel/swr)](https://github.com/vercel/swr) |
| Date time utils | `npm i date-fns` | [GitHub](https://github.com/date-fns/date-fns) | [![https://img.shields.io/badge/npm/v/date-fns-blue](https://img.shields.io/npm/v/date-fns?label=date-fns)](https://npmjs.com/package/date-fns) | ![types](https://badgen.net/npm/types/date-fns) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/date-fns?label=date-fns)](https://bundlephobia.com/package/date-fns) | [![last update](https://badgen.net/github/last-commit/)](https://github.com/date-fns/date-fns) |
| Functional utils | `npm i ramda` | [GitHub](https://github.com/ramda/ramda) | [![https://img.shields.io/badge/npm/v/ramda-blue](https://img.shields.io/npm/v/ramda?label=ramda)](https://npmjs.com/package/ramda) | ![types](https://badgen.net/npm/types/ramda) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/ramda?label=ramda)](https://bundlephobia.com/package/ramda) | [![last update](https://badgen.net/github/last-commit/ramda/ramda)](https://github.com/ramda/ramda) |
| Data validator | `npm i validator` | [GitHub](https://github.com/validatorjs/validator) | [![https://img.shields.io/badge/npm/v/validator-blue](https://img.shields.io/npm/v/validator?label=validator)](https://npmjs.com/package/validator) | ![types](https://badgen.net/npm/types/validator) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/validator?label=validator)](https://bundlephobia.com/package/validator) | [![last update](https://badgen.net/github/last-commit/validatorjs/validator)](https://github.com/validatorjs/validator) |
| ID generator | `npm i nanoid` | [GitHub](https://github.com/ai/nanoid) | [![https://img.shields.io/badge/npm/v/nanoid-blue](https://img.shields.io/npm/v/nanoid?label=nanoid)](https://npmjs.com/package/nanoid) | ![types](https://badgen.net/npm/types/nanoid) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/nanoid?label=nanoid)](https://bundlephobia.com/package/nanoid) | [![last update](https://badgen.net/github/last-commit/ai/nanoid)](https://github.com/ai/nanoid) |
| Compare objects | `npm i dequal` | [GitHub](https://github.com/lukeed/dequal) | [![https://img.shields.io/badge/npm/v/dequal-blue](https://img.shields.io/npm/v/dequal?label=dequal)](https://npmjs.com/package/dequal) | ![types](https://badgen.net/npm/types/dequal) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/dequal?label=dequal)](https://bundlephobia.com/package/dequal) | [![last update](https://badgen.net/github/last-commit/lukeed/dequal)](https://github.com/lukeed/dequal) |
| Compare versions | `npm i compare-versions` | [GitHub](https://github.com/omichelsen/compare-versions) | [![https://img.shields.io/badge/npm/v/compare-versions-blue](https://img.shields.io/npm/v/compare-versions?label=compare-versions)](https://npmjs.com/package/compare-versions) | ![types](https://badgen.net/npm/types/compare-versions) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/compare-versions?label=compare-versions)](https://bundlephobia.com/package/compare-versions) | [![last update](https://badgen.net/github/last-commit/omichelsen/compare-versions)](https://github.com/omichelsen/compare-versions) |
| Good offline font | `npm i @fontsource/open-sans` | [GitHub](https://github.com/fontsource/fontsource) | [![https://img.shields.io/badge/npm/v/@fontsource/open-sans-blue](https://img.shields.io/npm/v/@fontsource/open-sans?label=@fontsource/open-sans)](https://npmjs.com/package/@fontsource/open-sans) | ![types](https://badgen.net/npm/types/@fontsource/open-sans) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/@fontsource/open-sans?label=@fontsource/open-sans)](https://bundlephobia.com/package/@fontsource/open-sans) | [![last update](https://badgen.net/github/last-commit/fontsource/fontsource)](https://github.com/fontsource/fontsource) |
| Converts markdown to JSX | `npm i markdown-to-jsx` | [GitHub](https://github.com/probablyup/markdown-to-jsx) | [![https://img.shields.io/badge/npm/v/markdown-to-jsx-blue](https://img.shields.io/npm/v/markdown-to-jsx?label=markdown-to-jsx)](https://npmjs.com/package/markdown-to-jsx) | ![types](https://badgen.net/npm/types/markdown-to-jsx) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/markdown-to-jsx?label=markdown-to-jsx)](https://bundlephobia.com/package/markdown-to-jsx) | [![last update](https://badgen.net/github/last-commit/probablyup/markdown-to-jsx)](https://github.com/probablyup/markdown-to-jsx) |
| Typed javascript | `npm i typescript` | [GitHub](https://github.com/Microsoft/TypeScript) | [![https://img.shields.io/badge/npm/v/typescript-blue](https://img.shields.io/npm/v/typescript?label=typescript)](https://npmjs.com/package/typescript) | ![types](https://badgen.net/npm/types/typescript) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/typescript?label=typescript)](https://bundlephobia.com/package/typescript) | [![last update](https://badgen.net/github/last-commit/Microsoft/TypeScript)](https://github.com/Microsoft/TypeScript) |
| useInView hook to detect when element is in view | `npm i react-intersection-observer` | [GitHub](https://github.com/thebuilder/react-intersection-observer) | [![https://img.shields.io/badge/npm/v/react-intersection-observer-blue](https://img.shields.io/npm/v/react-intersection-observer?label=react-intersection-observer)](https://npmjs.com/package/react-intersection-observer) | ![types](https://badgen.net/npm/types/react-intersection-observer) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/react-intersection-observer?label=react-intersection-observer)](https://bundlephobia.com/package/react-intersection-observer) | [![last update](https://badgen.net/github/last-commit/thebuilder/react-intersection-observer)](https://github.com/thebuilder/react-intersection-observer) |
| NextJS state in querystring | `npm i next-query-state` | [GitHub](https://github.com/youha-info/next-query-state) | [![https://img.shields.io/badge/npm/v/next-query-state-blue](https://img.shields.io/npm/v/next-query-state?label=next-query-state)](https://npmjs.com/package/next-query-state) | ![types](https://badgen.net/npm/types/next-query-state) | [![dependencies](https://badgen.net/bundlephobia/dependency-count/next-query-state?label=next-query-state)](https://bundlephobia.com/package/next-query-state) | [![last update](https://badgen.net/github/last-commit/youha-info/next-query-state)](https://github.com/youha-info/next-query-state) |
