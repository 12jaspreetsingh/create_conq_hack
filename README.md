RoboDataHub – Egocentric Robotics Data Pipeline

🚀 Overview

This project builds a complete pipeline to transform raw egocentric (first-person) videos into structured datasets that robots can learn from.

Robots struggle in real-world environments because they lack access to high-quality human activity data. Our system bridges this gap by converting unstructured video into meaningful, machine-readable information.

🎯 Problem
Robots cannot learn effectively from simulation alone
Lack of real-world egocentric datasets (especially in India)
Existing datasets like Ego4D dataset and EPIC-KITCHENS dataset are limited and not region-specific
💡 Solution

We provide a pipeline that:

Processes raw egocentric video data
Segments human actions (start/end)
Detects hand-object interactions
Generates structured annotations
Converts them into robot-understandable formats
⚙️ Pipeline
Raw Video → Frame Extraction → Action Segmentation → 
Hand & Object Detection → Annotation → Structured Dataset
🧠 Key Features
Converts unstructured video into structured data
Generates action-level annotations (time-based)
Supports hand-object interaction understanding
Produces robot-ready action sequences
Scalable for large dataset creation
📦 Output Format

Example:

{
  "video": "video_01.mp4",
  "actions": [
    {
      "start": 0,
      "end": 2,
      "action": "pick",
      "object": "cup",
      "interaction": "grasp"
    }
  ],
  "description": "Person picks up a cup and pours water."
}
🌍 Use Cases
Robotics training datasets
Humanoid AI systems
Human activity understanding
Autonomous systems
🇮🇳 Unique Value
Focus on India-specific environments and workflows
Scalable data collection approach
Bridges vision, language, and robot actions
🛠️ Tech Stack
Python
OpenCV
MediaPipe
YOLOv8
JSON / CSV
🔮 Future Scope
Crowdsourced data collection platform
Real-time annotation system
API for robotics companies
Large-scale dataset generation
