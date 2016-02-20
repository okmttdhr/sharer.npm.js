[Sharer.npm.js](https://www.npmjs.com/package/sharer.npm.js)
=========

[Sharer.npm.js](https://www.npmjs.com/package/sharer.npm.js) is the node package module for [Sharer.js](https://ellisonleao.github.io/sharer.js/). Checkout [the official docs page](https://ellisonleao.github.io/sharer.js/) for more info.

## Installing

```
npm install sharer.npm.js
```

## Usage

(sample using with react)

```javascript
import Sharer from 'sharer.npm.js';

class Sample extends React.Component {
  handleClick(e) {
    const sharer = new Sharer(e.target)
    sharer.share()
  }

  render() {
    return (
      <button
        onClick={::this.handleClick}
        className='sharer button'
        data-sharer='twitter'
        data-title='Checkout Sharer.js!'
        data-url='https://ellisonleao.github.io/sharer.js/'>
        Share on Twitter
      </button>
    )
  }
}
```
