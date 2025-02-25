# Three-Shot SAM2 Segmentation Enables Expert-Level Quantification of Lumbar Paraspinal Muscles on Multi-Sequence MRI

Welcome to the **3Shot-LPM-Seg** repository! Three-Shot SAM2 enables expert-level quantification of lumbar parapsinal muscle area and fatty infiltration ratio.

## Method Overview

**3Shot-LPM-Seg** automatically segments the lumbar erector spinae (LES) and multifidus (MF) muscles across T1-weighted, T2-weighted, Dixon water images on the L4/L5 disc level. This method was retrospectively validated across four datasets on a total of 943 MRI slices from 486 participants. 

---


## Implementation Workflow

1. **Model Inference**:  
   Use the SAM2 model for LPM segmentation in a training-free manner
   
   Refer to: [Implementation_steps.md](documentation/Implementation_steps.md)  

3. **Post-Processing**:     
   Refer to: [LPM_seg_curated_into_top1_mask.ipynb](LPM_seg_curated_into_top1_mask.ipynb)  

4. **Segmentation Accuracy Evaluation**:  
   Assess segmentation performance using Dice Similarity Coefficient (DSC) metrics.  
   Refer to: [LPM_seg_accuracy_evluate_in_DSC.ipynb](LPM_seg_accuracy_evluate_in_DSC.ipynb)  

5. **Statistical Evaluation**:  
   Calculate muscle volume using both automated and manual segmentations.  
   Refer to: [LPM_seg_to_vol_2csv.ipynb](LPM_seg_to_vol_2csv.ipynb)  


---


## License

This project is licensed under the **Apache License, Version 2.0**.  
Refer to the [LICENSE](LICENSE) file for details.

---

## Publication

Details of the associated publication will be updated soon.
