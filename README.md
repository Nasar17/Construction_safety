# OVERVIEW
- Ensuring the safety of workers on construction sites is critical, especially in high-risk environments where proper use of Personal Protective Equipment (PPE) is mandatory. 
- This project introduces a computer vision-based safety monitoring system that automatically detects PPE violations from video streams. 
- Two computer vision models were explored for this task: YOLOv12 (You Only Look Once version 12 ) and RDETR (Refined DEtection TRansformer). 
- Both models were trained on a curated construction PPE dataset and evaluated based on detection accuracy, inference speed, and mean Average Precision (mAP). 
- YOLOv12 demonstrated superior performance and was selected for deployment. 
- The finalized model was embedded into a modular Python pipeline that supports both live and recorded video input, enabling real-time detection of safety violations. 
- Annotated output videos and detailed PDF reports are generated to provide actionable insights. 
- This system offers a scalable and automated solution to enhance PPE compliance and improve safety oversight on construction sites.
# DATASET
- The dataset comprises 3,000 annotated images, collected from various real-world construction scenarios.
- Each image includes bounding box annotations for objects of interest, labeled according to ten predefined classes that cover both protective gear and safety violations.
- These classes are:
  - PPE Items: helmet, goggles, gloves, boots, vest
  - Violation Tags: no_helmet, no_goggles, no_glove, no_shoes
  - Others: person
# RESULTS
 - # YOLO V12 
    ![Screenshot 2](Screenshot%202025-08-13%20163500.png)

 - # RFDETR
    ![Screenshot 1](Screenshot%202025-08-13%20162943.png)
   
# CONCLUSION
 Considering the total detection performance, training scalability, and inference speed, YOLOv12was selected as the final model for integration into the video-based safety monitoring pipeline. 
 RFDETR, while competitive in some areas, was found to be less optimal under the practical constraints of deployment on dynamic construction sites.
