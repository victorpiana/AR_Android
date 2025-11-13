# 🧾 Augmented Reality Project Submission - Victor PIANA

> This repository contains the submission files for the Augmented Reality (AR) practical work (TP). This set of Android APKs showcases various AR capabilities, including marker-based tracking, plane detection, object manipulation, and advanced face tracking with dynamic interactions.

[![Engine](https://img.shields.io/badge/Engine-Unity-gray.svg)](https://unity.com/)
[![Platform](https://img.shields.io/badge/Platform-Android-green.svg)](https://www.android.com/)
[![Framework](https://img.shields.io/badge/Framework-ARFoundation-lightgray.svg)](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@4.2/manual/index.html)
[![Author](https://img.shields.io/badge/Author-Victor_PIANA-blue.svg)](#)

---

## 📦 PROJECT CONTENT & FEATURES

### 1. Part 1 - QR Code (Image Marker Tracking)

* **APK File:** `Partie1 QR CODE Piana Victor.apk`
* **Feature:** Displays a **3D object** triggered by an image marker (**QR code**).

### 2. Part 2 - Plane Detection, Selection, and Interactions

* **APK File:** `Partie 2 TP (Plan) Piana Victor.apk`
* **Core Functionalities:**
    * ▶️ **Plane Detection:** Automatically identifies horizontal surfaces (floors, tables).
    * ▶️ **Object Placement:** Allows placing a 3D object via screen tap.
    * ▶️ **Visual Selection:** Enables selecting the placed object.
    * ▶️ **Interaction:** Supports **rotation**, **scaling**, and **movement** of the object on the detected planes.

### 3. Part 3 - Face Detection

| APK File | Feature Description |
| :--- | :--- |
| **`Visage1 Piana Victor.apk`** | Displays a **3D object** anchored to the detected face. |
| **`Visage2 PianaVictor.apk`** | Integrates a **custom video feed** superimposed on the face. |
| **`Visage3 PianaVictor.apk`** | Displays an **animated XYZ reference frame** (gizmo) fixed to the head. |

---

## 4. Going Further - Combined Dynamic Application

* **APK File:** `PourAllerPlusLoin_Victor_Piana.apk`
* **Overview:** A stable, autonomous application combining face tracking with dynamic state changes based on head movement and user stillness.

### ✨ Dynamic User Experience

#### 1. Startup Instructions Phase

* Two explanatory messages are displayed:
    * *« Turn or tilt your head to change the emoji (up / middle / down) »*
    * *« Stay still to accelerate the star • Move → it slows down • Tilt your head → changes the color »*
* **Timing:** Each message is shown for **2.5 seconds**, then fades out with an **alpha blend effect over 2.5 seconds**.
* **Robustness:** Occurs **once per session**; if the face is lost and rediscovered, the system cleanly restarts this phase.

#### 2. Dynamic Emojis on Face

* No emoji displayed at startup.
* A single emoji is shown based on the **vertical orientation of the head**:
    * **High Tilt** (Looking up) → Red emoji
    * **Neutral Position** → Neutral emoji
    * **Low Tilt** (Looking down) → Yellow emoji
* Emojis remain **hidden** until the instruction phase is complete.

#### 3. Floating and Dynamic Star

* The star appears **above the head** upon instruction completion.
* **Speed/Size:** Its rotation speed and size progressively **increase** if the user remains **still**.
* **Movement Impact:** It automatically **slows down** when the user moves.

#### 4. Adaptive Visual Effects

* The star's **color changes** based on the vertical face tilt:
    * High Head Tilt: **Red**
    * Low Head Tilt: **Yellow**
    * Normal Head Position: **Green**
* The star is accompanied by a **dynamic luminous halo**.

---

## 🚀 How to Test (Android APKs)

All provided APK files are ready to be installed on any Android device.

1.  **Download** the desired `.apk` file(s).
2.  On your Android device, enable **"Install from unknown sources"** in your security settings (if you haven't already).
3.  Open the downloaded `.apk` file to install the application.
4.  Launch the app and grant **camera permissions** to enable the Augmented Reality experience.

---

## ✅ Status

All APK files have been individually tested and confirmed to be fully functional.
