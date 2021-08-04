# eye_tracker_data

Data was collected from Tobii Fusion screen-based Eye Tracker. The study invited six volunteers to participate in the study. Their ages are between 21∼45 years old. All participants have a drivers' license with 2∼18 years of driving experience. 

This study collected drivers' gaze data by letting participants watch dashcam captured videos of driving scenes in the lab setting. 
Original videos are downloaded from https://github.com/Cogito2012/CarCrashDataset. Each video lasts 5 seconds, and the frequency of the videos is 10 Hz.

We selected 100 videos for participants: 50 of these are positive videos containing a crash, and the remaining 50 are negative videos with no crash at all. 
In "video_selection.csv" file: "Class" states the video is positive or negative; "video_no" is the video number; "selected?" indicates that whether this video is selected in our experiment; "ego_involved?" means the crash is ego involved or not. 

Risk objects in 50 positive videos are obtained manually and found in "RiskObj_Feature.csv" data. Here the risk object means the vehicle involved in the crash. (For example, vehicle 1 crashed into vehicle 2 crashes caused by avoiding vehicle 3; only vehicles 1 and 2 are risk objects).  If the ego vehicle is the only vehicle that crashed, the risk object is the vehicle that caused the crash. 

Each volunteer watched the video sequence twice. They took a break for at least 30 minutes between the two times of experiments. Twelve experiments data can be found in the release "Raw gaze data".

Our paper was submitted to TRB 2022 conference and is under review at this moment. Submitted paper can be found in arXiv: http://arxiv.org/abs/2108.01599
