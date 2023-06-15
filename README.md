## Citation
If you use this repository, please cite the following paper. This paper has been accepted and will be published later.

Li, Y., Karim, M. M., & Qin, R. (2023 June). A Gaze Data-based Comparative Study to Build a Trustworthy Human-AI Collaboration in Crash Anticipation. In International Conference on Transportation and Development 2023.

~~~~  
@article{li2021gaze,
  title={A Gaze Data-based Comparative Study to Build a Trustworthy Human-AI Collaboration in Crash Anticipation},
  author={Li, Yu and Karim, Muhammad Monjurul and Qin, Ruwen},
  booktitle={International Conference on Transportation and Development 2023: Airfield and Highway Pavements},
  year={2023},
  organization={American Society of Civil Engineers Austin, TX}
}
~~~~
# Eye tracker data

Data was collected from Tobii Fusion screen-based Eye Tracker. The study invited six volunteers to participate in the study. Their ages are between 21∼45 years old. All participants have a drivers' license with 2∼18 years of driving experience. 

# Video data
This study collected drivers' gaze data by letting participants watch dashcam captured videos of driving scenes in the lab setting. 
Original videos are downloaded from https://github.com/Cogito2012/CarCrashDataset. Each video lasts 5 seconds, and the frequency of the videos is 10 Hz.
We selected 100 videos for participants: 50 of these are positive videos containing a crash, and the remaining 50 are negative videos with no crash at all. 
In "video_selection.csv" file: "Class" states the video is positive or negative; "video_no" is the video number; "selected?" indicates that whether this video is selected in our experiment; "ego_involved?" means the crash is ego involved or not. 

# Risk objects data
Risk objects in 50 positive videos are obtained manually and found in "RiskObj_Feature.csv" data. Here the risk object means the vehicle involved in the crash. (For example, vehicle 1 crashed into vehicle 2 crashes caused by avoiding vehicle 3; only vehicles 1 and 2 are risk objects).  If the ego vehicle is the only vehicle that crashed, the risk object is the vehicle that caused the crash. 
This is an example of the comparision of video frame with/without the risk object highlighted:

![image](https://github.com/yuli1102/eye_tracker_data/assets/44143351/dbb3da20-d294-4cc7-9caf-0d3bf21c78cb)
![image](https://github.com/yuli1102/eye_tracker_data/assets/44143351/be72a1da-f8ac-48b8-a778-2f5efed977c7)

Note that these highlighted frames are only used in analysis, and participants didn't see these highlights. 

# Gaze Data
Each volunteer watched the video sequence twice. They took a break for at least 30 minutes between the two times of experiments. Twelve experiments data can be found in the release "Raw gaze data". Gaze data are collected and classified into fixation, saccade, and Unclassified by the software of Tobii Pro Lab. This image shows an example of gaze distribution:
![image](https://github.com/yuli1102/eye_tracker_data/assets/44143351/605e2c21-e020-4ce6-9774-8f9c70746242)

# Spatial Distribution of Drivers’ Attention
These are heat map of fixation count for negtive and positiive videos. The left is negative and right one is positive result:
![image](https://github.com/yuli1102/eye_tracker_data/assets/44143351/334b2466-21a7-490f-b810-f2ff4d70dd33)

# Measures
More analysis based on this diagram can be found in the paper. 
![image](https://github.com/yuli1102/eye_tracker_data/assets/44143351/dc363cf2-2b06-4481-925c-bc9de93a060c)

Our paper was submitted and accpeted to 2023 T&DI ICTD-Pavements Conference. The paper will be published later. You can find the submitted paper can be found in arXiv: http://arxiv.org/abs/2108.01599
