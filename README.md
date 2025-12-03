# MarcoSmiles AR 1.0

MarcoSmiles AR 1.0 is a distributed client–server augmented reality (AR) platform designed for musical interaction and performance. The system leverages a Meta Quest headset for real-time hand tracking and visualization, while heavy computation, including model training and inference, is offloaded to a high-performance server.

## Overview

- **Platform:** Meta Quest 3 headset (AR), high-performance server for computation
- **Purpose:** Enable natural, immersive music creation while addressing limitations of Leap Motion-based prototypes
- **Key Features:**
  - Distributed client–server architecture
  - Real-time gesture recognition in AR
  - Offloading of training and inference to external server
  - MIDI output for integration with external DAWs such as Ableton Live and FL Studio


## Client: MarcoSmilesClient
1. **Import the Project into Unity Hub**:
    - Open Unity Hub.
    - Click the **Add** button.
    - Navigate to the `MarcoSmilesClient` folder and select it.
2. **Configure the build settings for Meta Quest**:
    - Go to **File > Build Settings**.
    - Select **Android** as the platform and click **Switch Platform**.
3. **Configure the server IP address**:
    - In the Unity Editor Hierachy, select the `ServerCommunicator` object.
    - In the `Server Gateway` component, set the `Server URL` field to http://*serveripaddress*:5005.
4. **Deploy the application to the Meta Quest device**:
    - Connect the device via USB.
    - Click **File -> Build and Run** to deploy the application.
___

## Server: ET_MarcoSmilesServer
How to start

1. Navigate to the `ET_MarcoSmilesServer` directory.
2. Install dependencies with the command:
    
    ```shell
    pip install -r requirements.txt
    ```
    
3. Start the server with:
    
    ```shell
    python app.py
    ```
