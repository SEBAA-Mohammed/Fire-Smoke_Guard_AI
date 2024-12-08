# Introduction

Wildfires are one of the most destructive natural disasters that affect ecosystems, property, and human lives. The devastating effects of wildfires are widespread, causing loss of life, property damage, air pollution, and long-lasting environmental changes. Early detection and timely monitoring are crucial for preventing these large-scale destructions. With advancements in artificial intelligence (AI), machine learning, and real-time communication technologies, the ability to detect wildfires early and respond effectively has significantly improved. This project leverages AI-driven fire and smoke detection using YOLO (You Only Look Once) and integrates real-time location tracking and updates with Leaflet and Supabase, offering an innovative solution for wildfire monitoring.

# Problem Statement

Wildfires are a growing concern globally, and Morocco has been no exception. In 2022, the country experienced over 500 wildfires, destroying 22,762 hectares of forest. Among the most affected regions were Tangier, Tetouan, and Al Hoceima, where a total of 188 fires ravaged approximately 18,704 hectares. These incidents underscore the urgent need for more efficient monitoring and detection systems to prevent catastrophic wildfires. 

The inability to detect wildfires early on often results in significant loss of life and property. Currently, fire detection systems rely on manual methods, including patrols and visual inspections, which can be slow, inefficient, and costly. In addition, many remote areas are difficult to monitor, making it challenging to respond quickly in critical moments. Consequently, a more robust, automated solution for wildfire detection is urgently needed to protect both the environment and human lives.

# Objectives

This project aims to address these challenges by implementing an AI-driven wildfire detection system that provides real-time updates to authorities and stakeholders. By using YOLO (You Only Look Once) for fire and smoke detection, the system will be capable of identifying fire outbreaks quickly and efficiently, even in remote areas. The detection system will integrate with real-time mapping technology using Leaflet and Supabase, enabling faster and more accurate responses.

Specifically, the project has the following objectives:

1. **Fire and Smoke Detection**: Implement YOLO to detect fire and smoke using video feeds from cameras deployed in forests and fire-prone areas.
   
2. **Real-Time Communication**: Use Supabase for real-time updates and data synchronization, providing authorities with instant alerts and actionable data on wildfire locations.
   
3. **Visualization and Mapping**: Integrate Leaflet to visualize detected fires on a map, showing the fire's exact location and other relevant data, such as the severity of the fire, estimated spread, and affected areas.

4. **Scalability**: Develop a system that can be scaled to cover larger areas and can be adapted for use in different regions and countries, offering a universal solution for wildfire detection.

5. **Public Awareness**: Provide a platform where the public can access information on fire outbreaks, including updates on wildfire status and safety recommendations, helping them stay informed and take precautionary measures.

# Technology Stack

## YOLO (You Only Look Once)

YOLO is an advanced real-time object detection algorithm that can identify multiple objects in images and video streams with high speed and accuracy. For this project, YOLO will be used to detect fire and smoke in video feeds from cameras deployed in forested and wildfire-prone areas. YOLO's real-time processing capabilities are ideal for wildfire detection, as it can detect even small fires early, reducing response times and potentially saving lives.

## Supabase

Supabase is an open-source real-time database that integrates seamlessly with PostgreSQL, providing real-time updates and data synchronization. In this project, Supabase will serve as the backend to handle all data-related operations, including the storage of fire detection data, tracking fire locations, and providing real-time updates to authorities and the public. Supabase's real-time features will ensure that once a fire is detected, the system immediately alerts relevant stakeholders, minimizing response delays.

## Leaflet

Leaflet is a widely-used open-source JavaScript library for interactive maps. It is lightweight, easy to use, and highly customizable, making it the ideal choice for visualizing wildfire detection data. Using Leaflet, the system will display detected fire locations on a map, providing real-time information about the fire's spread and severity. The integration with Supabase will allow the map to update in real time as new fires are detected and tracked, ensuring that stakeholders have access to the most up-to-date information.

# Methodology

### 1. Fire and Smoke Detection

To detect fire and smoke, the system will leverage YOLOv5, a state-of-the-art version of YOLO. YOLOv5 is highly effective for real-time object detection in videos and images, and it will be trained to recognize fire and smoke from video streams captured by cameras in the field. The system will continuously monitor the camera feeds, process the images using YOLOv5, and trigger an alert whenever fire or smoke is detected.

The algorithm will be trained on a custom dataset containing various images of fire and smoke from different environments to ensure high accuracy and reliability in diverse conditions. Once trained, the model will run on a continuous loop, identifying potential wildfire occurrences with minimal false positives.

### 2. Data Storage and Real-Time Updates

After detecting fire or smoke, the system will store the data in a PostgreSQL database using Supabase. The database will include information such as the location of the fire, the time of detection, and other relevant metadata. Supabase's real-time capabilities will ensure that once a fire is detected, the data is instantly synchronized across all connected clients, alerting authorities, emergency services, and the public about the fire's location and status.

### 3. Mapping and Visualization

Leaflet will be used to create a dynamic, interactive map that displays detected fire locations. The system will use GPS data from the camera systems to pinpoint the exact coordinates of the fire on the map. As new fires are detected, the map will update in real time, ensuring that stakeholders have the latest information. The map will display not only fire locations but also other useful data, such as the estimated size of the fire, its current spread, and any evacuation zones.

The map will also feature different layers, allowing users to filter information based on the severity of the fire, the time of detection, or the location. This functionality will help authorities prioritize their responses and deploy resources more efficiently.

# Expected Results

The primary result of this project will be the successful implementation of a real-time wildfire detection and monitoring system that leverages AI, machine learning, and real-time communication technologies. The system will provide:

1. **Early Detection of Wildfires**: The integration of YOLO for fire and smoke detection will enable rapid identification of fires, even in remote areas, reducing the time needed for emergency responses.

2. **Real-Time Updates and Alerts**: Using Supabase's real-time capabilities, the system will instantly notify authorities and the public of new fire incidents, ensuring faster action and better coordination.

3. **Accurate Location Tracking**: Leaflet will provide an interactive map that accurately tracks fire locations, offering crucial information for decision-making and resource allocation during firefighting efforts.

4. **Scalability and Adaptability**: The system will be scalable, enabling it to be deployed in different regions and adapted to various environmental conditions.

5. **Public Awareness**: By providing real-time updates to the public, the system will help raise awareness of fire dangers and promote safety measures, reducing the risk of injury and property damage.

# Conclusion

This project offers an innovative and scalable solution for wildfire detection, leveraging the power of AI, machine learning, and real-time communication technologies. The combination of YOLO for fire detection, Supabase for real-time updates, and Leaflet for mapping will provide a comprehensive and effective tool for monitoring wildfires. By improving detection accuracy, response times, and overall public safety, this system will contribute significantly to efforts to combat the growing threat of wildfires globally. The system's potential to save lives, protect property, and preserve natural ecosystems makes it a valuable tool in the fight against wildfires.
