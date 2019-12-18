# The Pantora AxF Viewer snap

  The Pantora AxF Viewer is 3D viewer for AxF Materials. Pantora AxF Viewer allows users to visualize and swap 3D materials in a controlled scene with real-time rendering. No need to be an expert in computer graphics. Just drag-and-drop materials. Change the lighting to see how a material would look under different conditions.

  https://www.xrite.com/service-support/downloads/p/pantora_free_viewer_v1_0_0

  This code enables Pantora AxF Viewer to work on Linux

## Install

    sudo snap install --dangerous ./pantora-free-viewer_1.0_amd64.snap


![pantora-free-viewer](screenshot.jpg?raw=true "pantora-free-viewer")

## NVIDIA

workaround for latest nvidia drivers not working with snap

```bash
GLCORE=`ls /usr/lib/x86_64-linux-gnu/libnvidia-glcore.so.[0-9]*.[0-9]*.[0-9]*`
sudo ln -vs $GLCORE ${GLCORE%.[0-9]*}
```