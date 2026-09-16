# JPEG to GeoTIFF Overlay Tool

This is a browser-based prototype for:

- selecting an input JPEG folder
- selecting a reference GeoTIFF folder
- choosing a target output folder
- matching the JPEG to the lower-resolution GeoTIFF by feature detection
- overlaying the JPEG into the correct spatial location
- exporting the result to the output folder

The app is designed to run directly in Google Chrome without requiring a local server.

## Open it directly in Chrome

1. Download or clone the repository.
2. Open the project folder.
3. Double-click `index.html`.
4. Chrome should open the app.

## Important note

This is a prototype georeferencing workflow. It uses browser-side feature matching and the result is best-effort. For accurate quantitative spatial measurements, the final result should be validated with known ground control points and a proper coordinate reference system.

## Suggested next step

If you provide sample JPEG and reference TIFF files, the matching logic can be refined to support the actual image pair used in your project.
