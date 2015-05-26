# ngReact-with-transclude

Add transclude to [ngReact](https://github.com/davidchang/ngReact) library

# Installation

Install via Bower:

```
bower install git://github.com/huisenwu/ngReact-with-transclude.git
```

or via npm:

```
npm install git://github.com/huisenwu/ngReact-with-transclude.git
```

# Usage

For example, you want to use angular directive transcluded content as React children props.

hello.js
```
React.createClass({
  render: function() {
    return <h1>{this.props.children}</h1>;
  }
});
```
hi.js
```
React.createClass({
  render: function() {
    return <span>{this.props.children}</span>;
  }
});
```

```
<hello><hi>Hello World</hi></hello>
```
