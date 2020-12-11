# strainmatLabeler
## 1 Introduction and Functions
This software enable user to check the strain matrix from .mat file exported by [DENSEAnalysis](https://github.com/denseanalysis/denseanalysis) software and add new TOS curves.
![record](./imgs/record_small.gif)

The functions include:
### 1.1 Visualize Strain Matrix
![vis](./imgs/loaded.png)
![vis](./imgs/view_3D.png)
### 1.2 Generate and Visualize "Full-Resolution" Strain Matrix
![vis](./imgs/loaded_full_res.png)
### 1.3 Add TOS Labels
![vis](./imgs/add_points.png)
### 1.4 Export to .mat File or Image
![vis](./imgs/export_mat.png)

## 2 Usage
### 2.1 Start Program
```python
# Dependencies: numpy, scipy, matplotlib, pyQt
python ./strainMatLabelorQt.py
```
### 2.2 Load .mat File Containing Strain Matrix
Drag `.mat` file exported by DENSEAnalysis to the left canvas.
![vis](./imgs/drag_to_load.png)
### 2.3 Load .mat File Containing TOS Curve
Drag `.mat` file containing TOS to the left canvas.
![vis](./imgs/tos_loaded.png)
### 2.4 Check Strain Matrix
Please feel free to try the options on the right panel
### 2.5 Annotate New TOS Curve
- Add a control point: mouse middle click at target location
- Remove a control point: mouse right click at target point
- Move a control point: mouse left click at target point
### 2.6 Export
![vis](./imgs/export_mat.png)
If `TOS only` is checked, the added TOS data will be store at the root path of the saved file; otherwise, the TOS data would be stored inside `TOSAnalysisInfo`, and the annotator name will be appended. 
