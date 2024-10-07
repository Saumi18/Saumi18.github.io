This project is a simple augmented reality (AR) web application that uses AR.js and A-Frame to display a 3D object (a yellow cylinder) when a specific barcode marker is detected using the device's webcam.

Features:
1. Barcode Marker Detection: The application uses a 4x4 matrix barcode (similar to QR codes) with a specific value (165) to detect and display the AR object.
2. 3D Object Rendering: When the barcode marker is recognized, a yellow cylinder is rendered above the marker.
3. Webcam Integration: Uses the device’s webcam to capture and process the marker in real-time.
4. Responsive Design: The application is optimized for various screen sizes and ensures the AR experience is smooth by disabling UI debug elements.

To run the application:
1. Clone or Download the repository containing this HTML file.
2. Open the HTML file in a browser with webcam permissions enabled (best viewed using a mobile browser or a desktop browser with a webcam).
3. Point the webcam at a barcode marker with the value 165 to see the 3D yellow cylinder appear.

Technologies Used
1. HTML & JavaScript: Basic HTML structure with JavaScript libraries for AR and 3D rendering.
2. A-Frame: A framework for building 3D and AR/VR experiences directly in HTML.
3. AR.js: A library built on top of A-Frame that provides AR functionality.
4. aframe-extras: An extension library for A-Frame to handle various utilities like loaders and physics.

Libraries Included:
1. A-Frame v0.9.0
2. AR.js for A-Frame
3. aframe-extras Loaders
4. AR.js Configuration

The AR.js script is configured to:
1. sourceType: Webcam - It uses the device's webcam for AR detection.
2. detectionMode: mono_and_matrix - Supports both traditional markers and matrix barcode markers.
3. matrixCodeType: 4x4 - The marker used is a 4x4 barcode type.

Usage Notes:
Ensure that you grant your browser permission to access the webcam.
This project works best with barcode markers generated for the 4x4 matrix code type. The value used here is 165.
If the 3D object does not appear, check the lighting conditions and ensure the barcode is clearly visible to the camera.
Customization
Change Marker Value: Modify the value attribute of the <a-marker> element to use a different barcode marker.
Change 3D Object: Replace <a-cylinder> with any other A-Frame primitive (e.g., <a-box>, <a-sphere>) or a 3D model using the <a-entity> tag.
