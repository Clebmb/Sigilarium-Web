# Sigilarium 2.0

**Sigilarium** is a web-based application designed for generating, manipulating, and animating geometric sigils. It translates various forms of user input into visual patterns using configurable grid systems and rendering options.

### Practical Application in Chaos Magick
This tool streamlines the sigilization process—a core technique in Chaos Magick for focusing will and manifesting intent. It provides a digital framework for:
*   **Abstraction**: Automatically converting conscious statements of intent into non-linear, abstract glyphs to bypass the "psychic censor."
*   **Gnosis & Charging**: Utilizing hypnotic animations (stroboscopic lines, rotation, color cycling) to assist practitioners in achieving a state of gnosis (altered consciousness) essential for charging the sigil.
*   **Ritual Geometry**: Leveraging numerological and geometric grids (such as the Saturn square or radial wheels) to structure the intent within specific metaphysical correspondences.

## Features

### Input Modes
*   **Text Processing**: Converts text input into geometric paths by mapping characters to grid coordinates (removing vowels and duplicates).
*   **Numeric Input**: Maps sequences of numbers directly to grid points.
*   **Freehand Drawing**: Allows users to draw custom paths directly on the HTML5 Canvas.
*   **Image Analysis**: Uploads an image and samples its brightness/luminosity values to generate a corresponding coordinate sequence.

### Geometric & Rendering Control
*   **Grid Systems**:
    *   **Saturn (3x3)**: Standard numeric 3x3 grid mapping.
    *   **Witch Wheel**: Circular radial arrangement.
    *   **Chaos Scatter**: Randomized distribution of points.
*   **Segments**: Adjustable kaleidoscope effect (1-16 segments) for radial symmetry.
*   **Symmetry**: Toggleable X and Y axis mirroring.
*   **Styling**: Real-time control over stroke color, background color, glow effects, and cubic bezier curve smoothing.

### Animation System
The application supports real-time canvas animations:
*   **Segment Draw / Live Trace**: Progressively draws the path segments.
*   **Line Flow**: Dashed line offset animation.
*   **Rotation**: Continuous CW or CCW rotation.
*   **Pulse**: Scale modulation (breathing effect).
*   **Chroma**: HSL color cycling.

### Sigil Scribe Tool
A utility for processing statements of intent:
1.  **Unique Character Extraction**: Filters distinct letters.
2.  **Consonant Reduction**: Removes vowels.
3.  **Gematric Conversion**: Maps letters to numeric values.
4.  **Sigil Nucleus**: Reduces the sum of values to a single digit (recursive sum).

### Export Options
*   **PNG**: Exports the current canvas state as a static image (supports transparency).
*   **GIF**: Client-side GIF generation using `gif.js` to capture active animations.

## Tech Stack
*   **Frontend**: HTML5, CSS3, Vanilla JavaScript.
*   **Rendering**: HTML5 Canvas API (2D Context).
*   **Libraries**: `gif.js` (for GIF export).

## Local Development & Setup

This is a static web application. It does not require a build step or a Node.js backend to run basic features.

### Prerequisite
*   A modern web browser (Chrome, Firefox, Edge).

### Running the Application
1.  **Clone the repository**:
    ```bash
    git clone https://github.com/Clebmb/Sigilarium-Web.git
    ```
2.  **Serve the files**:
    *   **Basic**: You can simply open `index.html` in your browser.
    *   **Advanced (Required for GIF Export)**: Due to browser security policies (CORS/Web Workers), the GIF export feature may encounter issues if run directly from the file system (`file://`). It is recommended to use a local development server.
        *   **Python**: `python -m http.server 8000`
        *   **Node/NPM**: `npx serve .` or use the Live Server extension in VS Code.

---

### *NOTHING IS TRUE. EVERYTHING IS PERMITTED.*
