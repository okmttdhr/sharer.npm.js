[Sharer.npm.js](https://github.com/okmttdhr/sharer.npm.js)
=========

[Sharer.npm.js](https://github.com/okmttdhr/sharer.npm.js) is the node package module for [Sharer.js](https://ellisonleao.github.io/sharer.js/). Checkout [the official docs page](https://ellisonleao.github.io/sharer.js/) for more info.

## Installing

```
npm install sharer.npm.js
```

## Usage

```javascript
import Sharer from 'sharer.npm.js';

const elm = document.querySelector('.sharer');
const sharer = new Sharer(elm);
sharer.share();
```

Using from React.

```javascript
import React from 'react';
import Sharer from 'sharer.npm.js';

class Sample extends React.Component {
  handleClick(e) {
    const sharer = new Sharer(e.target);
    sharer.share();
  }

  render() {
    return (
      <div onClick={::this.handleClick}>
        <button className='sharer button' data-sharer='twitter' data-title='Checkout Sharer.npm.js!' data-url='https://github.com/okmttdhr/sharer.npm.js'>Share on Twitter</button>
      </div>
    );
  }
}
```
