# 📘 LLM Context — WebXR Export

## 📌 Project Overview

**WebXR Export** is a Unity Engine XR Package/Provider for building immersive WebXR (AR/VR) experiences using Unity Web. It integrates the WebXR JavaScript API into Unity Web (WebGL) builds, allowing developers to create and export virtual and augmented reality content that runs in compatible web browsers.

This repo also includes sample projects and packages for added interactivity, such as XR Interaction Toolkit support and Mixed Reality Capture.

---

## 🎯 Purpose

This file is meant for **AI tools, contributors, and documentation generators** to understand the scope, structure, and usage of the repository, beyond the standard README. It’s designed to clarify key details that may not be fully obvious from code or folder names alone.

## 🧠 High-Level Functionality

* Exports Unity scenes and projects to WebGL that support **WebXR immersive sessions (AR/VR)**.
* Allows development using standard Unity workflows and C# scripting.
* Supports interaction packages and integration with Unity’s XR ecosystem (Unity Input System and XR Interaction Toolkit).
* Provides sample scenes and demos for reference and testing.

## 📦 Project Structure

Below are high-level directory purposes:

```
.github/                   – GitHub configs, workflows
ArtSources/                – Source art assets (if any)
Build/                     – Legacy demo
DebugProjects/             – Debug/test projects
Documentation/             – Docs and guides
MainProject/               – Core Unity project
Packages/                  – UPM packages (WebXR Export, WebXR Interactions)
XRInteractionToolkitDemo/  – Demo using Unity XR Interaction Toolkit
```

## 🛠 Tech Stack & Compatibility

* **Unity**: Supports Editor versions 2020.3.11f1 and up.
* **WebGL / WebXR**: Outputs WebGL builds compatible with WebXR APIs.
* **Languages**: C# (Unity), JavaScript (WebXR glue code)
* **Key APIs**:

  * WebXR Device API
  * WebXR Hand Input & Gamepad Modules
  * Optional WebXR Polyfill for unsupported browsers

## 🧾 Key Concepts for LLMs

**Immersive Session** – A WebXR session in VR or AR mode (e.g. VR headset or AR on mobile).

**UPM Packages** – Unity Package Manager packages; use OpenUPM registry or Git UPM import to include in projects.

**WebGLTemplates** – Provided templates that are required to build WebXR-compatible Unity Web output.

## 🚀 Getting Started (Basic Workflow)

1. **Import Packages**

   * Install `WebXR Export` and `WebXR Interactions` via OpenUPM.

2. **Configure Project**

   * Enable WebXR Export in **Project Settings → XR Plug-in Management → WebGL**.

3. **Copy WebGL Templates**

   * Use **Window → WebXR → Copy WebGLTemplates** to include required templates.

4. **Import and Test Sample Scenes**

   * Import sample scenes (from `WebXR Interactions`).

5. **Build & Serve**

   * Build to WebGL and host via HTTPS to enable WebXR (secure context required).

## 📚 Coding Conventions (General)

* Use consistent Unity coding standards.
* Keep platform-specific configuration in dedicated folders.
* Test WebGL builds often during development.
* Document any WebXR API changes in comments or issues.

## 🧪 How to Run (Example Steps)

In Unity:

* Import packages via Package Manager.
* Use provided templates and settings.
* Build for WebGL and test on a secure server (HTTPS).

## 🧩 Common Issues & Notes

* Some platforms (like certain iOS browsers) may have limited or no WebXR support.
* WebXR requires secure contexts (HTTPS).
* Projects may require manual configuration to enable specific features like hand tracking or hit tests.
* Unity XR SDK support is limited on web. Prefer Disable XR Display Subsystem in the WebXR Settings window, and use WebXRCamera component instead of the WebXRCameraSettings component.

## 🤝 Contribution Guidelines

* Open issues for bugs or feature requests using the templates.
* Follow Unity version compatibility notes.
* Reference documentation in PRs when adding features.
* Be aware this is an experimental project with evolving API support.

## 🔗 Useful Links

* Documentation folder in repo (HTML and Markdown)
* Live demo: [https://de-panther.github.io/unity-webxr-export/](https://de-panther.github.io/unity-webxr-export/)
* WebXR specs and samples resources

## 🏷 License

This project is licensed under the **Apache License, Version 2.0**.
