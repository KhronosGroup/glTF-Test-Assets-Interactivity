<p align="center">
<img src="Models/glTF_RGB_June16.svg" height="100">
</p>

# glTF Interactivity Sample Assets

|  |  |
|-|-|
| [![Calculator](Models/Calculator/screenshot/screenshot.png)](Models/Calculator/README.md)  | Calculator model using Transmission and Volume extensions. [[Show]](https://gltf-interactivity.needle.tools/?model=https://raw.githubusercontent.com/needle-tools/glTF-Interactivity-Sample-Assets/main/Models/Calculator/glTF-Binary/Calculator.glb)<br>Credit:<br>&copy; 2025, Needle. [CC BY 4.0 International](https://creativecommons.org/licenses/by/4.0/legalcode)<br>


## Introduction

This Repository contains tests and samples of glTF assets using the KHR_interactivity extension, which allows for the creation of interactive 3D models. KHR_interactivity allows for the creation of interactive elements within 3D scenes, in a graph-based manner.

## Viewing the sample and test assets online

The models can be viewed in the [Graph Authoring Tool](https://gltf-interactivity.needle.tools/), which is a web-based tool that allows you to load GLB files with the KHR_interactivity extension and interact with them. A graph-based interface allows you to see the nodes and connections that make up the interactive elements of the model. You can also modify the properties of the nodes and connections, allowing you to experiment with different configurations and see how they affect the behavior of the model.

## Lists

All models are tagged to allow easier access. These lists simplify your access and review of the models. All lists include the model name, screen shot, link to display the model in Sample Viewer, a short description, and the license/credits for the model. The following lists are available

* [Showcase](./Models/Models-showcase.md) (#showcase) for models that demonstrate real-world use cases of glTF Interactivity, ranging from simple to complex.
* [Testing](./Tests/Interactivity/Interactivity-testing.md) (#testing) for assets that are designed for programmatic or manual testing of KHR_interactivity implementations. These models can either be used to verify the behavior of specific features, or added to test suites to ensure correctness of implementation.

A summary of the model license is shown in each display, but see the `README.md` in each model's directory for detailed license information.

## Model Contents

Sample glTF 2.0 models are provided in one or more of the following forms of glTF:

* glTF (`.gltf`) with separate resources: `.bin` (geometry, animation, skins) and `.jpg` or `.png` image files.  The supporting files are easily examined when separated like this, but must be kept together with the parent glTF file for the model to work.
* Binary glTF (`.glb`) using the [binary container format](https://github.com/KhronosGroup/glTF/blob/master/specification/2.0/README.md#glb-file-format-specification).  These are easily shared due to the bundling of all the textures and mesh data into a single file.

## Other glTF Models

For additional glTF models, see:

* [Khronos glTF Sample Assets](https://github.com/KhronosGroup/glTF-Sample-Assets) offers an extensive suite of models demonstrating various glTF features.

## Questions or Comments

If you have any questions, submit an [issue](https://github.com/needle-tools/glTF-Interactivity-Sample-Assets/issues).


---
&copy; 2025, The Khronos Group and Needle. Licensed as CC-BY 4.0 International