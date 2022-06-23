---
layout: page
title: "Getting Started with the 2D Camera"
course: "visstudiocameraunity"
unit: 2
---

## Setting up your project

First and foremost, you are going to need a 2D Unity project. These instructions are for Unity Version 2021.3.4f1. If you already have a project created and you are adapting it for the Visualization Studio, that is perfectly fine. Just know that some of the instructions provided may differ if you are using a different version of Unity. We have done our best to keep the instructions general, but images and videos may not reflect your Unity setup.

---

## Custom Resolution

In order for the camera to function properly in the Visualization Studio, you are going to need to set up a custom resolution for your display. While the Visualization Studio is an array of 8 projectors, what is displayed is considered one screen with a resolution of 15360x1080.

To set up a custom resolution, you will need to go to the game view screen in the Unity Editor.

![Switch to game view](images/gameview.png)

Next to the dropdown labeled Display 1, you will find another dropdown with the aspect ratios.

![Open aspect ratios](images/aspectratio.png)

At the bottom of that dropdown, there is an option to create a custom resolution profile. Click on that.

![Click to add custom aspect ratio](images/dropdown.png)

You can name the profile whatever you choose. For the purposes of this instruction, we will name it "VisStudio".

![Set name of custom aspect ratio](images/namevisstudio.png)

Keep the selection of Fixed Resolution and in the fields below, set the width to be ```15360``` and the height to be ```1080```.

![Set values of custom aspect ratio](images/setresolution.png)

Save the resolution and make sure that it is the one selected from the dropdown.

![Save custom aspect ratio](images/saved.png)

In your game view, the top bar should now look like this.

![Final result](images/finalaspectratio.png)

---

Now that the custom resolution is done, you are basically all set to develop 2D scenes for the Visualization Studio. With that being said, we recommend that you continue through the unit for some helpful tips and considerations that will benefit your development process and your final product.
