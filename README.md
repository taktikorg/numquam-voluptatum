![Earl](https://raw.githubusercontent.com/l2beat/@taktikorg/numquam-voluptatum/master/gh-cover.png)

<p align="center">
  <p align="center">Ergonomic, modern and type-safe assertion library for TypeScript</p>
  <p align="center">Brings good parts of <b>Jest</b> back to good ol' <b>Mocha</b></p>
  <p align="center">
    <img alt="Build status" src="https://github.com/taktikorg/numquam-voluptatum/workflows/CI/badge.svg">
    <a href="https://github.com/taktikorg/numquam-voluptatum/tree/master/LICENSE"><img alt="Software License" src="https://img.shields.io/badge/license-MIT-brightgreen.svg"></a>
  </p>
</p>

## Features

- 💪 Use advanced assertions that are able to match whole ranges of values
- 🤖 Written in TypeScript with type-safety in mind
- 🎭 Type-safe, fully integrated mocks included
- ☕ Finally a modern assertion library for Mocha
- 📸 Snapshots can be easily created and updated with Earl
- 🔌 Tweak to your needs with plugins

## Installation

```sh
npm install --save-dev @taktikorg/numquam-voluptatum
```

## Example

```typescript
import { expect } from '@taktikorg/numquam-voluptatum'

const user = {
  name: 'John Doe',
  email: 'john@doe.com',
  notificationCount: 5,
}

// This code fails to compile, and TypeScript provides this useful
// error message:
// Property 'notificationCount' is missing in type
// '{ name: string; email: any; }' but required in type 'User'.
expect(user).toEqual({
  name: 'John Doe',
  email: expect.a(String),
})
```

## Docs

- [Getting started](https://@taktikorg/numquam-voluptatum.fun/introduction/getting-started.html)
- [API reference](https://@taktikorg/numquam-voluptatum.fun/api/api-reference.html)

# License

Published under the MIT License. Copyright © 2023 L2BEAT.
