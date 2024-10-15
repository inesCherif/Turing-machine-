# Turing Machine Simulator

## Description
This project is a web-based simulation of a Turing machine. The Turing machine operates on a tape of binary data using a set of predefined instructions. Users can interactively explore the Turing machine's behavior and experiment with different programs, such as:
- Replacing binary digits (0 → 1)
- Adding unary numbers
- Subtracting unary numbers
![Interface](images/interface)



## Features
- Simulate basic Turing machine operations such as replacing, adding, or subtracting binary digits.
- Predefined examples of Turing machine programs to quickly start with.
- Interactive user interface for controlling the tape, setting initial states, and manually stepping through the machine's operations.
- Customizable style and functionality to suit your needs.

## How to Use
1. Clone or download the repository to your local machine.
2. Open the `index.html` file in a browser to start using the Turing machine simulator.



## Technologies Used
- HTML
- CSS
- JavaScript



## Code Explanation
At the beginning of the code, you will find some styles. You can freely modify these styles as needed to change the appearance of the simulator.
```html
<style> ... </style>
```
The HTML page consists of two empty tables, which are dynamically generated using JavaScript to represent the tape and the program.



## Customization

You can easily customize both the appearance and functionality of the simulator:

### CSS Styling

To change the look and feel, modify the CSS rules in the `<style>` block located in the `<head>` section of the HTML file. You can change colors, fonts, button styles, and more.

### Adding Your Own Turing Machine Programs

You can add your own Turing machine programs by modifying the `exemples` object in the JavaScript section of the code. Each new example should follow the structure:

```javascript
var exemples = {
  CustomExample: {
    debut: ["A", 0, "your_initial_tape_content"],
    tete: 0, // Initial head position
    programme: {
      // Define the program's states and transitions
      A0: "B",  // State A reads 0, moves to state B
      A1: "d",  // State A reads 1, writes a 1 and moves right
      Bb: "F",  // State B finishes the execution
    },
  },
};


