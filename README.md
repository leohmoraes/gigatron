<h1 align="center">
<br>
  <a href="https://github.com/FotonTech/gigatron"><img src="https://i.imgur.com/LVlSk6u.gif" alt="Gigatron" width=228"></a>
<br>
Gigatron
</h1>

<p align="center">The best boilerplate for your Monorepo Fullstack projects</p>

<p align="center">
  <a href="http://makeapullrequest.com">
    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="PRs Welcome">
  </a>
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square" alt="License MIT">
  </a>
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square" alt="">
  </a>
</p>

<hr />

## Introduction

This boilerplate contains all you need to start your next monorepo Fullstack project.

## Getting started

1. Clone this repo using `https://github.com/FotonTech/gigatron.git`
2. Move to the appropriate directory: `cd gigatron`.<br />
3. Run `yarn` to install dependencies.<br />
4. Creat `.env` file in `./packages/server` with `MONGOOSE=mongo_url`<br />

## Commands

- `npm start` - start the app, server and web.

## Adding React Native Deps

- If you add native dependencies that don't begin with `react-native-` add them to workspaces.nohoist in the root packages.json, with the globs below:

```json
// example with foobar package
// foobar doesn't match `react-native-` so we need to add manually to nohoist
// react-native-foobar would be fine though!
    "workspaces": {
        "nohoist": [
            "**/foobar",
            "**/foobar/**",
        ]
    },

```

## Linking

- Since most of the app is built on `/shared` you may need to add a dependency with native code on `/shared`. If you do copy it over to `/app` and link it with `react-native link your-dep-name-here`


## Next features:

- [ ] **Now serverless auto deployment**: Better HMR support;

## License

MIT license, Copyright (c) 2019 Foton.

## Contributors

Thanks goes to these wonderful people ([emoji key](https://github.com/all-contributors/all-contributors#emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
| [<img src="https://avatars0.githubusercontent.com/u/13947203?v=4" width="100px;" alt="Jabur"/><br /><sub><b>Jabur</b></sub>](https://github.com/jaburcodes)<br />[💬](#question-jaburcodes "Answering Questions") [🐛](https://github.com/FotonTech/gigatron/issues?q=author%3Ajaburcodes "Bug reports") [💻](https://github.com/FotonTech/gigatron/commits?author=jaburcodes "Code") [🎨](#design-jaburcodes "Design") [📖](https://github.com/FotonTech/gigatron/commits?author=jaburcodes "Documentation") [💡](#example-jaburcodes "Examples") [🤔](#ideas-jaburcodes "Ideas, Planning, & Feedback") [🚇](#infra-jaburcodes "Infrastructure (Hosting, Build-Tools, etc)") [👀](#review-jaburcodes "Reviewed Pull Requests") | [<img src="https://avatars0.githubusercontent.com/u/15015324?s=460&v=4" width="100px;" alt="Thom"/><br /><sub><b>Thom</b></sub>](https://github.com/thomazella)<br />[💻](https://github.com/FotonTech/gigatron/commits?author=thomazella "Code") [🤔](#ideas-thomazella "Ideas, Planning, & Feedback") [👀](#review-thomazella "Reviewed Pull Requests") | [<img src="https://avatars1.githubusercontent.com/u/7690649?v=4" width="100px;" alt="paulogdm"/><br /><sub><b>paulogdm</b></sub>](https://paulogdm.com)<br />[💬](#question-paulogdm "Answering Questions") [💻](https://github.com/FotonTech/gigatron/commits?author=paulogdm "Code") [🤔](#ideas-paulogdm "Ideas, Planning, & Feedback") [🚇](#infra-paulogdm "Infrastructure (Hosting, Build-Tools, etc)") [📦](#platform-paulogdm "Packaging/porting to new platform") [🔌](#plugin-paulogdm "Plugin/utility libraries") [🛡️](#security-paulogdm "Security") [🔧](#tool-paulogdm "Tools") |
| :---: | :---: | :---: |
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
