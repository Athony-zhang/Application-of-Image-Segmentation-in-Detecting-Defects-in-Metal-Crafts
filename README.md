# Application-of-Image-Segmentation-in-Detecting-Defects-in-Metal-Crafts
The split-and-merge algorithm delivers high-accuracy metal defect detection via robust pre- and post-processing. To enhance performance, parameters must be adjusted to match the specific characteristics of the inspected images.


Region segmentation in image segmentation plays a crucial role in the detection of handicrafts. This paper primarily investigates the application of split-and-merge operations in region segmentation for detecting surface defects on metal handicrafts (aluminum sheets).


This algorithm develops a comprehensive detection workflow. First, image preprocessing is performed: histogram equalization is used to enhance the global contrast of the image, Gaussian filtering is applied to remove image noise, and a combination of large-kernel Gaussian blurring with differential methods is employed to correct for uneven illumination. Next, the split-and-merge algorithm is adopted for image segmentation, using the within-region gray-level variance (VWHR) as a consistency metric. The algorithm parameters are optimized as follows: the split variance threshold is set at 250, the merge variance threshold at 85, and additional feature-selection criteria include a gray-level difference threshold (40) and a minimum defect area threshold (500). To address the issue of repeated defect identification, a bounding-box merging strategy based on geometric center distance (threshold: 60) is designed.


The experimental results show that the optimized algorithm can effectively highlight and distinguish black spot defects on the surface of aluminum sheets, significantly reducing both the false-positive rate (such as misidentification of metal edges) and the miss-rate. This algorithm exhibits excellent robustness and “template” characteristics; by adjusting the corresponding parameters, it can be adapted to meet detection requirements for various material crafts and defect types, making it highly valuable for industrial applications. 

Keywords: image segmentation; defect detection; histogram equalization; split-and-merge algorithm; Gaussian filtering; industrial inspection
