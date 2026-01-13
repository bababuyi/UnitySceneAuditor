# UnitySceneAuditor

A Unity Editor tool for exporting and auditing scene hierarchies, components, transforms, and script variables.

This utility helps you quickly inspect scene setup, debug wiring issues, and document complex Unity scenes by exporting the active scene’s structure to a readable text file.



## Features

* Export full scene hierarchy
* Lists all GameObjects and child relationships
* Shows Transform data (position, rotation, scale)
* Displays all components and scripts per GameObject
* Exports public variable values for each MonoBehaviour
* Safely handles:
* Unity object references
* Enums and primitives
* Arrays and lists (size only)
* Missing scripts



## Installation



1. Clone or download this repository

2\. Copy the ExportHierarchyToText.cs file into your Unity project under Assets/Editor

3\. Let Unity recompile. Dont worry this tool will **NOT** be included in your builds



## How to use

1. Open your Unity project

2\. Open the scene you want to inspect

3\. In the top menu, go to Windows and then Export Hierachy to Text

4\. Click Export Current Scene Hierarchy

5\. Choose where to save the .txt file



## Limitations



* Only public fields are exported by default
* \[HideInInspector] fields are ignored
* Private \[SerializeField] values are not included (by design)
