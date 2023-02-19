# Modal React Component

This is a simple modal React component that you can use in your projects.

## Installation

You can install the component using npm:

npm install --save react-modal

## Usage

To use the modal component, you need to import it into your React project:

```jsx
import { Modal } from "react-modal-oc";

<Modal isOpen={true} onRequestClose={() => setIsOpen(false)}>
  <h2>Modal Title</h2>
  <p>Modal content goes here.</p>
</Modal>;
```

The isOpen prop controls whether the modal is visible or hidden, and the onRequestClose prop is a function that will be called when the user clicks outside the modal or presses the escape key.

You can customize the style of the modal and its content by passing in style and contentStyle props respectively.

```jsx
<Modal
  isOpen={true}
  onRequestClose={() => setIsOpen(false)}
  style={{ backgroundColor: "rgba(0, 0, 0, 0.5)" }}
  contentStyle={{ padding: "40px" }}
>
  <h2>Modal Title</h2>
  <p>Modal content goes here.</p>
</Modal>
```

## Props

| Name           | Type     | Default Value | Description                                     |
| -------------- | -------- | ------------- | ----------------------------------------------- |
| isOpen         | boolean  | false         | Determines whether the modal is open or closed. |
| onRequestClose | function | undefined     | Function to close the modal.                    |
| style          | object   | {}            | Style object for the modal container.           |
| contentStyle   | object   | {}            | Style object for the modal content container.   |
