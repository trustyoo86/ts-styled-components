# ts-styled-components
Using typescript interface in [styled-components](https://www.npmjs.com/package/styled-components)

## Usage

### Install
```bash
npm i ts-styled-components --save
yarn add ts-styled-components
```

### Usage
```typescript
import withProps from 'ts-styled-components'

interface IProps {
  isTest: boolean,
}

const styles = {
  containers: withProps<IProps>()(styled.view)`
    width: ${(props) => props.isTest ? '600' : '200' }px;
  `
};
```