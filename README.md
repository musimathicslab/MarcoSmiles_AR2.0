# MarcoSmiles AR 2.0

MarcoSmiles AR 2.0 is the latest iteration of the MarcoSmiles AR system, focusing on efficiency, usability, and enhanced musical interaction. The platform retains the distributed AR architecture while optimizing training and performance workflows.

## Overview

- **Platform:** Meta Quest 3 headset (AR), high-performance server for computation
- **Purpose:** Improve user experience, reduce training complexity, and support creative musical expression
- **Key Features:**
  - Optimized data acquisition: single-session hand-position capture
  - Automatic detection of stable hand poses without fixed timing constraints
  - Decoupled data acquisition and model training for flexibility
  - Enhanced performance interactions:
    - Octave control via hand height along coronal plane
    - Repeated-note triggering via forward motion along sagittal plane
  - Dedicated MIDI management for external DAW integration
    
## Resources
- 🎬 The video is not yet available, but it is under review and will be published as soon as possible.
  
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
