# react-safe-storage

> Local storage with encryption

[![NPM](https://img.shields.io/npm/v/react-safe-storage.svg)](https://www.npmjs.com/package/react-safe-storage) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

```bash
npm install --save react-safe-storage
```

## Dependencies

This module is pure javascript code and does not have any depencencies


## Security

It is a simple cipher based utility and does not guarantee military grade security. But it does not have any dependencies on any external library and does the job.

## Configuration

This component needs a secret passphrase that is used for ciphering and deciphering. Ideally, the secret passphrase should come from environment variables.

## Functionality

```jsx

/*

secret_passphrase: secret password used for ciphering & deciphering
key: key for local storage
value: value to be stored in local storage for the specified key

*/

setItem('secret_passphrase', 'key', 'value') {}
getItem('secret_passphrase', 'key') {}

```


## Usage

```jsx

import React from 'react'

import { getItem, setItem } from 'react-safe-storage'

const App = () => {

  setItem('secret_passphrase', 'email', 'hrus********e@gmail.com')
  console.log(getItem('secret_passphrase', 'email'));

  return <div>Hello Safe Storage</div>
}

export default App

```

## License

MIT © [superflows-dev](https://github.com/superflows-dev)
