# FrameProcessor

A [Micro-Manager](https://micro-manager.org/) plugin that can process stack images in time. The processing can be applied in real-time (live mode) or during an acquisition (MDA).

This plugin has been inspired from the excellent FrameAverager plugin from [OpenPolScope](http://www.openpolscope.org/pages/MMPlugin_Frame_Averager.htm) available on github at https://github.com/LC-PolScope/Micro-Manager-Addons.

The motivation to create this plugin was to make it compatible with Micro-Manager 2 and also add more processing operations.

# Features

- This plugin can perform several classic operations during **live** or **MDA** such as `mean`, `sum`, `max` and `min` on a certain number of frames defined by the user.
- Images are processed for each combinations of Z, Channel and Stage Position.
- User can choose a set of channels to be ignored by the processor.

![Screenshot of the Frame Processor plugin](/screenshot.png)

# Usage

- Download the JAR file at https://github.com/hadim/FrameProcessor/releases.
- Copy it to `YOUR_MICRO_MANAGER_FOLDER/mmplugins/`.
- Launch Micromanager.
- Execute the plugin with Plugin ▶ On-The-Fly Image Processing ▶ Frame Processor.
- Launch a live or MDA acquisition.
- The acquisition window should display the processed images (mean image of the last 10 images by default).

Please report any issue to https://github.com/hadim/FrameProcessor/issues.

# Develop

- Import the project into Netbeans/Eclipse (Ant project).
- Add the appropriate MM JAR files to the properties of the project (follow [theses instructions](https://micro-manager.org/wiki/Writing_plugins_for_Micro-Manager)).
- Hack it !
- Launch Micromanager directly from Eclipse/Netbeans by running Debug.

# Authors

`FrameProcessor` has been created by [Hadrien Mary](mailto:hadrien.mary@gmail.com).

This work started in 2016 at the [Gary Brouhard laboratory](http://brouhardlab.mcgill.ca/) at the University of McGill.

# License

GPLv3. See [LICENSE](LICENSE)
