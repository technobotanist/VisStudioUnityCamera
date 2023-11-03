---
layout: page
title: "Setting Up a Project for the Visualization Studio"
course: "visstudiocameraunreal"
unit: 1
---

<iframe id="top" src="https://www.youtube.com/embed/ewRKuI49vPQ" name="embed" width="854" height="480" title="Visualization Studio Unreal Engine Setup Walkthrough" allow="autoplay" allowfullscreen="true"></iframe>

<hr>

<h4> <a href="codesnippets.html" target="_blank">Code Snippets</a></h4>
<h4>Jump To:</h4>
<p1>
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=0&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[00:00]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[00:00]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=76&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[01:16]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[01:16]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=138&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[02:18]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[02:18]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=164&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[02:44]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[02:44]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=177&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[02:57]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[02:57]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=229&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[03:49]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[03:49]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=653&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[10:53]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[10:53]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=689&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[11:29]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[11:29]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=703&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[11:43]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[11:43]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=773&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[12:53]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[12:53]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=848&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[14:08]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[14:08]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=1109&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[18:29]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[18:29]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=1477&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[24:37]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[24:37]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=1797&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[29:57]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[29:57]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=1840&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[30:40]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[30:40]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=1873&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[31:13]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[31:13]</a>  ||  
<a href="https://www.youtube.com/embed/ewRKuI49vPQ?start=1915&autoplay=1" target="embed" allow="autoplay" onclick="document.getElementById('[31:55]').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' });" >[31:55]</a><br><br>
</p1>
---

<div style="height: 250px;overflow: scroll;">
<h4>[00:00]</h4>
<ul>
  <li>Begin with a C++ Unreal Project (if using an existing Blueprint-only project, it must first be converted to a C++ project).</li>
  <li>In the content browser, navigate to C++ Classes, and then into the folder with your project’s name.</li>
  <li>Create a new C++ class with Actor as the Parent Class.</li>
  <li>Name this <b>“ASplitScreenManager”</b></li>
  <li>Copy all of the provided code for ASplitScreenManager.cpp, and replace the default code with it.</li>
  <li>For ASplitScreenManager.h copy ONLY the line <em>void ApplyEightViewportSettings();</em> and insert that line directly under <em>AASplitScreenManager();</em></li>
  <li>Save the files, and return to the editor.</li>
</ul>
<p id="[00:00]"></p>
<br><br>

<h4>[01:16]</h4>
<ul>
  <li>Create another C++ class, being sure to check “Show All Classes”</li>
  <li>Search for and select GameInstance as the parent class.</li>
  <li>Name this <b>“VizStudioGameInstance”</b></li>
  <li>Like before, copy all of the provided code for VizStudioGameInstance.cpp, and replace the default code.</li>
  <li>For VizStudioGameInstance.h, only the lines from  <em>public:</em>  to <em>ULocalPlayer…</em>  need to be copied from the provided code and pasted just below <em>GENERATED_BODY()</em> in Visual Studio.</li>
</ul>
<p id="[01:16]"></p>
<br><br>

<h4>[02:18]</h4>
<ul>
  <li>Back in the editor, create one more C++ class, and select GameViewportClient as the parent class.</li>
  <li>Name this <b>“VizStudioGameViewportClient”</b></li>
  <li>This requires no additional code.</li>
</ul>
<p id="[02:18]"></p>
<br><br>

<h4>[02:44]</h4>
<ul>
  <li>Now create a Blueprint class from ASplitScreenManager.</li>
  <li>Name this <b>“ASplitScreenManagerBP”</b></li>
  <li>This should be placed in your project’s Content folder. Go there now.</li>
</ul>
<p id="[02:44]"></p>
<br><br>

<h4>[02:57]</h4>
<ul>
  <li>Now to create a few more Blueprint classes.</li>
  <li>Create a Pawn class, and name it <b>“VizCameraReceiverPawn”</b></li>
  <li>Create a Game Mode Base class, and name it <b>“VizGameMode”</b></li>
  <li>Create another Pawn class, and name it <b>“VizParentPawn”</b></li>
  <li>Finally, create a Player Controller class, and name it <b>“VizPlayerController”</b></li>
</ul>
<p id="[02:57]"></p>
<br><br>

<h4>[03:49]</h4>
<ul>
    <li>Open up the VizGameMode Blueprint.</li>
    <li>Follow along with the video to continue setting up the VizGameMode.</li>
</ul>
<p id="[03:49]"></p>
<br><br>

<h4>[10:53]</h4>
<ul>
  <li>At this point, be sure that the Possess node inside your collapsed Change First Player To A Parent Pawn node has an execute output running to the collapsed node’s Outputs node.
</li>
  <li><em>Even if the collapsed nodes appear to be connected from the Event Graph, they will not be if this change is not made.</em>
</li>
  <li>From here, continue following along with the video to set up Panini Projection in the Construction Script.
</li>
</ul>
<p id="[10:53]"></p>
<br><br>

<h4>[11:29]</h4>
<ul>
  <li>Go to VizGameMode’s Class Defaults, and change the Default Pawn Class to <b>VizCameraReceiverPawn</b>, <em>NOT VizParentPawn</em></li>
  <li>Set the HUD class to None</li>
  <li>With that, the VizGameMode Blueprint is set up.</li>
</ul>
<p id="[11:29]"></p>
<br><br>

<h4>[11:43]</h4>
<ul>
  <li><em>*Technically, this section is optional if you do not plan to move the player in your project, or if you simply do not want vignetting when moving. If that is the case, skip to [14:08].</em></li>
  <li>Now, make a new material named Blur_PP.</li>
  <li>Follow the video closely for steps.</li>
</ul>
<p id="[11:43]"></p>
<br><br>

<h4>[12:53]</h4>
<ul>
  <li>It is important to note that the Input names on the Custom node are case sensitive. For example, “uv” can <b>NOT</b> be changed to “UV” without the code needing to be changed.</li>
  <li>Be sure to replace the default code in the Custom node with the code provided.</li>
</ul>
<p id="[12:53]"></p>
<br><br>

<h4>[14:08]</h4>
<ul>
  <li>Open the VizParentPawn Blueprint.</li>
  <li><em>*If you do not want movement functionality for your player, all you need for the following section is to follow the setup instructions for Event BeginPlay, and connect a GetActorTransform node to the SpawnActor node’s Spawn Transform pin as seen starting at [16:40]. </em></li>
</ul>
<p id="[14:08]"></p>
<br><br>

<h4>[18:29]</h4>
<ul>
  <li><em>*If you do not want vignetting during player movement, skip ahead to [30:40].</em></li>
</ul>
<p id="[18:29]"></p>
<br><br>

<h4>[24:37]</h4>
<ul>
  <li>You do not need to enter these values yet. At [29:57] a compiler error will require that the nodes be refreshed, and the values will be reset to their defaults. Hold off on entering those values for now.</li>
</ul>
<p id="[24:37]"></p>
<br><br>

<h4>[29:57]</h4>
<ul>
  <li>This compiler error is just Unreal not understanding that the old input names in the nodes have been changed. Unfortunately, this does mean that the values will need to be input again after the nodes are refreshed if you entered them earlier.</li>
</ul>
<p id="[29:57]"></p>
<br><br>

<h4>[30:40]</h4>
<ul>
  <li>Back in the VizParentPawn’s EventGraph, set up the Possessed Event.</li>
</ul>
<p id="[30:40]"></p>
<br><br>

<h4>[31:13]</h4>
<ul>
  <li>Now, open the VizCameraReceiverPawn Blueprint, and follow the video to set up the camera for correct use in the Visualization Studio.</li>
</ul>
<p id="[31:13]"></p>
<br><br>

<h4>[31:55]</h4>
<ul>
  <li>Lastly, open the Project Settings, and change the Default GameMode and Game Instance classes to VizGameMode and VizStudioGameInstance, respectively.</li>
</ul>
<p id="[31:55]"></p>
</div>
