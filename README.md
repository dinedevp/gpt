# Audio to AI Video Web App

This sample application demonstrates a simple interface for uploading audio
files and generating a video via an external AI video generation service.
The actual API integration is left as a placeholder.

## Setup

1. Create a virtual environment and install dependencies:

```bash
cd server
pip install -r requirements.txt
```

2. Run the development server:

```bash
python app.py
```

The app will be available at `http://localhost:5000`.

## How It Works

- Users upload an audio file (e.g., MP3 or WAV) through the web interface.
- The server saves the audio file and would normally send it to a third-party
  AI video generation API along with selected options.
- For demonstration purposes, the app copies a placeholder video instead of
  calling an external service.
- The resulting video is shown on the page with a download link.

## Notes

To integrate a real video generation service, modify the `generate_video`
function in `server/app.py` to call your chosen API and save the returned
video file into `static/videos`.


## NextHorizon Call Center Site

Un site complet pour le centre d'appel NextHorizon est disponible dans le
repertoire `nexthorizon/`. Ouvrez `nexthorizon/index.html` pour decouvrir les
differentes sections (services détaillés, valeurs, FAQ et formulaire de
contact).

### Hébergement sur Netlify

Le site statique dans `nexthorizon/` peut être déployé directement sur Netlify.
Lors de la configuration du site, indiquez simplement `nexthorizon` comme
répertoire de publication ("publish directory"). Le fichier `netlify.toml`
contient déjà ce paramétrage par défaut.
