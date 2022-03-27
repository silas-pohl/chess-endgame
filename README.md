# Development of an AI for the chess endgame

This repository is being created as part of a student research project entitled **Development of an AI for the chess endgame**. In chess, it is possible to compute an optimal strategy for positions where only a few pieces are left on the board using a so-called retrograde analysis. The main goal is the implementation of this retrograde analysis in Python, in order to obtain a program that can handle the different endgames. For support and visualization the library [python-chess](https://python-chess.readthedocs.io/en/latest/) is used and the program is implemented using [Jupyter notebooks](https://jupyter.org/).

## 🔘 Access and run the notebooks
The intended way to access the notebooks is directly via the online environment [Deepnote](https://deepnote.com/project/Chess-Endgame-9uNN-8heQNu95tDKiwFIwA). Nevertheless, they can also be run locally on the user's own machine. To do this, the repository must be cloned, a corresponding Jupyter environment set up and all the requirements used (see requirements.txt) installed.

## 📙 Notebooks and project structure
The intended execution sequence of the Jupyter notebooks can be seen from the numbering:
- `ChessEndgame.ipynb` This notebook is the introduction to playing chess games using the python-chess library and endgame databases. A player class is created, with the help of which you can replay arbitrary endgames with up to 4 pieces. For this purpose the so-called Gaviota tablebases are used. In addition, this program will later be used to validate the results of the self-performed retrograde analysis.
- `RetrogradeAnalysis.ipynb` ...
- `ChessEndgameWithCustomTablebases.ipynb` ...
