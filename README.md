# FISH_spot_selection
This tool is meant for the manual intensity extraction of FISH spots.

Using napari as GUI, the user can select from the maximum projection (ch, y, x) of arrays with shape (z, ch, y, x) the points to extract a fixed XYZ volume (pixels) intensities. 
As output the user can generate:
- Plots of the ROIs selected per cell in maximal projection in Z.
- Plots of the ROIs selected per cell in maximal projection in X.
- An Excel with different sheets providing:
    - raw: the different information collected from the name position, coordinates and intensities comprised in the ROIs selected (max, min, sum, std).
    - counts: number of points selected per layer
    - intron: points selected from the intron layer
    - exon avg: average of the exon selected from the exon layers per cell.
    - relative expression: normalization of the intensity from the intron ROI over the exon avg ROIs
    - frequency: number of times that the intron layer appears over the total of cells screened.
