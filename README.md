# React-Marcat-Dropdown

## Requirements

Before getting started, make sure you have the following installed:

- Node.js: [Download and install Node.js](https://nodejs.org) (v15min)
- React : [Install and install React](https://react.dev)

## Used

Styled-component was used on this project, please check if there are any compatibility issues before importing the component.

## Installation

Install this package:

```shell
npm install react-marcat-dropdown
```

Import the DropdownInput component:

```js
import DropdownInput  from "react-marcat-dropdown/dropdown";
```

## Description
This component renders a custom dropdown input that can be used to select one option from a list of options. The component is implemented using styled-components and is fully customizable.

## Props

- `name`: string (required) - The name of the input.
- `data`: string[] (required) - An array of strings that represents the list of options.
- `personnalId`: string (optional) - Id for the selector.
- `defaultText`: string (optional) - The default text that appears in the dropdown before an option is selected.
- `fontSize`: string (optional) - The font size for the dropdown. Defaults to "1em".
- `color`: string (optional) - The color of the selected option text. Defaults to "rgba(0,0,0,0.25)".
- `borderColor`: string (optional) - The color of the dropdown border. Defaults to "1px solid rgba(0,0,0,0.25)".
- `borderRadius`: string (optional) - The border radius of the dropdown. Defaults to "5px".
- `scrollBarBackgroundColor`: string (optional) - The background color of the scrollbar. Defaults to "rgba(0,0,0,0.25)".
- `scrollBarThumbColor`: string (optional) - The color of the scrollbar thumb. Defaults to "rgba(0,0,0,0.5)".
- `scrollBarWidth`: string (optional) - The width of the scrollbar. Defaults to "8px".
- `scrollBarRadius`: string (optional) - The border radius of the scrollbar. Defaults to "10px".
- `selectBoxColor`: string (optional) - The background color of the dropdown options. Defaults to "#ffffff".
- `selectBoxOptionsColor`: string (optional) - The color of the dropdown options text. Defaults to "rgba(0,0,0,0.25)".
- `labelled`: boolean (optional) - Whether to include a label for the input. Defaults to false.

## State

The component uses the `useState` hook to keep track of the selected option. When an option is selected, the state is updated accordingly.

## Functions

- `handleChange`: This function is called whenever the selected option changes. It updates the state with the new selected option.

## Usage

```tsx
import React from 'react';
import DropdownInput  from "react-marcat-dropdown/dropdown";

const options = ['Option 1', 'Option 2', 'Option 3'];

const MyComponent = () => {
  return (
    <DropdownInput
      name="myDropdown"
      data={options}
      defaultText="Select an option"
      color="red"
      borderColor="2px solid red"
      borderRadius="10px"
      scrollBarBackgroundColor="#f0f0f0"
      scrollBarThumbColor="#c5c5c5"
      scrollBarWidth="12px"
      scrollBarRadius="20px"
      selectBoxColor="#ebebeb"
      selectBoxOptionsColor="#333333"
      labelled
      personnalId="selector"
      fontSize="1em"
      required
    />
  );
};
```

In the above example, a `DropdownInput` component is rendered with some custom props. The `options` array is passed as the `data` prop to populate the dropdown. The `defaultText`, `color`, `borderColor`, `borderRadius`, `scrollBarBackgroundColor`, `scrollBarThumbColor`, `scrollBarWidth`, `scrollBarRadius`, `selectBoxColor`, and `selectBoxOptionsColor` props are used to customize the appearance of the dropdown. Finally, the `labelled` prop is set to `true` to include a label for the input.
