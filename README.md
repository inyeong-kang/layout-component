# jero-payments-modal

> A library to design common components built in React & TypeScript

## Overview

- You can use this library when designing common components, especially for layout.
- Just Install, Import and Then Use it!

## Version

> Latest version: 0.1.0 (updated in 2023.09.18)

- Major package version
  - "react": "^18.2.0"
  - "react-dom": "^18.2.0"
  - "@emotion/react": "^11.11.1"
  - "@emotion/styled": "^11.11.0"
  - "typescript": "^5.2.2"

## How to Use

### Installation

```Shell
npm i jero-design-system
```

### Import Package

- If you wanna use all components, import all components from this package.

```
import { Button, Container, Grid, Flex } from 'jero-design-system';
```

- If you wanna use specific components, import them from this package.

```JavaScript
import { Button, Flex } from 'jero-design-system';
```

## Package Structure

```
📦jero-design-system
 ┣ 📂dist
 ┃ ┣ 📂Button
 ┃ ┃ ┣ 📜index.d.ts
 ┃ ┃ ┗ 📜index.js
 ┃ ┣ 📂Container
 ┃ ┃ ┣ 📜index.d.ts
 ┃ ┃ ┗ 📜index.js
 ┃ ┣ 📂Flex
 ┃ ┃ ┣ 📜index.d.ts
 ┃ ┃ ┗ 📜index.js
 ┃ ┣ 📂Grid
 ┃ ┃ ┣ 📜index.d.ts
 ┃ ┃ ┗ 📜index.js
 ┃ ┣ 📜index.d.ts
 ┃ ┗ 📜index.js
 ┣ 📜package.json
 ┣ 📜README.md
 ┗ 📜tsconfig.node.json
```

## Component & Props

### Container

<img src="./public/img/jero-container.png"/>

```JavaScript
import { Container } from 'jero-design-system';

function App() {
  return (
    <div className='App'>
      <h1>Container</h1>
      <Container
        maxWidth='900px'
        minWidth='300px'
        height='30vh'
        backgroundColor='#E7E7E7'
      >
        This is Container
        <p>Hello Nice to Meet U</p>
        <h3>How are you?</h3>
        <h4>I'm fine, thanks!</h4>
      </Container>
    </div>
  );
}
```

| props name      | props type        | props description                                        |
| --------------- | ----------------- | -------------------------------------------------------- |
| maxWidth        | `string`          | Max-width of Container (ex. '600px'), **required props** |
| minWidth        | `string`          | Min-width of Container (ex. '300px')                     |
| height          | `string`          | Height of Container (ex '90vh')                          |
| backgroundColor | `string`          | background-color of Container (ex 'gray')                |
| children        | `React.ReactNode` | Element or Node of Container                             |

### Grid

<img src="./public/img/jero-grid.png"/>

```JavaScript
import { Grid } from 'jero-design-system';

function App() {
  return (
    <div className='App'>
      <h1>Grid</h1>
      <Grid rows={2} columns={2} gap='5px' backgroundColor='#E7E7E7'>
        <div className='item'>Item 1</div>
        <div className='item'>Item 2</div>
        <div className='item'>Item 3</div>
        <div className='item'>Item 4</div>
      </Grid>
    </div>
  );
}
```

| props name      | props type        | props description                                   |
| --------------- | ----------------- | --------------------------------------------------- |
| rows            | `number`          | justify-content of Grid (ex. 4), **required props** |
| columns         | `nubmer`          | align-items of Grid (ex. 3), **required props**     |
| gap             | `string`          | gap of Grid (ex '10px')                             |
| backgroundColor | `string`          | background-color of Grid (ex 'gray')                |
| children        | `React.ReactNode` | Element or Node of Grid                             |

### Flex

<img src="./public/img/jero-flex.png"/>

```JavaScript
import { Flex } from 'jero-design-system';

function App() {
  return (
    <div className='App'>
      <h1>Flex</h1>
      <Flex direction='column' justify='space-between' align='center' gap='5px'>
        <div className='item'>Item 1</div>
        <div className='item'>Item 2</div>
        <div className='item'>Item 3</div>
        <div className='item'>Item 4</div>
      </Flex>
    </div>
  );
}
```

| props name      | props type        | props description                                          |
| --------------- | ----------------- | ---------------------------------------------------------- |
| direction       | `row, column`     | flex-direction of Flex (ex. '600px'), **required props**   |
| justify         | `string`          | justify-content of Flex (ex. 'center'), **required props** |
| align           | `string`          | align-items of Flex (ex '90vh'), **required props**        |
| gap             | `string`          | gap of Flex (ex '90vh')                                    |
| backgroundColor | `string`          | background-color of Flex (ex '90vh')                       |
| children        | `React.ReactNode` | Element or Node of Flex                                    |

### Button

<img src="./public/img/jero-button.png"/>

```JavaScript

import { Button, Flex } from 'jero-design-system';

function App() {
  return (
    <div className='App'>
      <h1>Button</h1>
      <Flex direction='row' gap='10px' justify='start' align='start'>
        <Button label='Primary' primary />
        <Button label='Secondary' />
        <Button label='Small' size='sm'></Button>
        <Button label='Medium' size='md'></Button>
        <Button label='Large' size='lg'></Button>
      </Flex>
    </div>
  );
}
```

| props name | props type         | props description                                            |
| ---------- | ------------------ | ------------------------------------------------------------ |
| primary    | `boolean`          | If a button is used in primary tasks, add `primary` props.   |
| size       | `'sm', 'md', 'lg'` | Adjust the size of Button, including font-size inside Button |
| label      | `string`           | Text of Button                                               |

## Source

- [Github Code](https://github.com/inyeong-kang/layout-component)
- [npm.js](https://www.npmjs.com/package/jero-design-system)

## Developer

- [jero-kang](https://github.com/inyeong-kang)
