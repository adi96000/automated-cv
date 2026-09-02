# Aditya Yarramsetty's resume

[![Release](https://img.shields.io/github/release/adi96000/automated-cv.svg?style=flat)](https://github.com/adi96000/automated-cv/releases/latest)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](./LICENSE)
[![Build status](https://img.shields.io/github/actions/workflow/status/adi96000/automated-cv/general.yaml?style=flat)](https://github.com/adi96000/automated-cv/actions?query=workflow%3Ageneral)
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg?style=flat)](https://github.com/semantic-release/semantic-release)

My resume written in LaTeX based on [Awesome-CV](https://github.com/posquit0/Awesome-CV) with a complete CI/CD pipeline. Fully automated testing, building & release process is powered by GitHub Actions & [semantic-release](https://github.com/semantic-release/semantic-release). The output PDF can be found in the [releases section](https://github.com/adi96000/automated-cv/releases/latest).

## Download: [resume.pdf](https://adi96000.github.io/automated-cv/resume.pdf)

## Local Development

### Setup

The following tools are recommended for local work:

- `git`: `>=2`
- Build: TeX Live with `latexmk` (LuaLaTeX) **or** Docker (`>=18.09`) for a containerized build
- Tests: Node.js `>=16` to install and run Prettier locally
- `make` (standard on macOS/Linux)

Clone the repository:

```shell
git clone https://github.com/adi96000/automated-cv.git
```

Install local dev tools (Prettier):

```shell
npm install
```

### Test & Build Locally

- format (write): `npm run format`
- format (check): `npm run format:check`
- test: `make test` (runs Prettier; set `RUN_SUPER_LINTER=1` to run super-linter via Docker)
- build: `make build` (uses local `latexmk` when available, otherwise Docker)
- run test & build: `make all`

## Credits

The list of some third party components used in this project, with due credits to their authors and license terms. More details can be found in their README documentations.

- [posquit0/Awesome-CV](https://github.com/posquit0/Awesome-CV)
- [xu-cheng/latex-action](https://github.com/xu-cheng/latex-action)

Forked from [ezpzbz/automated-cv](https://github.com/ezpzbz/automated-cv), itself forked from `https://github.com/kirintwn/resume`.