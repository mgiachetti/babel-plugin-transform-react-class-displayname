# babel-plugin-transform-react-class-displayname
Babel plugin that injects class' name as `displayName` property.

## Install:

```
  npm i -D mgiachetti/babel-plugin-transform-react-class-displayname#master
```

## Usage:

via `.babelrc`

```
{
   "plugins": ["transform-react-class-displayname"],
}
```

## Example:

In:

```
  const component = class Class1 {

  };

  class Class2 {
   
  }
```

Out:

```
  const component = class Class1 {
    static displayName = "Class1";
  };

  class Class2 {
    static displayName = "Class2";
  }
```

