# WAET.github.io
This is a template page for hosting WAET tests.

## Usage
- Standard MUSHRA: https://jacquelm.github.io/WAET.github.io/test.html?url=tests/mushra_test.xml
- Simple MUSHRA: https://jacquelm.github.io/WAET.github.io/test.html?url=tests/mushra_simple.xml
- Vocoder MUSHRA: https://jacquelm.github.io/WAET.github.io/test.html?url=tests/mushra_vocoder.xml

## Run locally
1) Start a local server from the repo root:
   `python3 -m http.server 8000`
2) Open a test in your browser:
   `http://localhost:8000/test.html?url=tests/mushra_vocoder.xml`

## Run on GitHub Pages
1) Set the Formspree endpoint in `test.html`:
   `window.WAET_FORM_ENDPOINT = "https://formspree.io/f/xqarlaqp";`
2) Push to GitHub and enable Pages for the repository.
3) Open the hosted URL, for example:
   `https://<user>.github.io/<repo>/test.html?url=tests/mushra_vocoder.xml`

Notes:
- On GitHub Pages there is no PHP backend, so results are submitted via Formspree.
- If the submission fails, the UI shows a download link so participants can save the XML results.