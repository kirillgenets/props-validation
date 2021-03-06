# About **react-props-validator** package

This is the HOC for validation prop-types in React.
You can use it like a simple high-ordered component.
When the error in prop-types occured user will see the PropTypesError component.

## Installation

With NPM:
```
npm i react-props-validator --save
```
Or with Yarn:
```
yarn add react-props-validator --save
```

## Usage

You can simply use it as any other HOC.
Just like that:
```
import propTypesChecker from '../hoc/propTypesChecker';
...
export default propTypesChecker(<ComponentName>);
```

You must set prop ```errorBoundary``` to the component you want to check - it must be a Component/Node that will render instead of the component with wrong props.<br/>
This errorBoundary component can receive ```errors``` prop which is the array of PropTypes error messages.

## Examples

Example of ErrorBoundary you can find there: [PropTypesError](https://github.com/kirillgenets/react-props-validator/tree/master/src/components/PropTypesError/PropTypesError.jsx)<br/>
Example of usage the HOC you can find there: [PropTypesError](https://github.com/kirillgenets/react-props-validator/tree/master/src/components/Example/Example.jsx).
