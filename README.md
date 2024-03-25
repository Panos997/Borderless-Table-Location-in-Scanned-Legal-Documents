This section of my capstone project focuses on identifying and extracting borderless tables from financial statements.

The project worked with a dataset containing a total of 119 financial statements, which were not publicly available. Within these financial statements, there were 183 borderless tables. However, none of these tables were pre-annotated, which added complexity to the task. Consequently, we manually annotated all 183 borderless tables for research purposes.

To address this objective efficiently, we developed a methodology with two approaches.

In the first approach, we utilized pre-trained models. Specifically, we selected two models: YOLOv8 and detr-doc-table-detection. YOLOv8 included three variations fine-tuned on similar datasets: yolov8n-table-extraction, yolov8s-table-extraction, and yolov8m-table-extraction. The detr-doc-table-detection model is based on detr-resnet-50.

In the second approach, we fine-tuned a Yolov8n model for table extraction. We attempted to use the Img2Table library to extract table structures from the predictions of the YOLOv8n model. This involved applying Img2Table to cropped tables from located images and saving the extracted tables in Excel files.

This project provides a practical framework for utilizing object detection models to locate and extract borderless tables from financial documents with diverse and challenging structures. It starts with manual annotation of data and progresses to successful model training.
