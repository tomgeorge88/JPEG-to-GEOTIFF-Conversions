# JPEG to GeoTIFF Overlay Prototype

This version avoids direct `.length` calls on optional raster and OpenCV results. It normalizes GeoTIFF raster output, counts OpenCV matches with its API, and counts RANSAC inliers with `mask.rows` and `mask.ucharAt()`.

Open `index.html` in Chrome. The app loads GeoTIFF.js and OpenCV.js from CDNs, so an internet connection is required. Chrome's File System Access API is required for writing into the selected output folder.

The result is a prototype and must be checked with known control points before quantitative use.
