# Unity-Git-Template
A github template for unity

In git, or any version control system for that matter, you only want to maintain the "Assets" and "Project Settings" folders in the repository (repo). For git, to do that, add the following text in .gitignore

------------ start copy -------------
# =============== #
# Unity generated #
# =============== #
Temp/
Obj/
UnityGenerated/
Library/
Build/
------------ end copy ---------------

Next, in the Unity editor...
Goto Edit -> Project Settings -> Editor.
In the Inspector window
- under "Version Control: Mode" choose "Visible Meta Files"
- under "Asset Serialization: Mode" choose "Force Text"

After cloning the repo, open up any Unity scene file and Unity will setup up the rest of the meta and working files automatically.

Remember to check that you are publishing to the correct platform on File -> Build Settings, as this setting sometimes reset.
