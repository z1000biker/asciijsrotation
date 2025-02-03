ASCII Rotating Sphere with Caustic Background
This project is a JavaScript simulation of a rotating ASCII sphere with a dynamic, caustic-style background. The sphere is made up of ASCII characters (in this case, the text is ascii numbers), and the background features smooth, morphing colors that create an underwater caustic effect.

Features
Rotating ASCII Sphere:

The sphere is represented by points in 3D space, projected onto a 2D canvas.

The ASCII characters fade from white (closest) to gray (farthest), creating a depth effect.

The sphere rotates smoothly along all three axes.

Caustic-Style Background:

The background features organic, morphing colors generated using a simple noise function.

The colors shift smoothly over time, creating a dynamic, underwater caustic effect.

Customizable:

The text, font size, rotation speed, and background colors can be easily modified.

How It Works
Sphere Generation:

The sphere is generated using spherical coordinates, with points distributed randomly across its surface.

Each point is projected onto the 2D canvas using a simple perspective projection.

Rotation:

The sphere rotates using 3D rotation matrices for the X, Y, and Z axes.

Caustic Background:

The background is generated using a noise function (simpleNoise) that creates smooth, organic patterns.

The colors are calculated based on the noise value and updated over time to create a morphing effect.

Rendering:

The background is drawn in a grid (20x20 pixels) for performance.

The ASCII characters are drawn on top of the background, with their brightness determined by their depth.

Code Structure
HTML:

The <canvas> element is used to render the simulation.

The noisejs library is not required; a simple noise function is implemented directly in the code.

JavaScript:

The render function handles the animation loop using requestAnimationFrame.

The getCausticColor function generates colors for the background based on noise values.

The rotateX, rotateY, and rotateZ functions handle 3D rotation.

How to Run
Clone the repository:


git clone https://github.com/your-username/ascii-rotating-sphere.git
Open the index.html file in your browser.

Customization
Change the Text:

Modify the chars variable in the JavaScript code to use different ASCII characters or text.

Adjust Font Size:

Change the fontSize variable to make the ASCII characters larger or smaller.

Modify Rotation Speed:

Adjust the rotationSpeed variable to make the sphere rotate faster or slower.

Customize Background:

Modify the getCausticColor function to change the color scheme or noise pattern.

Dependencies
None! The project uses vanilla JavaScript and HTML5 Canvas.

