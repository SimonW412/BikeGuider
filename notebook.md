---
title: Notebook
layout: page
nav_order: 4
---

## Weekly Updates
### Week 1
All: Brainstormed project ideas.

### Week 2
All: Set up the project website and completed the project proposal. Defined core features and potential stretch goals.

### Weeks 3 and 4
Jun: PRD, finalize formative user study details.

Jiuyang, Simon: Build a prototype that generates different vibration patterns.

Please see PRD for more details.

### Week 5
We conducted a two-phase, within-subjects formative study (N=4, all university students) to evaluate user preferences for vibration intensity and pattern, focusing on intuitiveness and physical comfort.

Participants sat on a stationary bicycle equipped with vibration motors on the handlebars. In both phases, vibrations were applied to the left handlebar, right handlebar, and both handlebars simultaneously, corresponding to left turn, right turn, and U-turn.

**Phase 1: Vibration Intensity**
- Intensities: 25%, 50%, 75%, 100% PWM duty cycle. Orders were randomized for each participant.
- Participants rated each intensity on intuitiveness, comfort, and overall performance using a 5-point Likert scale.
- Participants ranked the intensities after completing all trials.

**Phase 2: Vibration Pattern**
- Patterns: Single-burst (200ms), double-burst (400ms), ramp-up (0% to 75% PWM duty cycle in 2s), wave (fluctuate between 0% and 75% PWM duty cycle every 100ms for 2s). Orders were randomized for each participant.
- Participants rated each pattern on intuitiveness, comfort, and overall performance using a 5-point Likert scale.
- Participants ranked the patterns after completing all trials.

---

**5-pt Likert Scale Results**

Vibration Intensity (higher = better)

|Intensity (% duty cycle)|Intuitiveness(avg)|Comfort(avg)|
|:---:|:---:|:---:|
|25%|1.25|**5**|
|50%|3|4.5|
|75%|4.5|3.25|
|100%|**5**|3.25|

Vibration Pattern (higher = better)

|Pattern|Intuitiveness(avg)|Comfort(avg)|
|:---:|:---:|:---:|
|Single|3.5|4.0|
|Double|4.75|4.0|
|Ramp|4.25|3.5|
|Wave|**5.0**|**4.75**|

**Ranking Results**

Vibration Intensity (lower = better)

|25%|50%|75%|100%|
|:---:|:---:|:---:|:---:|
|4.0|3.0|**1.25**|1.75|

Vibration Pattern (lower = better)

|Single|Double|Ramp|Wave|
|:---:|:---:|:---:|:---:|
|3.25|2.0|3.25|**1.0**|

Summary: Participants prefer a medium‑high intensity wave pattern (fluctuate between 0% and 75% PWM duty cycle every 100ms for 2s), offering the best tradeoff for intuitiveness and physical comfort. 100% intensity remains useful for critical alerts; 25% is comfortable but too subtle to rely on.

### Week 6

***Bluetooth Low Power***

We are trying to set up the Bluetooth Low Power (BLE) for communication between the Android App and ESP32 chip. We tried to send simple messages from Android App to esp32 chip first just for testing. Then, we planned to send more complex messages with different data structures to see whether the connection is reliable or not.

***Mapbox Map Interface***

We experimented with the Mapbox Map APIs for all navigation info. If we can successfully capture the navigation info from API, the app is responsible for sending this info to esp32. The data format is still being determined.

***Camera***

We connected OV7670 camera to ESP32 board. We identified a I2C issue caused by ESP IDF 5.4.1 and esp32-camera driver 2.0.15. The I2C communication between the camera and esp32 cannot be established (no acknowledgement issue). Downgrading the esp32-camera module from 2.0.15 to 2.0.11 temporarily solve the problem. While successfully connect camera to esp32, our esp32 board do not has external ram for frame buffer and has limited computing power.
Thus, we plan to add a MAX78000 board with camera onboard to achieve the object detection functionality and use SPI to connect esp32 and MAX78000 boards.

### Week 7
***Computer Vision***

We recieved the Max78000 board and tried to deploy existing YADES Project on Max board. However we found that the model and synthesis configuration are misconfigured and the project cannot be synthesized. We added a issue on the github to that project and currently we are debugging that project.

### Week 8
***Computer Vision***

We are still debugging the project synthesis problem.

Communication between ESP32 and Max78000 board in development. SPI and I2C protocol tested. Found Max78000 SPI and I2C driver issues. Under SPI slave mode, Max78000 does not response to the master's read request. Under I2C slave mode, Max78000 keeps pulling SCLK low, causing master timesout and failed transaction. Next step is to make Max to be the master and ESP32 to be the slave.

***PCB***

Schematic completed, pending inter-board and board-sensor communication test pass.

### Week 9 and 10
***PCB***
PCB manufacture compelete and the design is bug free.

***Enclosure***
CAD design for enclosure and mount complete. Initial prototype 3D printed. There are several flaw and error in the design so the pcb does not fit in this prototype. Refined version is being printed.

