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
- Patterns: Single-burst (200ms), double-burst (400ms), ramp-up (0% to 100% PWM duty cycle in 2s), wave (fluctutate between 0% and 75% PWM duty cycle every 100ms for 2s). Orders were randomized for each participant.
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

Summary: Participants prefer a medium‑high intensity wave pattern (fluctutate between 0% and 75% PWM duty cycle every 100ms for 2s), offering the best tradeoff for intuitiveness and physical comfort. 100% intensity remains useful for critical alerts; 25% is comfortable but too subtle to rely on.
