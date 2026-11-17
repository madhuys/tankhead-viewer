# TankHead viewer

3D viewer for the TankHead turret-headed robot: textured model, Bang-to-Parts splits, printable STL/3MF

A static site: plain HTML, CSS and JavaScript, no build step.

## Run

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Then open http://127.0.0.1:8000/.

## Test

```sh
python3 -m unittest discover -s tests
```

The test checks that every page parses and that every local link and asset it names exists.

A static site has no server code, so it makes no AI calls (a key in a page would be anyone's): an app that needs
chat, speech, pictures or embeddings is a FastAPI or Vite + React app (their READMEs list the calls).
