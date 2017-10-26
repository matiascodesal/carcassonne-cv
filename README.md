# carcassonne-cv

1. Install Git for Windows with Git Bash
1. Install python 3.6.3amd64 (I installed in C:\python-3.6.3)
1. In a directory where you want to store your code, you should be able to right-click in the dir and choose "Open Git Bash"
1. Clone the repo: git clone https://github.com/matiascodesal/carcassonne-cv.git
1. Enter the repo directory: cd carcassonne-cv
1. Install virtualenv: /c/python-3.6.3/Scripts/pip install virtualenv
1. Make a virtualenv dir: mkdir .venv
1. Create the virtualenv: /c/python-3.6.3/Scripts/virtualenv .venv/carcacv
1. Activate the virtualenv: source .venv/carcacv/Scripts/activate
1. Install packages to env: pip install -r requirements.txt
1. Test env is setup
   1. winpty python
   1. import cv2
   1. cv2.__version__

Initial batch of images were found here: https://github.com/nathanial/caracassonne

## Image Naming Scheme
```<Tile Functional Type>_<Tile Art Variant>_<Photograph Instance>```

- **Tile Function Type**: A letter from A-X which corresponds with the mapping from Appendix A of this thesis: https://project.dke.maastrichtuniversity.nl/games/files/msc/MasterThesisCarcassonne.pdf

- **Tile Art Variant**: Can just be a slight difference in art for the same functional tile due to art direction or differing game edition.

- **Photograph Instance**: Used to enumerate the various images of the same functional type and same art variant.  We want the same tile in a variety of different lighting conditions, distances, angles, blurriness, etc. to train the CV.

