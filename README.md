# react-social

> Simple [React](http://facebook.github.io/react/index.html) components for
> social (Facebook, Twitter and Pinterest) buttons and social counts.

## Install

```bash
npm install react-tagsinput --save
```

## Example

```javascript
var FacebookButton = require("./react-social").FacebookButton
  , FacebookCount = require("./react-social").FacebookCount;

var App = React.createClass({
  render: function () {
    var url = "https://github.com";

    return (
      <FacebookButton url={url}>
        <FacebookCount url={url} />
        {" Share " + url}
      </FacebookButton>
    );
  }
});
```

## Button (FacebookButton, TwitterButton, PinterestButton) API

### Props

##### url

The url you want to share, default is `window.location`.

##### media (required for Pinterest)

Url of an image, required for PinterestButton.

## Count (FacebookCount, TwitterCount, PinterestCount) API

### Props

##### url

The url you want to get the count of, default is `window.location`.

### Methods

##### getCount()

Return the social count.

---

MIT Licensed