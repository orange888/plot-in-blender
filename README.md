## plot-in-blender
### What it is ?
This is a python library to analyse data, so far the following plots can be visualized in Blender. 
- BarPlot
- ScatterPlot (2D and 3D)
- HistPlot


<p align="center"><img src="https://raw.githubusercontent.com/hazilMohamed/data-visualization-using-blender/master/res/screenshots/3D-scatterPlot.png"></p>

### Requirements
- Blender 2.82 or higher.
- Python 3.8x.

### Setup
- Clone the repo to your directory.
- Change the BLENDER_PATH to your blender executable.

### Importing
Import the library to your project
```shell
import plotinblender as bl
```

### Usage
The plotinblender accepts both lists and numpy arrays as arguments
```python
import numpy as np
X = np.array(np.random.rand(500)*500)
y = np.array(np.random.rand(500)*500)
z = np.array(np.random.rand(500)*500)
```
To plot, use the following functions:
- BarPlot
```python
bl.barPlot(X,y)
```
- ScatterPlot
```python
#Two arguments gives 2D plots while Three gives 3D plots
bl.scatterPlot(X, y)
bl.scatterPlot(X, y, z)
```
- HistPlot
```python
#Bins is optional value
bl.histPlot(X, bins)
```

### Contribute
If you have a new idea for plotting or find out a bug or something, please feel free to raise an issue or pull request.

### TODO
- Need to implement plots for negative values too.
- Planning to implement an FBX viewer for viewing plots.
- Materials for objects in Blender.
- Categorical plots.

