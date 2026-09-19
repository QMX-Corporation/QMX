# 🎮 QMX Engine

> A lightweight, low-level 3D graphics engine built from scratch with C++ and DirectX 12.

![API](https://img.shields.io/badge/API-DirectX%2012-blue)
![Language](https://img.shields.io/badge/Language-C%2B%2B-green)
![Compiler](https://img.shields.io/badge/Compiler-Clang%20%2F%20LLVM-orange)
![License](https://img.shields.io/badge/License-MIT-purple)

---

## 📌 About The Project

**QMX Engine** is an experimental low-level 3D graphics framework designed to interface directly with modern GPU hardware via Microsoft DirectX 12. The project focuses on bare-metal pipeline management, custom HLSL shader compilation at runtime, and high-precision frame execution without heavy third-party engine abstractions.

## Key Features

* **DirectX 12 Low-Level Pipeline:** Full manual control over SwapChains, Command Queues, Command Allocators, and Fences.
* **Custom HLSL Runtime Shader Compiler:** Dynamic compilation of Vertex and Pixel shaders via `d3dcompiler`.
* **Explicit Resource & State Management:** Custom Pipeline State Objects (PSO), Root Signatures, and Input Layouts tailored for raw GPU performance.
* **VRAM Buffer Allocation:** Manual allocation and mapping of Vertex Buffers into GPU Upload Heaps.
* **High-Precision Game Loop:** Integrated `QueryPerformanceCounter` system calculating real-time FPS and frame DeltaTime.

---

## 💻 Target Hardware & Compatibility

* **Test Machine:** Samsung NP550XDA
* **CPU:** Intel® Core™ i3-1115G4 (11th Gen)
* **GPU:** Intel® UHD Graphics (DirectX 12 Feature Level 11_0+)
* **OS:** Windows 11 Home 24H2
* **Arch:** `x86_64`

---

## 🛠️ Toolchain & Environment

* **Compiler & Build Tools:** Clang / LLVM / Make (`build.bat`)
* **Graphics API:** DirectX 12 (D3D12) / DXGI 1.6
* **Host OS:** Windows 11 Home 24H2
* **Editor:** Visual Studio Code
* **Version Control:** Git & GitHub Desktop & GitHub.com
* **ENTRY:** Discord Server. Name of Server: Devs Studio
* **Server-Discord:** https://discord.gg/88hUjybuY5
* **Limit-Collaborators-In-Server:** 5-10 Collaborators

---

## Critic Files

### What is files?
  * **README: The README.md, is permitted modify this.**
  * **The main: The main.cpp, modify this NO resolving a problem is canceled the Pull Request.**
  * **Resources Table: The resource.rc, is much critic, is permitted modify if modify the main.cpp.**
  * **Build: build.bat Is much critic, NOT permissions of modify.**
  * **Make: The Makefile is small critic, all permissions of modify. But, NOT remove this file.**
  * **Git Ignore: The .gitignore is much critic, controlling what File is ignored for Git/Github. NOT Permissions.**
  * **Notes: In .gitignore or build.bat, I´m have ALL PERMISSIONS of modify.**

---

## 🚀 Getting Started

### Prerequisites

* Windows 10/11 64-bit OS
* Clang Compiler / Make / Windows SDK (for DirectX 12 headers and `d3dcompiler.lib`)
* GPU supporting DirectX 12 Feature Level 11_0 or higher

### Building & Running

```bash
# Clone the repository
git clone https://github.com/dev12124/QMX.git
cd QMX

# Git workflow examples
git branch feature/new-resource
git checkout feature/new-resource
git commit -m "feat: add index buffer rendering"
git request-pull

# To compile and link using Make and build.bat
make