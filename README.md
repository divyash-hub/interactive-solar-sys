# HELIOS — The Solar System in Real Time

An interactive 3D model of the Solar System that runs in the browser. Every planet sits where it really is today and moves along its true elliptical orbit.

**Designed & developed by Divyash Agrawal**

## Features

- **Real positions:** planet positions are computed from NASA/JPL orbital elements by solving Kepler's equation every frame, so the layout matches the real sky for any date.
- **Time machine:** play live, speed up to a year per second, reverse, or jump back to "Now".
- **High-resolution planet maps** (up to 4K), based on NASA imagery.
- **Earth:**
  - a day/night shader with NASA city lights on the night side
  - shiny oceans
  - a cloud layer
  - a glowing atmosphere
- **Real-time shadows:**
  - moons cast eclipse shadows on their planets
  - Saturn's rings and Saturn shadow each other
- **Halley's Comet:** its tail grows as it nears the Sun and points away from it. Its next return is in 2061.
- **13 moons**, the asteroid belt (with its real gaps) and the Kuiper Belt.
- **Live telemetry** for each planet:
  - distance from the Sun
  - distance from Earth
  - orbital speed
  - how long sunlight takes to reach it
- **Guided tour**, keyboard shortcuts and a layout that works on phones.
- **Cinematic look:** HDR bloom, filmic tone mapping and lens flare.

## Run it locally

Browsers block 3D textures on pages opened straight from your computer (`file://`), so serve the folder instead:

- **VS Code:** install the "Live Server" extension, right-click `index.html` and choose **Open with Live Server**.
- **Python:** run `python -m http.server` in this folder, then open http://localhost:8000.

## Publish it on GitHub Pages

1. Create a new repository and upload everything in this folder (`index.html`, `README.md` and the `textures` folder).
2. Go to **Settings → Pages**, set **Source** to "Deploy from a branch", choose `main` and `/ (root)`, then save.
3. After a minute or two, your site is live at `https://<your-username>.github.io/<repo-name>/`.

## Built with

[Three.js](https://threejs.org) (WebGL), written in plain HTML, CSS and JavaScript. No build step is needed.

## Credits

- **Planet and Sun maps:** [Solar System Scope](https://www.solarsystemscope.com/textures/), licensed CC BY 4.0 and based on NASA imagery.
- **Earth city lights:** NASA Black Marble.
- **Earth normal and ocean maps:** three.js example assets.
- **Moon, Pluto and outer-moon maps:** community maps based on NASA/JPL mission imagery (Galileo, Cassini, Voyager, New Horizons).
- **Orbital elements:** NASA/JPL Solar System Dynamics.
