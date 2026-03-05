# ITSC-2026

This repository contains experimental data, evaluation metrics, and documentation associated with a study on vehicle teleoperation. The project focuses on how predictive visual aids can reduce the negative effects of network delay during remote driving.

## SYSTEM DEMONSTRATION
<video src="https://github.com/user-attachments/assets/167f1b2a-74db-4614-96e2-a59c834f0df9" width="100%" autoplay loop muted playsinline></video>

## RESEARCH FOCUS
We collected teleoperation data from ten participants with different backgrounds in driving and gaming. Operators controlled the KALIPSO research vehicle on a physical test track in Madrid, Spain, while we measured driving accuracy and mental workload using the NASA Task Load Index. 

## INTERFACE EVALUATION
The project compares three specific setups:

- **Baseline:** Raw video feed without any extra help.

- **Telemetry HUD:** Video with real-time data like speed and network status.

- **Augmented Reality (AR):** Predictive lines showing the future path of the car to compensate for lag.

## TECHNICAL HIGHLIGHTS
The system architecture is built for reliability and speed, using WebRTC for sub-second video streaming and command handling. To ensure easy installation and avoid software conflicts, all components run inside Docker containers. The vehicle itself integrates with the Openpilot ecosystem, allowing the remote station to send steering, throttle, and braking commands directly to the car's internal bus.

## KEY RESULTS AND CONCLUSIONS
The experimental data proves that adding predictive visual aids is essential for safe remote driving. The Augmented Reality interface reduced lateral deviation by almost 80 percent compared to the standard video feed. Furthermore, although the network delay remained the same during all tests, operators reported that the delay felt much less annoying and their mental workload decreased significantly when using the AR lines.

The study also found that these visual aids help bridge the skill gap between different types of users. While experienced gamers initially handled lag better, the AR interface allowed non-gamers to reach the same performance level as experts. In conclusion, predictive interfaces are a vital requirement for the future of vehicle teleoperation as a safe fallback for autonomous systems.

## REPOSITORY STRUCTURE
### DATA/
Raw data including GNSS (GPS) coordinates and system messages collected during the experiments.

### DOCS/
Technical documentation and the research paper regarding the system architecture and results.

### MEDIA/
Visual assets, including images of the hardware setup and trajectory visualizations.

### RESULTS/
Analysis of driving stability and summaries of the human factor surveys.

