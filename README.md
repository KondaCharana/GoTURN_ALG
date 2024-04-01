# GoTURN_ALG
           +---------------------------------------------------+
           |                                                   |
           |                     Video                         |
           |                                                   |
           +---------------------------+-----------------------+
                                       |
                       +---------------v---------------+
                       |                               |
                       |     GOTURN Algorithm         |
                       |                               |
                       +---------------+---------------+
                                       |
               +-----------------------v----------------------+
               |                                           |
               |          Feature Extraction                |
               |                                           |
               +------------------+------------------------+
                                  |
                      +-----------v------------+
                      |                        |
                      |  Online Fine-Tuning   |
                      |                        |
                      +-----------+------------+
                                  |
                     +------------v-------------+
                     |                          |
                     |     Regression Network   |
                     |                          |
                     +------------+-------------+
                                  |
                     +------------v-------------+
                     |                          |
                     |     Bounding Box        |
                     |     Prediction          |
                     |                          |
                     +------------+-------------+
                                  |
                     +------------v-------------+
                     |                          |
                     |        Tracking          |
                     |                          |
                     +------------+-------------+
                                  |
                    +-------------v------------+
                    |                          |
                    |       Adaptive           |
                    |       Learning           |
                    |                          |
                    +-------------+------------+
                                  |
                    +-------------v------------+
                    |                          |
                    |    End-to-End Training   |
                    |                          |
                    +--------------------------+

Explanation of components:

Video: Input video sequence containing frames with the target object to be tracked.

GOTURN Algorithm: Main algorithmic module that orchestrates the tracking process.

Feature Extraction: Initial stage where features are extracted from the target object within the initial bounding box.

Online Fine-Tuning: Process of fine-tuning the feature extractor and regression network using online training.

Regression Network: Neural network component that predicts the bounding box coordinates of the target object.

Bounding Box Prediction: Predicted bounding box coordinates based on the features extracted from the current frame.

Tracking: Actual tracking process where the predicted bounding box is used to localize the target object in subsequent frames.

Adaptive Learning: Continuous adaptation of the tracking model based on the tracking results and feedback.

End-to-End Training: Training of the entire GOTURN pipeline in an end-to-end manner to learn tracking directly from data.
