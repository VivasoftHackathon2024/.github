
![Team Image](https://res.cloudinary.com/dyktljlnj/image/upload/v1737125813/BUET_Multithreading_cover_photo_smqiop.png)

# FrameWise: AI Powered Video Analysis Platform

This project leverages advanced AI technologies to provide comprehensive analysis of video content, transforming vast amounts of unstructured video data into actionable insights. By integrating state-of-the-art Vision Language Models (VLMs) and Large Language Models (LLMs), our platform offers real-time monitoring, detailed summarizations, and interactive querying capabilities.

Key Features:

1. Automated Video Logging and Summarization: Efficiently processes and condenses extensive video footage into concise summaries for quick review.

2. Specialized Analytical Agents: Includes agents for detecting specific events such as fires, assaults, thefts, and other suspicious activities, enhancing security and operational efficiency.

3. Interactive Chat Interface: Allows users to engage with video logs through natural language queries, facilitating intuitive data retrieval and analysis.

4. Support for Streaming and Uploaded Videos: Capable of analyzing both live video streams and pre-recorded footage, providing flexibility across various use cases.

Use Cases:

1. Public Safety: Assists government agencies in monitoring and responding to criminal activities, thereby enhancing community safety.

2. Retail Analytics: Provides insights into customer behavior, supporting targeted marketing strategies and improving customer experiences.

3. Industrial Monitoring: Ensures compliance with safety protocols and detects anomalies in operational processes, reducing risks and improving efficiency.


# Technical Overview

![FrameWise Architecture Diagram](https://res.cloudinary.com/dyktljlnj/image/upload/v1737125702/framewise_architecture_ykujtj.png)

Fig: FrameWise Architecture Diagram

## List of Agents

This is a table of contents for your project. It helps the reader navigate through the README quickly.
- [Alert/Email Notifier Agent](#project-title)
- [Summarization Agent](#project-title)
- [Chat agent](#quick-start-demo)
- [Fire Detection Agent](#table-of-contents)
- [Assault Detection Agent](#installation)
- [Crime Detection Agent](#usage)
- [Drug Detection Agent](#development)
- [Theft Detection Agent](#contribute)
- [Tamper Detection Agent](#license)
- [Suspicious Activity Agent](#license)
- [Customer Behaviour Agent](#license)

## Tech Stack

- [Nvidia Cosmos 34B VLM model](#project-title)
- [OpenAI](#project-title)
- [OpenAI Embeddings](#project-title)
- [LangChain](#project-title)
- [Pgvector](#project-title)
- [PostgreSQL](#project-title)
- [Supabase](#project-title)
- [Django](#project-title)
- [ReactJS](#project-title)


## Backend Workflow

### Pre-recorded video

1. Video is uploaded
2. Uploaded video is passed through the Nvidia Cosmos 34B VLM model to generate logs every 30s which are stored on Supabase PostgreSQL Database
3. The logs are vectorized and stored in pgvector
4. Summary is generated from that vectorized information. Summary tries to detect any incident of crime/theft/assault
5. Automated agents such as fire agent, assault agent, crime agent, drug agent, etc analyze the uploaded video and give a specialised response about the severity if they are detected
6. Users can also chat with the video information using the chat agent to get more detailed and personalised information from the video logs

### Streaming services/Realtime CCTV footage

1. Video is uploaded
2. Uploaded video is passed through the Nvidia Cosmos 34B VLM model to generate logs every 30s which are stored on Supabase PostgreSQL Database
3. The logs are vectorized and stored in pgvector
4. Summary is generated from that vectorized information. Summary tries to detect any incident of crime/theft/assault
5. Users can set custom alerts by defining specific criteria they want to monitor.
6. Alert/Email agent keeps on checking for that custom requirement and sends a mail to the user if it is detected.
7. Users can also chat with the video information using the chat agent to get more detailed and personalised information from the video logs



# Other Resources and Links

## FrameWise: Deployed Application Link:

[Deployed Application Link](https://www.canva.com/design/DAGcZQZvbpg/F4Vc7P5iTI3l9LH_-X9XMA/edit?utm_content=DAGcZQZvbpg&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

## Presentation Video Link:

[Presentation Video Link](https://www.canva.com/design/DAGcZQZvbpg/F4Vc7P5iTI3l9LH_-X9XMA/edit?utm_content=DAGcZQZvbpg&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

## Presentation Slide:

[Presentation Slide Link](https://www.canva.com/design/DAGcZQZvbpg/F4Vc7P5iTI3l9LH_-X9XMA/edit?utm_content=DAGcZQZvbpg&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

## Backend Repo Link:

[Backend Repo Link](https://github.com/VivasoftHackathon2024/nvidia-video-processing.git)

## Frontend Repo Link:

[Frontend Repo Link](https://github.com/VivasoftHackathon2024/framewise-frontend.git)
