---
sidebar_position: 1
slug: manual
---

Click **[Preferences] -> [AI App]**, choose **[ADAS]**, you can see the **[Rolling Stop]** Alarm:
<img src="assets/stop1.png" width="70%" />

## Alarm Type
The difference between selecting "Alarm" and "Event" as the alarm type is explained below:

| Alarm Type | Description |
| :--- | :--- |
| Alarm | When an alarm is triggered, this will report to the platform |
| Event | When an alarm is triggered, this will not report to the platform |


## Trigger
Click **[Trigger] -> [Setup]**:
<img src="assets/stop2.png" width="50%" /> <br/><br/>

| Parameter  | Description |
| :--- | :--- |
| **Detection Distance** | This parameter defines the distance at which the ADAS camera starts providing alerts when detecting a stop sign. Typically, the ADAS camera can detect stop signs from 20 to 30 meters away. If set to 10 meters, the device will alert the driver with both audio and visual notifications on the R-Watch when the vehicle is 10 meters from the stop sign. |
| **The Minimum Speed is Greater Than ... in ...** | This parameter defines the condition for triggering a stop sign alert. If the minimum speed of the vehicle within the specified time exceeds the set speed threshold, a stop sign alert will be triggered. |
| **Effective Time** | Select a time frame between 0 and 10 seconds. Any multiple rolling stop alarms triggered within this time frame will be considered as the same alarm |
| **Do not refresh the alarm timer** | By default, this option is unchecked, meaning that any multiple rolling stop alarms occurring within a certain time frame (effective time) will be treated as the same alarm, and the effective time will be reset accordingly.<br/>When checked, if multiple alarms of the same type occur within the same time frame, they will still be considered part of the same alarm. However, the effective time will not be reset, meaning that if the total duration of the alarm exceeds the effective time, the alarm will end, and its duration will be recorded as the effective time. After the effective time, a new alarm will be recorded, starting from when the previous alarm ended. |


When the ADAS camera detects the stop sign,  <img src="assets/stop4.png" width="30" /> will appear on the R-Watch in full screen without blinking until the detection ends.

## Linkage
<img src="assets/stop3.png" width="50%" /> <br/><br/>

| Parameter  | Description |
| :--- | :--- |
| **Channel**<br/> | After an alarm is triggered, select one or more channels. The video from these channels will be marked as alarm footage. |
| **Post Recording**<br/> | After the alarm ends, the video from the selected channel will be delayed for a period of time and marked as alarm footage. |
| **Lock**<br/> | The locked alarm footage cannot be overwritten until the recording protection time has elapsed or it is manually unlocked. It will not be overwritten even if the storage is full. |
| **Linkage Screen**<br/> | After an alarm is triggered, if an external screen is connected, the screen will automatically switch to the designated view. |
| **Detected MP3 Voice** | When a stop sign is detected, the main device will play the voice message: "Watch out for stop sign." |
| **Detected R-Watch Voice** | When a stop sign is detected, the R-Watch will emit a beep sound |


## Alarm Capture
<img src="assets/stop5.png" width="50%" /> <br/><br/>

| Parameter  | Description |
| :--- | :--- |
| **Capture Mode**<br/> | You can choose between **Single Capture** and **Cycle Capture**.<br/>**- Single Capture**: This option captures a single image each time. After the capture interval, another image will be taken. The total number of captures and the interval between each capture are determined by the parameters below.<br/>**- Cycle Capture**: This option captures multiple images at once each time. After the capture interval, it will continue capturing images in a cycle until the alarm's effective time ends. The number of images captured each time and the interval between captures are determined by the parameters below. |
| **Capture PCS** | See above |
| **Capture Interval**<br/> | See above |
| **Channel**<br/> | Select the channels for which images need to be captured. You can choose the image resolution and quality, as well as whether to upload the images via FTP. |

<br/><br/><br/><br/><br/>

