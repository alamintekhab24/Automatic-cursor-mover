# Automatic-cursor-mover
Automatic-cursor-mover is an python script which automatically moves your cursor within a minute, so that screen will not go off.
This simple Python script utilizes the `pyautogui` library to move the mouse cursor at regular intervals. The primary purpose is to prevent the computer from going into sleep or idle mode during long periods of inactivity.

## Usage

### Prerequisites

- Python installed on your machine.
- Required library: `pyautogui`

### Instructions

1. Clone or download the script to your local machine.
2. Open a terminal or command prompt in the directory where the script is located.

```bash
python mouse_mover.py [optional: minutes]
```

- If no argument is provided, the default time interval is set to 3 minutes.
- You can customize the time interval by providing a numeric argument (in minutes) when running the script.

### Example

```bash
python mouse_mover.py 5
```

This will move the mouse cursor every 5 minutes to prevent the computer from going into idle mode.

## Notes

- The `pyautogui.FAILSAFE` attribute is set to `False` to disable the failsafe feature. The failsafe feature moves the mouse to the upper-left corner of the screen to stop the program if the mouse is moved to that location. Disabling it is essential for the script's effectiveness.
- The script continuously moves the mouse vertically within the screen boundaries, creating consistent activity.
- The script will display a timestamp in the console every time it makes a mouse movement.

## Disclaimer

This script is intended for personal use and should be used responsibly. The constant mouse movements may interfere with regular computer usage, so it is recommended to run the script when the computer is not in active use. Use at your own discretion.
