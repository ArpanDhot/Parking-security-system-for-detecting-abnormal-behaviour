# Parking Security System For Detecting Abnormal Behaviour

## Project Description

This project has accomplished developing and implementing an intelligent parking management system that focuses on enhancing vehicle security and safety using deep learning algorithms. The project process entailed collecting and preprocessing a diverse video dataset representing normal activities, abnormal behaviours, and theft characteristics from various parking lots. The data was appropriately annotated, creating an adequate training set for deep learning models.

Our approach initially explored several machine learning methods, such as a human skeleton-based approach, LSTM+RCNN, and OpenCV object detection. Nevertheless, the former two methods didn't prove effective at detecting anomalies within individual automobile frames. As a result, our focus shifted towards leveraging machine learning methods to detect anomalies precisely and efficiently, which involved using bounding boxes and OpenCV for object detection.

The deep-learning model we chose utilises YOLOv5 for object detection. It's integrated into a comprehensive theft detection system that proved highly effective at detecting anomalies and notifying the driver through real-time alerts via a mobile application. While SQL was initially planned for the client dashboard database, we adopted Firebase, a cloud-based database, for more efficient and effective data storage.

Our parking management system boasts seamless integration with existing security systems, scalability, and real-world application success. It also addresses privacy and data security concerns. We developed a user-friendly dashboard for administrators and security personnel, which provides real-time parking lot information and features for managing alerts, reviewing video footage, and taking appropriate actions against potential theft incidents.

## Components of the Final System

The final parking management system comprises three main components:

### Client Application

The client application is a user-friendly, feature-rich platform that allows users to book and manage parking spaces. It provides real-time information, intuitive navigation, and a range of features that enhance the overall parking experience and enable users to make informed decisions about their parking needs.

### Security Dashboard

The Security Dashboard offers real-time monitoring and alerts of potential security threats in the monitored area. It incorporates advanced features such as number plate extraction, client checkout date verification, and real-time alerts to clients. These features provide valuable information to security personnel and system administrators.

### Object Detection Models

The heart of our security monitoring capabilities lies within the object detection models. Our approach explored several methods, including single-model detection, LSTM+RCNN, and multi-model detection. 

The final solution adopted for the system was multi-model detection, utilising YOLOv5. This approach consists of three distinct models, each having a specific role in detecting different classes of objects:

1. **Model 1:** Focuses on car-related events. It is designed to detect car doors opening and closing, number plates, and parking lots.
2. **Model 2:** Responsible for detecting individuals, particularly proficient in identifying security vests.
3. **Model 3:** Tasked with identifying tools which could indicate potential theft attempts.

## Implementation and System Overview Videos

We have prepared three videos to help you better understand our project and its components. Each video provides an in-depth overview of a specific aspect of the system.

### Video 1: Overview of the Project

This video provides a comprehensive overview of our Parking Management System project. It covers the research methodology, evaluation, and multiple aspects of the implementation process.

[![Security Dashboard](https://img.youtube.com/vi/PmKQ9ICGveY/0.jpg)](https://youtu.be/PmKQ9ICGveY "Security Dashboard - Click to Watch!")


### Video 2: Client Application Demonstration

This video offers a detailed walkthrough of the client application developed for Android. You will understand how each feature of the app works, including login, registration, menu navigation, booking, and booking log.
[![Project Overview](https://img.youtube.com/vi/9BrQgN0QSj0/0.jpg)](https://youtu.be/9BrQgN0QSj0 "Project Overview - Click to Watch!")



### Video 3: Security Dashboard Demonstration

In this video, we provide an overview of the security dashboard. We will guide you through logging in, adding channels, observing alert history, understanding the 2D homographic view, and looking into model detection. The video will also show the alert bar and how alerts are dispatched to the client with an image and an alert-type message.
[![Client Application](https://img.youtube.com/vi/CGJyasUssIk/0.jpg)](https://youtu.be/CGJyasUssIk "Client Application - Click to Watch!")



## Future Enhancements

While the system has fulfilled most of the original requirements, we acknowledge the need for future enhancements. Notably, the client application did not address the implementation of accessibility guidelines in its current version. We consider this a crucial aspect of future improvements to enhance usability for individuals with disabilities.

## Valuable Feedback

We sought feedback from industry experts to gain insights into the real-world usability of our system. One significant source was Ian, the owner of ”The Parking Consultancy Ltd.," who, with 20 years of experience in the field, provided valuable insights into potential deployment challenges and suggested further testing areas.

## Conclusion

The Parking Management System achieved its primary objectives by providing an efficient and comprehensive parking management and security solution. The system effectively caters to the needs of users, administrators, and security personnel.
