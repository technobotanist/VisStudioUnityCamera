---
layout: page
title: "Getting Started with the Teaching and Visualization Lab Emulator"
course: "visstudiocameraunity"
unit: 6
---

## Welcome to the VisSDK Teaching and Visualization Lab Emulator

When setting up your Unity 3D project meant for the Teaching and Visualization Lab you may want to use an emulator to help visualize what your project will look like within the space without actually being in the room. The emulator has an altered version of the 3D camera system to allow it to project what it sees onto an in-editor replica of the Teaching and Visualization Lab. The camera has defined features that can be altered for optimization within your specific project, however, the instructions within this section are for general use and may not pertain to a specialization you require. If any questions arise while following these instructions or adjusting the camera, please contact library_hightechspaces@ncsu.edu.

---

## Setting Up Your Project

Before anything else, you are going to need a new or existing Unity 3D project to put the emulator into. The camera system and emulator were developed for Unity Version 2021.3.4f1 and if you already have a project created on a different version and you are adapting it for the Teaching and Visualization Lab, that is perfectly fine. Just know that some of the instructions provided may differ if you are using a different version and this instruction set does its best to keep the instructions general, but images and videos may not reflect your exact Unity setup.

---

## Install ProBuilder

In order for the emulator to load the textures of the Teaching and Visualization Lab correctly, you will need to install ProBuilder as it was used to build the emulator. You can find a tutorial for how to install ProBuilder [here](https://docs.unity3d.com/Packages/com.unity.probuilder@4.0/manual/installing.html).

---

## Download the 3D Emulator Package

Below you will find the link to a github repo with the emulator package. You will want to download the package file named ```T&VEmulator.unitypackage```.

* [3D Emulator Package Download](https://github.com/technobotanist/VisStudioTesting/blob/main/Assets/Packages/T%26VEmulator.unitypackage)

---

## Switching to the Universal Render Pipeline

The ```Universal Render Pipeline``` was utilized to make the camera function properly on the projectors within the Teaching and Visualization Lab. The Universal Render Pipeline can be installed through Unity's ```Package Manager```.

To configure your project to use Universal Render Pipeline we recommend that you follow the instructions found [here](https://www.tomstephensondeveloper.co.uk/post/unity-universal-render-pipeline-urp-initial-setup) as the instructions walk through every aspect of the configuration process.
