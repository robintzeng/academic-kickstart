+++
# Experience widget.
widget = "experience"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 40  # Order that this section will appear.

title = "Experience"
subtitle = ""

# Date format for experience
#   Refer to https://sourcethemes.com/academic/docs/customization/#date-format
date_format = "Jan 2006"

# Experiences.
#   Add/remove as many `[[experience]]` blocks below as you like.
#   Required fields are `title`, `company`, and `date_start`.
#   Leave `date_end` empty if it's your current employer.
#   Begin/end multi-line descriptions with 3 quotes `"""`.
[[experience]]
  title = "ASML"
  company = "Droplet Generation Control and Automation System Intern"
  company_url = ""
  location = "San Diego, CA"
  date_start = "2020-05-21"
  date_end = "2020-08-14"
  description = """
  <br>

  * Designed an object detection pipeline from scratch by OpenCV, Tkinter and Scikit-learn in Python to detect the tin droplets and satellites for preprocessing, labeling, feature extraction and classification.
  * Detected the interest objects with maximally stable extremal regions (MSER) and eliminated the overlapped bounding boxes with Non-Maximum Suppression (NMS).
  * Evaluated the classifiers’ performance with k-fold cross validation, learning curve and validation curve.
  """

[[experience]]
  title = "Advanced Computer Vision – Improvements on Object Detection (Faster R-CNN)"
  company = "Software Team Leader"
  company_url = ""
  location = "Ann Arbor, MI"
  date_start = "2020-09-15"
  date_end = "2020-12-20"
  description = """
  <br>

  * Trained and evaluated the Faster R-CNN on PASCAL VOC 2007 with PyTorch.
  * Decoupled the classification head and localization head and improved the mAP by 1.
  * Introduced efficient channel attention and cross stage network to ResNet-50 backbone and increased 5 mAP..
  """

[[experience]]
  title = "Individual Study – Benchmark for Video Inpainting"
  company = "Team Member"
  company_url = ""
  location = "Ann Arbor, MI"
  date_start = "2020-09-03"
  date_end = "2020-12-30"
  description = """
  <br>

  * Designed algorithms to classify the degree of attributes — camera motion, foreground motion and displacement — which affect the video inpainting model performance on DAVIS dataset.
  * Evaluated the performance of the algorithm by Precision – Recall curve and ROC curve.
  """


[[experience]]
  title = "Mobile Robotics - Visual Inertia Navigation"
  company = "Team Leader"
  company_url = ""
  location = "Ann Arbor, MI"
  date_start = "2020-03-01"
  date_end = "2020-04-20"
  description = """
  <br>

  * Improved a Muti-State Constraint Kalman filter-based visual inertial navigation framework (Openvins) with learning- based interest point extractor – SuperPoint in Pytorch by using C++.
  * Evaluated the performance on the EuRoC MAV dataset with ROS and ameliorated the performance for every tasks.
  """

[[experience]]
  title = "Computer Vision - Depth Completion"
  company = "Team Member"
  company_url = ""
  location = "Ann Arbor, MI"
  date_start = "2020-03-01"
  date_end = "2020-04-20"
  description = """
  <br>

  * Completed dense depth data from a color image and sparse LiDAR data in KITTI depth completion benchmark.
  * Developed two-pathway learning architecture with U-Net like low-resolution feature extractor and utilized attention mechanism to propose the final prediction in Pytorch.
  """

[[experience]]
  title = "Self-Driving Car - Object Detection (YOLOv3)"
  company = "Perception Team Leader"
  company_url = ""
  location = "Ann Arbor, MI"
  date_start = "2019-11-01"
  date_end = "2019-12-31"
  description = """
  <br>

  * Placed 2nd overall in class and implemented and trained YOLOv3 on a given   dataset in Python with Keras.
  * Developed a layer to discriminate the distance of the objects with point cloud.
  """

[[experience]]
  title = "Eurobot 2018 Contest - Autonomous Robot"
  company = "Software Team Leader"
  company_url = ""
  location = "Taiwan/France"
  date_start = "2017-09-01"
  date_end = "2018-06-30"
  description = """
  <br>
  
  * Placed 24th overall in world counted.
  * Prototyped positioning system model with MATLAB for integration test, utilized microcontrollers and ultrawideband (UWB) chips to locate the robots accurately and practiced the whole system with C++ in Linux.
  * Implemented Kalman filter and trilateration algorithm to enhance measuring accuracy and stability, increasing 30% accuracy which is within 5 cm radius with high repeatability.
  
  
  """
[[experience]]
  title = "Mobile Robot"
  company = "Control Team Leader"
  company_url = ""
  location = "Hsinchu, Taiwan"
  date_start = "2017-09-01"
  date_end = "2018-01-30"
  description = """
  <br>
  
  * Developed a discrete-time PID controller and implemented it on Altera DE0-Nano by programming in Verilog.
  * Handled input from rotary encoders and output with PWM signals to control the rotational speed
  """

[[experience]]
  title = "Wafer Gripper"
  company = "Software Team Member"
  company_url = ""
  location = "Hsinchu, Taiwan"
  date_start = "2017-09-01"
  date_end = "2018-01-30"
  description = """
  <br>

* Designed a G-Code Interpreter to read the NC (numerical control) code and execute them on 3-axis wafer gripper.
* Built a human - computer interface and stimulated the wafer gripper’s motion by using Windows Forms.
* Implemented trapezoidal velocity profile and interpolation to control the stepper motors smoothly.
  """

[[experience]]
  title = "Powered Exoskeleton for Motion Recording"
  company = "Sensing and Communication Team Leader"
  company_url = ""
  location = "Hsinchu, Taiwan"
  date_start = "2017-05-01"
  date_end = "2017-12-30"
  description = """
  <br>

* Placed 2nd and “Most Popular” awards from 50 teams in Senior Capstone Project Competition.
* Developed a sensing exoskeleton suit consisting of 4 microcontrollers, 6 encoders and 4 inertial sensors for
detecting and recording the user’s movements, i.e. hand gestures.
* Used SPI, I2C, UART for fetching the data to the microcontrollers and fused the gyroscope and accelerometer
data by compensation filter.
* Built a Bluetooth communication system with cyclic redundancy check (CRCs) to improve its consistency.

  """
+++
