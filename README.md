# Jelly Box

A playground where whatever you type, draw or sculpt turns into squishy, translucent 3D jelly. Grab the jellies, throw them, pile them up and pop them.

**Live:** https://sirusgoorhuis.github.io/jelly-box-playground/

## What you can do

- **Type** text in eight fonts, as one jelly per letter or one per word
- **Draw** on the sketch pad (closed loops keep their holes)
- **Sculpt** a 3D blob with pull, inflate, dent and smooth brushes, starting from a blob, donut or pillow
- **Play:** drag to grab, flick to throw, double-click to pop, toggle gravity, shake everything
- Move the editor anywhere, or close it to an icon (Esc)

## How it works

Everything lives in a single `index.html`. Each jelly is a 2D soft body (shape matching, area preservation and a collision skin) rendered as a real 3D mesh with [three.js](https://threejs.org): refractive transmission, clearcoat and soft shadows, with depth bulge and lean driven by the physics.

Three.js, the icons and the fonts load from public CDNs, so the page needs an internet connection.

## Run locally

```sh
python3 -m http.server 5173
# open http://127.0.0.1:5173/
```
