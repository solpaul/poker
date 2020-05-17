# poker tracker

This project aims to develop a jupyter notebook/voila based app to track an online poker table and return nash push/fold ranges at the start of each hand.

Required installations:
- Anaconda (Python 3.7 version)
- Tesseract

Additional Python libraries:
- pyautogui
- win32gui
- webbrowser
- pytesseract
- voila

poker_voila.ipynb is the app notebook - can be run directly in the notebook, or using voila by running the following from a terminal:

<pre><code>voila --enable_nbextensions=True</code></pre>

initial_notebook.ipynb has rough development code.

vision_trainer.ipynb trains a neural net to recognise number of players sat at a table (ultimately not used, pytesseract was used instead to read numbers from the table images).

Current development items:
- Fix heads-up button position (requires additional image read)
- Speed up stack/button grab (stitch crops together for one OCR read by pytesseract)
- Ranges currently obtained by navigating to 3rd party website - replace with local calculation
