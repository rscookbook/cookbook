# Installing and Working with OpenDroneMap (ODM)
Contributed by: Connor McRae-Pharo, MSc
Publication date: 25 July 2025

OpenDroneMap (ODM) is an open-source toolkit designed to process aerial imagery captured by drones into usable spatial data. At its core, ODM takes collections of overlapping photos and turns them into high-resolution geospatial products such as orthophotos, 3D models, point clouds, and digital surface models/digital terrain models. These outputs can then be used for mapping, monitoring, or analysis across a wide range of environmental and spatial research applications.
If you’ve used commercial drone mapping platforms like Pix4D or DroneDeploy, you’ll find that ODM provides many of the same core capabilities, but with a few key advantages. It’s free to use, fully customizable, horizontally scalable, fairly forgiving, and built by a global community of developers/researchers. This makes it especially useful for academic work, long-term research projects, or any situation where transparency, reproducibility, and cost control are important, which is often the case with any level of academic research.
Whether you're mapping wetlands, monitoring forest change, or building a 3D model of a heritage site, ODM gives you the tools to turn raw imagery into a meaningful spatial product.
Installation Overview
ODM was originally developed as a standalone command-line application for photogrammetric processing. More recently, it has expanded into a multi-component software ecosystem designed to support image processing, spatial analysis, and visualization of aerial datasets. The core components of this system include ODM, NodeODM, WebODM, CloudODM, PyODM, and ClusterODM.
For the purposes of this guide, we will be focusing on ODM, NodeODM, and WebODM, with installation beginning with WebODM. WebODM provides a graphical interface for users and manages the deployment of both ODM and NodeODM automatically. This level of ODM is the most beginner friendly and provides a good pivot point to using the base command line ODM, which is often lighter/faster. While the initial setup of WebODM requires limited command-line interaction, the majority of user operations can be conducted through the graphical interface. Once we’ve gotten the WebODM up and running on your personal rig accessing to ODM via the terminal will be a few steps a way and introduced in at the end.
Platform Requirements 
ODM and its associated components are supported across all major operating systems, including Windows, macOS, and Linux, but this guide will be limited to Windows OS. Installation is facilitated through Docker, a containerization platform that encapsulates software environments and their dependencies. 
To run ODM effectively, your system needs to meet certain minimum specifications. At a minimum, a 64-bit CPU, 20 GB of available disk space, and 4 GB of RAM are required. With these specifications, the system can process approximately 100–200 images before encountering memory limitations.
For more reliable performance, particularly when working with larger datasets, a more capable machine is recommended. A recent-generation CPU, 100-200 GB of available disk space, and at least 16 GB of RAM will allow you to process several hundred images without major performance issues. More CPU cores will speed up processing times, though at this time, the presence of a dedicated GPU does not significantly affect performance. If you expect to process thousands of images, you should scale your RAM and storage linearly in proportion to the size of your image sets.
Installing on Windows
To my understanding Windows 7 is the oldest version that is supported by WebODM, kudos to you if you’re still using Windows 7. This installation is geared towards Windows 10.
Step 1: Enable Virtualization
Docker, the container platform used to run WebODM, requires hardware virtualization to be enabled in your BIOS. For some reason this setting is often disabled by default.
To check whether virtualization is enabled, open Task Manager (Ctrl + Shift + Esc), switch to the Performance tab, and look for the Virtualization entry. If virtualization is not enabled, you will need to reboot your computer, enter the BIOS or UEFI settings during startup (often by pressing F2, F10, F12, or Delete), and enable the VT-x or AMD-V option. Search online using your specific motherboard model for detailed instructions if needed.
Step 2: Install Required Software
You’ll need to install the following:
1.	Git, for downloading the source code.
2.	Python (version 3.xx), which is required for some scripts and tools.
When installing Python, ensure that the Add Python to PATH option is selected during setup. This ensures Python is available from the command line.
The version of Docker you install depends on your Windows edition if you're using Windows 10 Home, install Docker Toolbox, if you're using Windows 10 Professional or newer, install Docker Desktop.
Do not install both Docker Toolbox and Docker Desktop. Choose the one appropriate for your system, as running both can cause conflicts.
Once installed, launch Docker from the provided desktop shortcut
Step 3: Allocate Memory and CPU to Docker
Docker runs in a virtual machine on Windows. To ensure WebODM has enough resources, you’ll need to adjust memory and CPU allocation.
If using Docker Toolbox, open VirtualBox Manager, right-click the default VM, and shut it down using ACPI Shutdown. Then open Settings, go to the System tab, and increase the Base Memory slider to about 60–70% (or whatever your comfortable with) of your total system memory. Under the Processor tab, you can allocate around 50% of your CPU cores. Click OK, then restart the VM.
If using Docker Desktop, locate the whale icon in your system tray, right-click it, and open Settings. Under the Advanced tab, adjust the memory and CPU sliders similarly to above, and apply the settings
Step 4: Download WebODM
Open Git GUI, which comes bundled with Git. In the Source Location field, enter:
https://github.com/OpenDroneMap/WebODM
Then, under Target Directory, browse to a folder where you’d like WebODM to be stored. Click Clone to begin downloading the repository.
Step 5: Launch WebODM
From Git GUI, go to the Repository menu and select Git Bash to open a command line window. In the terminal, type:
./webodm.sh start
This command initiates the download of all necessary components: WebODM, NodeODM, and ODM. Once complete, you’ll see a series of messages confirming that services are running.
To access the WebODM interface:
1.	If you're using Docker Desktop, open a web browser and go to http://localhost:8000
2.	If you're using Docker Toolbox, run docker-machine ip in your terminal to retrieve your machine’s IP address, then navigate to http://<IP_ADDRESS>:8000 in your browser.
Wrapping Up
Once the installation process is complete and ./webodm.sh start has been successfully executed, WebODM can be accessed via your web browser. The first time you open the application, you’ll be greeted by a welcome screen and prompted to create your first user account. From there, you can begin exploring the WebODM dashboard, which serves as the central interface for managing projects, uploading imagery, initiating processing tasks, viewing results, using the 3D model viewer, etc...
Take a moment to navigate the interface and explore the available menus. Under the Processing Nodes section, you’ll notice that a node, odm-1, has already been configured and is ready for use. This node runs locally on your PC and was automatically set up during installation process.
For those encountering installation issues or needing help with basic maintenance tasks, the README is a good place to start and provides the most up-to-date guidance. Additionally, I really recommend poking around the OpenDroneMap Community Forum as it is an active and supportive space where users can ask questions, share solutions, and stay informed about new developments.
If you’ve made it this far you should have WebODM installed and running, and you're now ready to begin processing drone imagery and generating beautiful geospatial products. The next step is to upload a dataset, start a task, and see the software in action. 

Welcome to the wonderful world of OpenDroneMap!


