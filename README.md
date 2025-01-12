# Text Mixer: Mixed Caps Text Generator

A web application that takes user input and randomly converts the text to mixed uppercase and lowercase letters. This project is a fun way to create text with a quirky style for memes, captions, or other creative uses.

## Features

- Accepts user input through a text area.
- Randomly converts each character to uppercase or lowercase.
- Displays the mixed caps result dynamically.
- Clean and responsive design for a better user experience.

## Demo

You can try out the application live by opening the `index.html` file in any modern web browser.

## How to Use

1. Clone this repository or download the `index.html` file.
2. Open the `index.html` file in your browser.
3. Enter the text you want to transform in the text area.
4. Click the **Generate** button to see the mixed caps text appear below.

## Code Explanation

### HTML Structure

The HTML file includes:
- A `textarea` element for user input.
- A `button` element to trigger the mixed caps generation.
- A `div` element to display the output.

### CSS Styling

- A simple, responsive design using CSS.
- Text area and button are styled for usability and clarity.

### JavaScript Functionality

The main functionality is implemented in JavaScript:
```javascript
function generateMixedCaps() {
  const inputText = document.getElementById('inputText').value;
  let mixedText = '';

  for (let char of inputText) {
    if (Math.random() > 0.5) {
      mixedText += char.toUpperCase();
    } else {
      mixedText += char.toLowerCase();
    }
  }

  document.getElementById('outputText').textContent = mixedText;
}
```

This function:
- Reads the user input from the `textarea`.
- Iterates over each character in the string.
- Randomly converts each character to uppercase or lowercase.
- Updates the output `div` with the transformed text.

## Requirements

- A modern web browser (Chrome, Firefox, Safari, Edge, etc.)
- No external dependencies or libraries are required.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/text-mixer.git
   ```
2. Navigate to the project directory:
   ```bash
   cd text-mixer
   ```
3. Open the `index.html` file in your preferred browser.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue if you have ideas for improvement or find any bugs.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
