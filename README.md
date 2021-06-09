# **novemberdev_object_pooling_godot**

This is an experimental plugin for ObjectPooling in godot.

## Installation

Drop the addons folder into your project and enable the plugin by going to 

**project > Plugins > Check Enable on ObjectPooling**

## Usage

Simply click on ObjectPooling to the top right of your Godot-Editor to open the UI.

![Screenshot](screen_2.png)

## How does it work?

The ObjectPooler scans your Project for scene-Files and then displays them in the UI. Every scene has a number of instances assinged to it. On boot, the ObjectPooler will create that amount of instances for you to use. If you close the UI, it will automatically register itself as an autoload for your convenience.

More details on that are within the UI.

# Notes to this demo
This demo uses unique materials on purpose. Godot is very fast at instancing scenes but not at initializing them. I believe it is shader compilation that adds latency once the object can be seen, this plugin makes the stuttering go away. I tested this in Nov Run, a game I deployed to the Google Play store. If your pc is really fast, you may not even notice it, but in the real world with complex scenes, it really shows.

# Screenshots

## With ObjectPooling enabled:
![Screenshot](screen_0.png)

## Without ObjectPooling enabled:
![Screenshot](screen_1.png)

