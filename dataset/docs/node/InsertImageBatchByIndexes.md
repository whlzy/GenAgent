- `InsertImageBatchByIndexes`: The InsertImageBatchByIndexes node is designed for integrating specific images into a given batch of images at designated indexes, maintaining the original sequence order of the batch. This functionality is particularly useful for tasks that require precise manipulation of image sequences, such as inserting processed images back into their original context.
    - Parameters:
    - Inputs:
        - `images`: The original batch of images where new images are to be inserted. It serves as the base for the insertion operation. Type should be `IMAGE`.
        - `images_to_insert`: The images to be inserted into the original batch at specified indexes. This parameter is crucial for defining which images are added and where. Type should be `IMAGE`.
        - `insert_indexes`: The indexes within the original batch where the new images should be inserted. This parameter dictates the positions for insertion, aligning new images with the original sequence. Type should be `INDEXES`.
    - Outputs:
        - `images_after_insert`: The updated batch of images after insertion, preserving the original sequence order with the new images integrated at specified positions. Type should be `IMAGE`.
