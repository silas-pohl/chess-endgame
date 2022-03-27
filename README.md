# Development of an AI for the chess endgame

This repository is being created as part of a student research project entitled **Development of an AI for the chess endgame**. In chess, it is possible to compute an optimal strategy for positions where only a few pieces are left on the board using a so-called retrograde analysis. The main goal is the implementation of this retrograde analysis in Python, in order to obtain a program that can handle the different endgames. For support and visualization the library [python-chess](https://python-chess.readthedocs.io/en/latest/) is used and the program is implemented using [Jupyter notebooks](https://jupyter.org/).

## Access and run the notebooks (Recommended: Use a virtualenv)

```
git clone https://github.com/silas-pohl/chess-endgame.git
```
```
cd chess-endgame
```
```
pip install notebook
```
```
pip install -r requirements.txt
```
```
jupyter notebook
```

## Notebooks and project structure
The jupyter notebooks are described below in the order of the intended execution sequence:
1. `ChessEndgame.ipynb` This notebook is the introduction to playing chess games using the python-chess library and endgame databases. The ChessEndgame class is created with which you can play/import different endgames with the help of the so-called Gaviota tablebases. Played games are exported and stored in a file in the /games folder.
2. `PlayChessEndgame.ipynb` This notebook is used for actual playing with the ChessEndgame class, which was implemented in the previous notebook. Why the game functionality is outsourced is already explained in the previous notebook.
3. `RetrogradeAnalysis.ipynb` This notebook contains the actual Retrograde Analysis algorithm with the help of which we can create our own tablebases. These tablebases are serialized and stored as binaries in the /tables folder.
4. `ExtendedChessEndgame.ipynb` This notebook is extended the very first notebook and thus the ChessEndgame class. It implements the class CustomTablebases, which imports the previously created tablebases and the ChessEndgame class is adapted to the extent that playing with these custom tablebases is now possible. The actual playing with custom tablebases can take place directly in this notebook.
