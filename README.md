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

## Usage

```jsx

import React from 'react'

import { getItem, setItem } from 'react-safe-storage'

const App = () => {

  setItem('sdfsdf23434sd#4', 'email', 'hrus********e@gmail.com')
  console.log(getItem('sdfsdf23434sd#4', 'email'));

  return <div>Hello Safe Storage</div>
}

export default App

```

## License

MIT © [superflows-dev](https://github.com/superflows-dev)
