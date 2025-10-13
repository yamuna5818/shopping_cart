## React Snippets

#### React Function StateLess

rf→

```js
import React from "react";
import PropTypes from "prop-types";

const Component = (props) => {
  return <div></div>;
};

Component.propTypes = {};

export { Component };
```

rfts→

```ts
import React from "react";

type Props = {};

const Component = (props: Props) => {
  return <div></div>;
};

export { Component };
```

#### React Function

rfs→

```js
import React, { useState } from "react";
import PropTypes from "prop-types";

const Component = (props) => {
  const [state, setState] = useState(InitialState);
  return <div></div>;
};

Component.propTypes = {};

export { Component };
```

rfsts→

```ts
import React from "react";

type Props = {};

const Component = (props: Props) => {
  const [state, setState] = useState<Type>(InitialState);
  return <div></div>;
};

export { Component };
```

#### useState

rs→

```js
const [state, setState] = useState(InitialState);
```

rsts→

```js
const [state, setState] = useState < Type > InitialState;
```

### useReducer

rur→

```js
const [state, dispatch] = useReducer(Reducer, InitialState, Init);
```

### useMemo

rum→

```js
const FunctionName = useMemo(FunctionImp, [UpdateParams]);
```

### useEffect

rue→

```js
useEffect(FunctionImp, [UpdateParams]);
```
