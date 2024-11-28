Although there are tools available for batch renaming and symmetrizing rigs, 
there doesn't seem to be a tool that automatically creates separate DEFORM and DRIVER bones.
Tool brief:

1. Detect Identical Bones:
  * Identify bones that occupy identical positions within the armature.
2. Modify One Set of Bones:
  * For one set of these identical bones:
    * Deselect the DEFORM property to prevent them from deforming the mesh.
    * Rename these bones to indicate they are DRIVER bones.
3. Apply Constraints:
  * For each bone in the selection:
    * Add a constraint that causes it to follow or be driven by its corresponding identical bone.
4. Finalization:
  * The setup is now complete with separate DEFORM and DRIVER bones.

This method effectively creates a set of driver bones that control the deform bones without directly affecting the mesh.

