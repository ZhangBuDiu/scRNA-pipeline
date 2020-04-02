## Motivation
* This step is produced to eliminate cell-specific biases.
* Differences between `Normalization` and `Batch correction`: `Normalization` only considers technical biases, while `Batch corrrection` occurs from batches and must consider both technical biases and biological differences.
* Technical biases tend to affect genes in a similar manner, or at least in a manner related to their biophysical properties (e.g., length, GC content), while biological differences between batches can be highly unpredictable.


## normalization types:
1. library size
library size factor of each cells is propotional to its total RNA counts
2. deconvolution: 
assumpt that most genes are not defferential expression between cells and changes in total RNA content are not interesting.
3. spike-ins: 
normalized by spike-ins. (spike-ins is a transcription used to calibrate measurements. refer to [wike](https://en.wikipedia.org/wiki/RNA_spike-in))
total RNA are associated with a biological process of interest, e.g., cell cycle activity or T cell activation. 
