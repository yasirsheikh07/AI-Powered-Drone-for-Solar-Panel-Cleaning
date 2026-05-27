## Mission Planner Software: Step-by-Step Process

### Step 1: Install and Launch Mission Planner
- Download and install Mission Planner from the official website.
- Connect your Pixhawk to your laptop using a USB cable.
- Open Mission Planner and select the correct COM port and baud rate (usually 115200).
- Click `Connect` to establish a link with the flight controller.

---

### Step 2: Initial Setup and Configuration
- Go to `Initial Setup → Install Firmware` and load the appropriate firmware (usually ArduCopter).

- Calibrate the following:
  - Accelerometer (Level calibration)
  - Compass
  - Radio/RC Input
  - ESCs (Throttle calibration)
  - Flight Modes (Set modes like Stabilize, Loiter, Auto, etc.)

- Configure failsafe settings for:
  - Low battery
  - GPS signal loss
  - RC signal loss

---

### Step 3: Creating the Autonomous Mission
- Navigate to the `Flight Plan` tab.

- Use the map to:
  - Set the home location (take-off point).
  - Add waypoints for different sections of the solar panel array.

- Optionally add commands such as:
  - `DO_SPRAYER_ON`
  - `Delay`
  - `Loiter`
  - `RTL (Return to Launch)`

- Adjust altitude and speed parameters according to panel height and spraying requirements.

---

### Step 4: Write and Save the Mission
- Click `Write WPs` to upload the mission to the Pixhawk flight controller.
- Click `Save WPs` to save the mission locally for future use.

---

### Step 5: Pre-Flight Checks
Verify the following before take-off:
- Battery voltage
- GPS signal strength
- Telemetry connection
- Sprayer system status

- Arm the drone manually or through Mission Planner when all systems are ready.

---

### Step 6: Start the Autonomous Mission
- Start the mission using the RC transmitter or Mission Planner.
- The drone will:
  - Take off automatically
  - Follow predefined waypoints
  - Spray and clean targeted solar panel areas
  - Return to the launch point after mission completion

---

### Step 7: Live Monitoring During Flight
Use the `Flight Data` tab to monitor:
- Real-time drone location
- Altitude and speed
- Battery and GPS status
- Sensor readings and system messages

- Manual control can be taken anytime using the RC transmitter if required.

---

### Step 8: Post-Flight Logs and Analysis
- After landing, open `Dataflash Logs` to download flight logs.
- Analyze logs to:
  - Evaluate flight performance
  - Detect errors or anomalies
  - Improve future autonomous missions

## Note

Due to project size and hardware limitations, the original dataset and deployment code are not included in this repository. The repository contains the research workflow, AI experimentation notebooks, project documentation, and implementation methodology.
