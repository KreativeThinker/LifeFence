# Key Components of the Proposed Human Tracking System

The key components of the proposed Human Tracking System include:

1. **Arduino UNO**: 
   - This microcontroller serves as the main processing unit for the device, allowing it to read data from sensors and control outputs.

2. **Adafruit Ultimate GPS Shield**: 
   - This component is responsible for reading GPS data, specifically latitude and longitude, and is capable of connecting to multiple satellites.

3. **ESP2866 WiFi Module**: 
   - This low-cost WiFi microcontroller is used to transmit the GPS data to the cloud for storage and further access through applications.

4. **Power Supply**: 
   - A 9V DC battery is used to power the entire system, ensuring portability and ease of use.

These components work together to track the location of individuals and transmit that information to a cloud server, where it can be accessed via mobile applications or other devices [T1], [T5].


# Abstract

The proposed Human Tracking System is based on GPS (Global Positioning System) and the Internet of Things (IoT), designed to enhance safety and security for individuals, particularly children and patients in distress. This system utilizes advanced sensor technology to track, monitor, and assist individuals in various situations. By integrating GPS and IoT, the device aims to create an environment where individuals can be located at any time, significantly reducing the costs and efforts involved in tracking by various agencies. The system is designed to alert the appropriate authorities when assistance is needed, thereby improving response times in emergencies.

# Methodology

The implementation of the Human Tracking System involves several key phases:

1. **Hardware Components**:
   - The system is built using the following hardware:
     - **Arduino UNO**: Acts as the microcontroller to process data.
     - **Adafruit Ultimate GPS Shield**: Reads GPS data (latitude and longitude) and connects to satellites.
     - **ESP2866 WiFi Module**: Facilitates data transmission to the cloud.
     - **Power Supply**: A 9V DC battery powers the device.

2. **System Architecture**:
   - The architecture consists of four main phases:
     - **Client Device (Tracker Device)**: The physical device that tracks the user's location.
     - **Satellite Data Transmission**: The GPS shield communicates with satellites to obtain location data.
     - **Cloud Server (ThingSpeak)**: The GPS data is sent to a cloud server for storage and processing.
     - **Cellular Device (Mobile, System)**: Users can access the location data through mobile applications or web interfaces.

3. **Data Processing**:
   - The GPS data is collected by the Adafruit GPS shield and transmitted via the ESP2866 WiFi module to the ThingSpeak cloud server. This data can then be accessed through various applications, allowing users to monitor the location of individuals in real-time.

4. **Software Development**:
   - The device is programmed using C++ in the Arduino IDE. Libraries for the GPS shield and WiFi module are installed to facilitate communication and data handling.

5. **Testing and Validation**:
   - The system undergoes rigorous testing to ensure that all components are functioning correctly and that the GPS data is accurately transmitted and displayed on the cloud server.

# Conclusion

The proposed Human Tracking System offers a low-cost and efficient solution for tracking individuals' locations. It successfully integrates GPS and IoT technologies to provide real-time location data, enhancing safety for vulnerable populations such as children and patients. The system's architecture allows for easy access to location information through mobile applications, making it user-friendly and practical. Future developments may focus on miniaturizing the device and incorporating additional features, such as a spy camera, while maintaining affordability. This innovation not only addresses current safety concerns but also paves the way for more advanced tracking solutions in the future.


