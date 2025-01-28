### Convert Robot Model to Xacro Model in Blender with Phobos Plugin

1. **Import Model**:
   - Import the robot model from CAD software (preferred format: `.obj`).
   - Separate the model into individual meshes:
     - Select all (`A`), go to the "Modelling" tab, right-click, choose **Separate > By Loose Parts**.
   - Adjust the robot's origin to the trunk base.
   - Orient the robot: front faces the positive X-axis, left side faces the positive Y-axis.
   - Apply rotation to the entire robot:
     - Select all (`A`), go to the **Object** menu, select **Apply > Rotation**.
   - Remove unnecessary parts (e.g., internal trunk components, screws).
   - Group parts into their respective links:
     - Select the desired parts, right-click, and choose **Join**. Refer to the example for correct grouping.

2. **Phobos Setup**:
   - Set the Phobos type for each mesh part to **"Visual"** in the Phobos menu.
   - Create links:
     - Select the trunk, then click **Create New Link** in the Phobos menu. A bone will appear.
     - **Note**: Do not move or rotate the link during creation. Adjustments can be made after defining the joint.
   - Parent meshes to joints:
     - Select the mesh (child) and the bone (parent), then press `Ctrl+P` and choose **Bone Relative**.
     - Follow the hierarchical tree structure: trunk (base) has five children (right arm, left arm, right leg, left leg, head). Parent links accordingly.

3. **Finalize Skeleton**:
   - After completing the skeleton, proceed to define **collision** and **inertial** properties.

For additional guidance, refer to the provided YouTube tutorial.
