# Godot Bug #109930

## 1. Introduction: What is Godot?

**Godot** is a **free and open-source game engine** designed for creating both **2D and 3D games**. It provides a complete set of tools for game design, animation, scripting, and deployment—all within a single integrated environment.

The engine supports several programming languages:

- **GDScript** – a lightweight, Python-like language made specifically for Godot.
- **Visual Script** – a node-based scripting alternative for non-programmers.
- **C#**
- **C++**

Games developed in Godot can be exported to multiple platforms, including **Windows**, **Linux**, **macOS**, **Android**, **iOS**, and **Web (HTML5)**.

---

## 2. Bug 109930

The bug is found in the `Curve2D::get_closest_point()` function of the Godot Engine. The issue, discussed in [GitHub Issue #109930](https://github.com/godotengine/godot/issues/109930), causes incorrect nearest-point calculations for certain curve configurations.

---

## 3. Problem Description

The function `get_closest_point()` is designed to return the point on a curve closest to a given position in 2D space. However, under certain conditions—such as small or degenerate curve segments—the algorithm produced inaccurate results.

## 4. Methodology: Identifying and Approaching the Bug

To resolve the issue in Curve2D::get_closest_point(), the following procedure will be implemented.

### 4.1 Downloading and Building the Source

The first step will be to obtain the official Godot Engine source code from GitHub and build the project from source using Visual Studio.

### 4.2 Reproducing the Bug

Reproducing the bug using minimal test case.

### 4.3 Locating and Analyzing the Function

Locating the Curve2D::get_closest_point() function within the Godot source code and discuss several potential fixes.

---

## 4. Submitting the Changes
Read the Godot contributor guidelines and follow the instructions for submitting a pull request (PR).
