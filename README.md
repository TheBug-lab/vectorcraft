# SVG Art Generator

**SVG Art Generator** is an innovative project that creates unique, randomized SVG art based on various layouts and user-defined parameters. It offers a rich interface for customizing every aspect of the artwork, including colors, shapes, layout, density, and complexity. This project is built using a modular architecture consisting of a **Tkinter GUI**, a **Django backend providing a web API**, and demos showcasing its usage in **React** for web-based applications as well as generating motion graphics and customized presentations.

## Features
- Generate **random and unique SVG art** based on a wide variety of layouts.
- **Tkinter GUI** for generating art locally with real-time previews.
- **Django-based web API** to integrate the art generation into websites and other applications.
- **Fully customizable parameters** like color, shape, layout, density, complexity, and more.
- **React demo** to showcase how to use the API in web development.
- **Demo for motion graphics** and generating art for **custom presentations**.

## Layouts
The project supports multiple predefined layouts to create unique art pieces, with plans to expand layouts in the future:
- **FractalLayout**: Generates recursive fractal patterns.
- **MandalaLayout**: Creates circular, intricate designs with a spiritual or artistic touch.
- **GeometricLayout**: Uses geometric shapes to form structured yet abstract designs.
- **FlockingLayout**: Simulates flocking behavior to create dynamic, organic shapes.
- **NestedPatternsLayout**: Builds art through nested pattern structures.
- **SpiralChaosLayout**: Generates chaotic spiral patterns.
- **VoronoiLayout**: Creates Voronoi diagrams for natural, organic shapes.
- **NeonLayout**: Produces glowing, vibrant designs with a neon-like effect.
- **AbstractLayout**: Generates freeform, abstract art.
- **GlitchLayout**: Introduces distortion and randomness for a glitchy, modern look.
- **OpticalArtLayout**: Generates optical illusions using abstract shapes.
- **TesselationLayout**: Creates repeating tile patterns.
- **ScratchLayout**: Mimics scratch-like designs and imperfections.
- **PointillismLayout**: Creates art using small dots for a pointillist style.
- **CoiledLayout**: Builds coiled and swirling designs.
- **LSystemLayout**: Utilizes L-Systems for fractal and recursive patterns.
- **GeometricFlowLayout**: Creates flowing geometric patterns.

More layouts may be added in the future to enhance the diversity of generated art.

## Technologies Used
- **Frontend**: 
  - Tkinter (for the local GUI)
  - React (for the web demos)
- **Backend**:
  - Django (providing web API)
- **Art Generation**:
  - SVG manipulation with Python (via `cairosvg`, `svgwrite`, etc.)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/svg-art-generator.git
   cd svg-art-generator
   ```

2. Install dependencies:
   - For the **Django backend**:
     ```bash
     cd backend
     pip install -r requirements.txt
     python manage.py migrate
     ```

   - For the **Tkinter GUI**:
     ```bash
     cd gui
     pip install -r requirements.txt
     ```

   - For the **React demo**:
     ```bash
     cd react-demo
     npm install
     ```

## Usage

### Tkinter GUI
Run the Tkinter-based GUI locally to generate and preview SVG art in real-time.

1. Navigate to the `gui/` folder.
2. Run the following command:
   ```bash
   python main.py
   ```

This will open a graphical interface where you can select layouts, customize parameters (colors, shapes, etc.), and generate SVG art. The generated SVG can be saved directly from the interface.

### Web API (Django)
You can also generate art using the Django-based web API. The API allows you to send requests specifying layout type, colors, and other customization parameters, and receive a downloadable SVG file.

1. Navigate to the `backend/` folder.
2. Start the Django server:
   ```bash
   python manage.py runserver
   ```

3. You can now send POST requests to the API at `/api/generate-art/` to generate art via a web interface or external apps.

### React Demo
The project includes a **React-based web demo** to showcase how the backend can be used in web applications.

1. Navigate to the `react-demo/` folder.
2. Start the React app:
   ```bash
   npm start
   ```

The demo will show how users can interact with the API to generate SVG art on the web, including live previews and customization options.

### Art Customization
The SVG Art Generator allows for full customization of your artwork:
- **Colors**: Choose any color scheme (hex or RGB).
- **Shapes**: Pick from predefined shapes or define custom ones.
- **Layout**: Select from the numerous layouts described above.
- **Density and Complexity**: Control the complexity and amount of detail in each piece.
- **Randomization**: Enable or disable randomization for specific parameters.

## Contributing
We welcome contributions! Feel free to open issues and submit pull requests to improve the project.

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.
