# Sourcetrail
A software to easily visualize Java, C/C++ or Python code. Use it to present, explain, or maintain code.
10/10 Software!!

**Source: https://github.com/CoatiSoftware/Sourcetrail**
## Installation
---

Two possibilities: install the latest release dating from December 2021: https://github.com/CoatiSoftware/Sourcetrail/releases/tag/2021.4.19

Find a recent [fork](https://github.com/CoatiSoftware/Sourcetrail/forks). As of April 2025, here is a functional one: https://github.com/petermost/Sourcetrail

AppImage available in the official repo, needs to be built in the fork.

Once installed, in the settings (Edit -> Preferences), scroll down to "Java" and add the libjvm.so to "Java Path" (https://github.com/CoatiSoftware/Sourcetrail/blob/master/DOCUMENTATION.md#finding-java-runtime-library-location). On Linux, doing `find /usr/ -iname "libjvm.so" 2>/dev/null` is sufficient to find it.

## New Project
---
For a new project: Project -> New Project

For Sourcetrail Project Name: put the name of the project. If named "toto" then at the location set in Sourcetrail Project Location a file named `toto.srctrlprj` will be created (and can be used to reopen the project).

Add a Source Group via the "Add Source Group" button. In the case where it is a Java Project, click on Java -> Empty Java Source Group (unless another option fits better RTFM), click on "Next". Once in the Java Source Group page, add folder(s) either by dragging and dropping from the file explorer, or by clicking on the small "+" and putting the **absolute** path. And finally click on "Create" (or add other Source Groups if needed).

You will arrive on a page asking how to index, click on "All Files" then "Start". Don't pay attention to potential errors, they are often unresolved names and do not prevent the software from functioning properly.

## Usage
---

To use the software in a simple way:
1. Click on "classes".
2. Choose & click on the class you want to study
3. Observe
4. Click on the element you want to observe from that view

Each time you click on an element, the code at the origin of this part will be displayed on the right of the screen.

It is possible to choose the place of observation from the search bar at the top of the screen.

You can export the current view as an image at any time by clicking on "Save as Image" in the Right Click menu.

It is possible to group by file or by packages/namespaces/modules by clicking on one of the two small icons in the upper left of the screen.

To make an in-depth view, click on the icon with a Z shape in the upper left of the screen. Once on this page you can search by choosing the "From". You can choose up to which part of the code you want to search, or if you want the whole picture of everything that leads to it, or from everywhere it has. Imagine you have 5 classes A, B, C, D and E (each dependent on the next), and in From you put B. If in "To" you put class D, then the view displayed will be B, C, D. If you put C then "-> All Referenced" then the view displayed will be C, D, E. If you put then "<- All Referencing" the view displayed will be A, B, C. You can choose the Nodes and Edges to display. Once your configuration is chosen, click on "Search".
