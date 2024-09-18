# ESP3D-WEBUI-Mods
# Capture Extension for FluidNC

![Capture Extension](https://github.com/NEWTech-Creative/ESP3D-WEBUI-Mods/blob/main/capture%20Extension.png)

The **Capture Extension** is a powerful tool designed for Manual Data Input (MDI) with FluidNC. This extension allows users to log real-time position data, replay, edit, and export it as G-code for future use. It opens up possibilities for applications like camera sliders, robotic arms, and other scenarios where real-time positioning in a live environment is essential.

### Key Features:
- **Live Data Logging**: Capture live machine positions during operation.
- **Data Replay**: Revisit and replay captured positions for accurate movement replication.
- **Editable Logs**: Modify position data on the fly for precision adjustments.
- **G-code Export**: Save your captured positions as G-code for use in future operations.

This tool is particularly valuable for users looking to implement live position inputs in dynamic environments, making it ideal for applications such as:
- Camera sliders
- Robotic arms
- Any other project requiring real-time manual positioning.

> ⚠️ **Disclaimer**: This extension is currently in beta and may not account for all machine limits. Use at your own risk.

---

### How to Install the Capture Extension on WebUI3 (FluidNC):

1. **Upload** the `Capture.html` file to the flash memory on your ESP32.
2. In WebUI3, navigate to **Settings**.
3. Select **User Interface**.
4. Under **Extra Content Panel**, update with the following configuration:

   ![Capture Setup](https://github.com/NEWTech-Creative/ESP3D-WEBUI-Mods/blob/main/capture%20setup.png)

---

## How to Use the Capture Extension

### Capture a Position:
- Click 'Capture' to log the current machine coordinates.
- A new entry will appear, displaying the current position.

### Editing a Captured Position:
- To edit, click on the desired entry, and the machine will move to that location.
- Move the machine to the new position, adjust the **Feedrate** or add additional G-code.
- Click 'Capture' again to save the updated position.

### Jogging:
The extension supports two jogging modes via the buttons at the top of the interface:

1. **Short Jog**:
   - Click once to jog the machine by 1mm.

2. **Continuous Jogging**:
   - Hold down the jog button to continuously jog the machine in 10mm increments.
   - **Important**: Ensure you do not move the mouse off the jog button while holding it down, as the machine will continue to jog. This will be fixed in a future version.

### Exporting Positions as G-code:
- Click 'Save' to export your positions as G-code.
- You will be prompted to download the captured file in `.nc` format.

---

![Capture Extension UI Edit]([https://github.com/NEWTech-Creative/ESP3D-WEBUI-Mods/blob/main/capture%20Extension.png](https://github.com/NEWTech-Creative/ESP3D-WEBUI-Mods/blob/main/capture%20edit.png))
