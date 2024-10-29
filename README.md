Intelligent Surveillance System with Crime Detection and Emotion Recognition
============================================================================

Overview
--------

In the rapidly advancing field of video analytics, modern surveillance systems demand a blend of intelligence and adaptability to address complex security needs. This project presents an **Intelligent Surveillance System** that combines **Crime Detection** and **Emotion Recognition** capabilities. By integrating advanced computer vision and deep learning techniques, this system detects theft, abuse, and vandalism, while analyzing emotional states (like anger, fear, and suffering) to provide a human-centric perspective on security.

Key Components
--------------

1.  **Crime Detection**:
    
    *   Leverages machine learning models to detect anomalous activities (e.g., theft, abuse) in public spaces such as malls.
        
    *   Models trained on diverse datasets learn to identify anomalies based on spatial and temporal features.
        
2.  **Emotion Recognition**:
    
    *   Adds an emotional dimension to surveillance by analyzing body language and emotional expressions.
        
    *   Helps in anticipating suspicious activities before they occur.
        

Methodology and Results
-----------------------

### Crime Detection

Two models using DenseNet121 architecture were evaluated:

*   **Model 1**: Exhibits higher precision (50-83%), recall (58-78%), and F1-scores (55-80%) across all classes compared to Model 2.
    
*   **Model 2**: Shows lower accuracy and tends to make more false positives.
    

Model 1 consistently outperformed Model 2 with an overall accuracy of 66% versus 58%, making it more effective in identifying anomalous activities accurately.

### Emotion Recognition

The model's confusion matrix revealed insights into the accuracy of emotional classification:

*   Model showed variable performance in recognizing different emotional states: anger was classified most accurately, but **suffering** was often misclassified due to dataset imbalance.
    
*   For example, **Class 0 (Fear)** was identified correctly 182 times, but misclassified as Anger or Suffering in several instances, demonstrating the need for a more balanced dataset.
    

### Combined Results

Testing with the **UCF-crime dataset** indicated strong performance in crime detection, though the emotion recognition model leaned toward predicting **Anger** due to the dataset imbalance.

Conclusion
----------

**Model 1** emerges as the more reliable choice for both crime detection and emotion recognition, offering higher precision, recall, and F1-scores. This model can handle the spatial and temporal complexities of video data, making it suitable for applications in security, mental health, and human-computer interaction. Future improvements in data balancing and model refinement may lead to further enhancements in accuracy and applicability.

Keywords
--------

*   Crime Detection
    
*   Emotion Recognition
    
*   Computer Vision
    
*   Deep Learning
    
*   Video Analytics
