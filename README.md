# JPEG to GeoTIFF Overlay Prototype

Open `index.html` in Google Chrome. The app uses CDN-hosted GeoTIFF.js and OpenCV.js, so an internet connection is needed when it starts.

Workflow:

1. Choose an input folder and select a JPEG.
2. Choose a reference folder and select a GeoTIFF.
3. Inspect the detected dimensions, CRS, origin, and pixel size.
4. Choose an output folder.
5. Run ORB feature matching with RANSAC homography estimation.
6. Review the overlay preview and the reported inlier count.
7. Save an RGB GeoTIFF using the reference image's geospatial metadata.

This is intentionally a **prototype**. It rejects weak matches, but it cannot guarantee survey-grade accuracy. Perspective distortion, terrain relief, lens distortion, different seasons, or repetitive imagery can produce a plausible-looking but inaccurate result. Validate exported files with known control points before using them for quantitative measurements.

Chrome's File System Access API is required to write directly to the selected output folder. If the browser cannot provide that API, the app will not pretend that a PNG or non-georeferenced file is a GeoTIFF.
