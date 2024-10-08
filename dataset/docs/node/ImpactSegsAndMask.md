- `ImpactSegsAndMask`: This node applies a bitwise AND operation between the masks of segmented objects (SEGS) and a given mask (MASK), effectively filtering the segmented objects based on the mask. It's designed to refine segmentation results by combining them with an additional mask layer, enhancing the precision of the segmentation.
    - Parameters:
    - Inputs:
        - `segs`: The segmented objects (SEGS) to be refined. It represents the primary input for the operation, determining the base segmentation to be filtered. Type should be `SEGS`.
        - `mask`: The mask (MASK) to be applied to the segmented objects. It acts as a filter, refining the segmentation by retaining only the parts of the segmented objects that overlap with the mask. Type should be `MASK`.
    - Outputs:
        - `segs`: The refined segmented objects (SEGS) after applying the mask. It represents the output of the bitwise AND operation, containing only the parts of the original segmentation that overlap with the given mask. Type should be `SEGS`.
