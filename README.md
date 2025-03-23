**EDJumper**

This program was created out of my frustration losing track of my jumps in *Elite: Dangerous*. Whether you're exploring deep space or grinding trade routes, this tracker helps you stay on top of your jumps with minimal effort.

Features
- **Jump Counter**: Tracks the number of jumps you've made with the press of a key or button.
- **Countdown Tracker**: Set an expected number of jumps and see how many remain.
- **Keybind Customization**: Easily change the keybind for adding jumps, including Function keys (F1-F12).
- **OBS Integration**: Outputs jump data to `obs_output.txt` for seamless overlay integration.
- **Config File**: Saves your keybind preference so it's remembered between sessions.

How to Use
1. **Start the Program**: Launch `Elite Jumps Tracker.exe`. The interface will appear.
2. **Add Jumps**: Click the **Add Jump** button or press the assigned key (default is **Spacebar**).
3. **Set Expected Jumps**: Click **Set Expected Jumps**, enter a number, and the countdown will begin.
4. **Reset Counter**: Click **Reset Counter** to start fresh.
5. **Change Keybind**: Click **Edit Keybind** and enter your desired key.

Setting Function Keys (F1-F12) as Keybinds
To bind to a Function key:
1. Click **Edit Keybind**.
2. When prompted, type `f1`, `f2`, etc., in lowercase (e.g., `f5`).
3. Click **OK** and your new keybind will be saved in `config.json`.

OBS Integration
The tracker outputs data to `obs_output.txt` in this format:
```
Jumps Made: [number]
Jumps Remaining: [number]
Expected Number of Jumps: [number]
```

In OBS, create a **Text (GDI+)** source and set it to read from `obs_output.txt` to display your jump progress on screen.

Notes
- Ensure `config.json` is kept in the same folder as the `.exe` for keybind settings to persist.
- The program must be running to track keypresses, but it will function even when Elite: Dangerous is the active window.

If you encounter issues or have feature requests, feel free to reach out!

