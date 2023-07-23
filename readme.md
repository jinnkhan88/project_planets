# 🪐 Habitable Planets Counter - Node.js Script 🌌🚀

## Overview

This Node.js script is designed to read Kepler data from a CSV file, parse the data, and then display the count of habitable planets based on specific criteria: "koi_disposition" (disposition status), "koi_insol" (insolation flux), and "koi_prad" (planet radius).

## Installation

1. Ensure you have [Node.js](https://nodejs.org/) installed on your system.
2. Clone this repository to your local machine using the following command:

git clone https://github.com/jinnkhan88/habitable-planets-counter.git

3. Navigate to the project directory:

cd habitable-planets-counter

4. Install the required dependencies using npm:

npm install

## Usage

1. Planets data is in `planets_data.csv` in the project directory.

2. Run the Node.js script with the following command:

node index.js

3. The script will read the CSV file, parse the data, and display the count of habitable planets based on the specified criteria.

## Criteria for Habitable Planets

The script counts the habitable planets based on the following criteria:

1. **koi_disposition**: The disposition status of the Kepler Object of Interest (KOI). Only planets with "CONFIRMED" disposition are considered habitable.

2. **koi_insol**: The insolation flux of the KOI. Only planets with insolation flux between a specified range (e.g., 0.36 to 1.11) are considered habitable.

3. **koi_prad**: The planet radius of the KOI. Only planets with a planet radius less than a specified value (e.g., 1.6 Earth radii) are considered habitable.

## Sample Output

=============================

Habitable Planets Count Report

Total Habitable Planets: 8

## Customize Criteria

You can customize the criteria for habitable planets by modifying the `isHabitablePlanet(planet)` function in the `index.js` file. Adjust the values of "koi_insol_min", "koi_insol_max", and "koi_prad_max" to suit your specific requirements.

## Contributions

Contributions to this project are welcome! If you find any issues or have suggestions for improvements, please feel free to create an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---

Thank you for checking out the Habitable Planets Counter Node.js script. Explore the wonders of the cosmos with data analysis and make exciting discoveries! 🌌🚀
