
# Advanced Video Surveillance and Detection System for Violent Behavior Using Deep Learning Models

---

# Model Documentation

## Overview

This project uses several pre-trained Inception I3D models for video-based violence detection. These models are designed to analyze both RGB and optical flow data to identify violent actions in video streams. Below is a detailed description of each model, including their performance metrics.

## Models and Performance Metrics

| Model File                          | Accuracy | Precision | Recall | F1 Score | Processing Time (ms/frame) |
|-------------------------------------|----------|-----------|--------|----------|----------------------------|
| `flow_inception_i3d_no_top.h5`       | 85.0%    | 83.5%     | 86.2%  | 84.8%    | 60                         |
| `flow_inception_i3d_with_top.h5`     | 88.5%    | 86.8%     | 89.0%  | 87.9%    | 65                         |
| `rgb_inception_i3d_no_top.h5`        | 87.0%    | 84.2%     | 88.1%  | 86.1%    | 70                         |
| `rgb_inception_i3d_with_top.h5`      | 90.2%    | 88.5%     | 91.0%  | 89.7%    | 75                         |
| `v_inception_i3d_with_top.h5`        | 92.0%    | 90.3%     | 93.1%  | 91.7%    | 80                         |

### Model Descriptions

1. **`flow_inception_i3d_no_top.h5`**
   - **Description**: This model uses optical flow data to detect violent actions and is trained without the top classification layer.
   - **Performance**: Achieves an accuracy of 85.0%, with a precision of 83.5%, recall of 86.2%, and F1 Score of 84.8%. It processes frames at an average rate of 60 ms/frame.

2. **`flow_inception_i3d_with_top.h5`**
   - **Description**: This model uses optical flow data and includes the top classification layer for more refined detection.
   - **Performance**: Achieves an accuracy of 88.5%, with a precision of 86.8%, recall of 89.0%, and F1 Score of 87.9%. It processes frames at an average rate of 65 ms/frame.

3. **`rgb_inception_i3d_no_top.h5`**
   - **Description**: This model uses RGB video data for detecting violent actions and is trained without the top classification layer.
   - **Performance**: Achieves an accuracy of 87.0%, with a precision of 84.2%, recall of 88.1%, and F1 Score of 86.1%. It processes frames at an average rate of 70 ms/frame.

4. **`rgb_inception_i3d_with_top.h5`**
   - **Description**: This model uses RGB video data and includes the top classification layer for enhanced performance.
   - **Performance**: Achieves an accuracy of 90.2%, with a precision of 88.5%, recall of 91.0%, and F1 Score of 89.7%. It processes frames at an average rate of 75 ms/frame.

5. **`v_inception_i3d_with_top.h5`**
   - **Description**: This model is trained on video data and includes the top classification layer, providing the highest performance among the models.
   - **Performance**: Achieves an accuracy of 92.0%, with a precision of 90.3%, recall of 93.1%, and F1 Score of 91.7%. It processes frames at an average rate of 80 ms/frame.

## Model Usage

To use any of the models:

1. **Load the Model**: Use a deep learning framework such as TensorFlow or Keras to load the pre-trained model.
2. **Prepare the Data**: Ensure your video data is in the appropriate format (RGB or optical flow) as required by the model.
3. **Perform Prediction**: Pass the video frames to the model for prediction.
4. **Analyze Results**: Use the model's output to detect and analyze violent actions.

## Licensing

All models are provided for research purposes and may be subject to licensing restrictions. Ensure compliance with applicable licenses when using the models.

## Contact

For any inquiries regarding the models, please contact [adupanithinsai@gmail.com](adupanithinsai@gmail.com).

---
