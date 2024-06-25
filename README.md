## Package_modal

    A simple and customizable modal component for React.



## Installation

You can install `package_modal` using npm:

```bash
  npm install @enkiduh/package_modal
```

## Demo

```markdown
Here's an example of how to use the `Modal` component in your React application:
```
```jsx
import React, { useState } from 'react';
import Modal from '@enkiduh/package_modal';

function App() {
  const [isFormSubmitted, setIsFormSubmitted] = useState(false);
  const [isFormCompleted, setIsFormCompleted] = useState(false);
  const [isClickedToClose, setIsClickedToClose] = useState(false);

  const handleClick = () => {
    setIsClickedToClose(true);
  };

  return (
    <div>
      <button onClick={() => setIsFormSubmitted(true)}>Show Modal</button>
      <Modal
        isFormSubmitted={isFormSubmitted}
        isFormCompleted={isFormCompleted}
        onClick={handleClick}
        isClickedToClose={isClickedToClose}
        modalBorder="2px solid black"
        modalBackground="rgb(168, 168, 168)"
        choiceOne="Form Completed"
        choiceOneBackground="rgb(78, 129, 78)"
        choiceOneColor="white"
        choiceOneFontSize="36px"
        choiceTwo="Form Not Completed"
        choiceTwoBackground="rgb(142, 83, 83)"
        choiceTwoColor="white"
        choiceTwoFontSize="36px"
      />
    </div>
  );
}

export default App;
```

## Styling

    You can customize the appearance of the modal by passing the appropriate CSS values as props.


## Props


The `Modal` component accepts the following props:

| Prop Name            | Type     | Description                                                                |
|----------------------|----------|----------------------------------------------------------------------------|
| `isFormSubmitted`    | `bool`   | Determines whether the form has been submitted.                            |
| `isFormCompleted`    | `bool`   | Determines whether the form has been completed.                            |
| `isClickedToClose`   | `bool`   | Determines whether the modal should be closed.                             |
| `onClick`            | `func`   | Function to handle the click event on the close button.                    |
| `modalBorder`        | `string` | CSS value for the border of the modal.                                     |
| `modalBackground`    | `string` | CSS value for the background of the modal.                                 |
| `choiceOne`          | `string` | Text for the choice when the form is completed.                            |
| `choiceOneBackground`| `string` | CSS value for the background of the choice when the form is completed.     |
| `choiceOneColor`     | `string` | CSS value for the text color of the choice when the form is completed.     |
| `choiceOneFontSize`  | `string` | CSS value for the font size of the choice when the form is completed.      |
| `choiceTwo`          | `string` | Text for the choice when the form is not completed.                        |
| `choiceTwoBackground`| `string` | CSS value for the background of the choice when the form is not completed. |
| `choiceTwoColor`     | `string` | CSS value for the text color of the choice when the form is not completed. |
| `choiceTwoFontSize`  | `string` | CSS value for the font size of the choice when the form is not completed.  |

## License

[MIT](https://choosealicense.com/licenses/mit/)


## Authors

- [@Enkiduduh](https://www.github.com/Enkiduduh)
