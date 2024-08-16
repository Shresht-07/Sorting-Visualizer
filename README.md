# Sorting Visualizer

This project is a web-based sorting visualizer that helps users understand how different sorting algorithms work by providing an interactive and animated representation. The user can generate a new array of bars, adjust the size and speed of the array, and select from various sorting algorithms to see how they operate.

## Features

- *Responsive Design:* Built with Bootstrap for a modern and responsive UI.
- *Interactive Controls:* Users can generate a new array, adjust the size and speed, and choose different sorting algorithms.
- *Multiple Sorting Algorithms:* Visualize the following algorithms:
  - Bubble Sort
  - Selection Sort
  - Insertion Sort
  - Quick Sort
  - Merge Sort

## Installation

To run this project locally, follow these steps:

1. *Clone the repository:*
    bash
    git clone https://github.com/Shresht-07/Sorting-Visualizer.git
    
2. *Navigate to the project directory:*
    bash
    cd sorting-visualizer
    
3. *Open the project in a browser:*
    - You can directly open the index.html file in your web browser.

## Usage

- *New Array:* Click the "New Array" button to generate a new array of bars.
- *Adjust Size:* Use the "Size" slider to adjust the number of bars in the array.
- *Adjust Speed:* Use the "Speed" slider to control the speed of the sorting animation.
- *Select Sorting Algorithm:* Click on one of the sorting buttons (Bubble Sort, Selection Sort, etc.) to visualize the sorting process.

## File Structure

- index.html - The main HTML file that contains the structure of the web page.
- style.css - Custom CSS for styling the sorting visualizer.
- js_files/ - A directory containing JavaScript files for different sorting algorithms and the main sorting logic.
  - sorting.js - Main script handling the visualizer's functionality.
  - bubble.js - Contains the logic for Bubble Sort.
  - insertion.js - Contains the logic for Insertion Sort.
  - merge.js - Contains the logic for Merge Sort.
  - quick.js - Contains the logic for Quick Sort.
  - selection.js - Contains the logic for Selection Sort.

## Dependencies

- [Bootstrap](https://getbootstrap.com/) - Used for responsive design and styling.

## Contributing

If you'd like to contribute to this project, feel free to fork the repository and submit a pull request. Issues and feature requests are welcome!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

- The project utilizes Bootstrap for styling and responsiveness.
- Inspired by various sorting visualizer tools available online.
