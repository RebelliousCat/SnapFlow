# RBC SnapFlow

**Contextual alignment tool for Blender 4.2.** Select 1, 2, or 3 vertices to snap, flip, or match objects instantly.

It aligns the objects based on the selection of vertices. No more manual gizmo fiddling, just select, click, and snap.

---

## Key Features

### 1. Single Object Alignment (World Axis)
Select vertices on a mesh in **Edit Mode** to perform context-aware snapping:

* **1 Vertex**: Click "Snap to Ground" to set the object's Z-height so that vertex sits exactly at Z=0.
* **2 Vertices (Edge)**: 
    * **First Click**: Aligns the selected edge perfectly to the chosen world axis (X, Y, or Z).
    * **Following Clicks**: Rotates the object **+90°** around that axis. This allows you to cycle through all 4 orientations while keeping the edge aligned.
* **3 Vertices (Face)**:
    * **First Click**: Aligns the face normal to the world axis.
    * **Following Clicks**: Performs a **180° Flip** (useful for ceiling/floor or front/back toggles).



### 2. Multi-Object Match (3-Point Snap)
Align any number of meshes to a target object by matching geometry:

1.  Select multiple objects (the **Active** one is the target).
2.  In **Edit Mode**, select **3 vertices** on each object.
3.  Click the alignment button.
4.  The non-active objects will move and rotate to match their 3 points to the active object's 3 points exactly.



---

## Installation

1.  In Blender, go to `Edit > Preferences > Add-ons`.
2.  Click `Install...` and select the script file.
3.  Find the panel in the **3D View Sidebar (N)** under the **SnapFlow** tab.
