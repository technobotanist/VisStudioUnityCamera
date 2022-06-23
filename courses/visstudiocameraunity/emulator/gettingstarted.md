---
layout: page
title: "Getting Started with the Visualization Studio Emulator"
course: "visstudiocameraunity"
unit: 3
---

## Welcome to the 3D Visualization Studio Emulator

When setting up your Unity 3D project meant for the Visualization Studio you may want to use an emulator to help visualize what your project will look like within the space. The emulator has an altered version of the 3D camera system to allow it to project what it sees onto an in-editor replica of the Visualization Studio. The camera has defined features that can be altered for optimization within your specific project, however, the instructions within this section are for general use and may not pertain to a specialization you require. If any questions arise while following these instructions or adjusting the camera, please contact ---@ncsu.edu.

---

## Setting up your project

Before anything else, you are going to need a new or existing Unity 3D project to put the camera into. The camera system was developed for Unity Version 2021.3.4f1 and if you already have a project created on a different version and you are adapting it for the Visualization Studio, that is perfectly fine. Just know that some of the instructions provided may differ if you are using a different version and this instruction set does its best to keep the instructions general, but images and videos may not reflect your exact Unity setup.

---

## Download the 3D camera package

Below you will find the link to a github repo with the emulator package. You will want to download the package file named ```3DEmulator.unitypackage```.

* [3D Camera Package Download](https://github.com/Elliott-Schultz/VisStudioTesting/blob/main/Assets/Packages/3DEmulator.unitypackage)

---

## Switching to the Universal Render Pipeline

The ```Universal Render Pipeline``` was utilized to make the camera function properly on the projectors within the Visualization Studio. The Universal Render Pipeline can be installed through Unity's ```Package Manager```.

To configure your project to use Universal Render Pipeline we recommend that you follow the instructions found [here](https://www.tomstephensondeveloper.co.uk/post/unity-universal-render-pipeline-urp-initial-setup) as the instructions walk through every aspect of the configuration process.
