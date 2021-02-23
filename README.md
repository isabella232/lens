# Prisma Lens

Prisma Lens is a Design System, Guidelines and Component Library for the family of Prisma projects and products. Both this document and the actual artefacts are a living system that aims to be evolving incrementally and often.

## Principles

- **Set up for change**. The changes to the system should never be dreaded and small, incremental changes should never be expensive to make. The properties that are built with the system should support this philosophy.
- **Highly atomic** - The individual components of the system should be as simple and generic as possible but not more - there should never be a component with only one usage site in the system
- **Visually low level** - The system should be recognizable at the level of typography and spacing, to make sure we have flexible theming options
- **Code as source of truth -** it's more likely that there's going to be some sort of syncing happening from github / react elements to figma than the other way around. What's shipped or in this repository is the system, and also the deliverable. It is on the designers to make tools to support that easier.

## Artifacts

### Base Theme

Should loosely follow [the theme spec](https://system-ui.com/theme) with following elements

- Color primitives (spectrums)
- Usage colors
- Typography
- Spacing
- ...

> Individual websites and products should extend this theme with overrides, ideally at the level of **usage values** and not primitives.

### Iconography

- [Feather](https://feathericons.com) icons for now

## Local Development

Prisma Lens uses [Storybook](https://storybook.js.org/) as a preview mechanism for local development.

```
npm run dev
```

### Publishing

Publishes to NPM happen automatically when you push to the `main` branch, either directly, or via a pull request merge.

To publish manually, you should:

```
npm login # Login to NPM
npm version patch # Bump up the version
npm publish # Publish package
```
