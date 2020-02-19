# Blender-vertex-raymarch
A simple blender script written for 2.79 for manually generating point clouds from SDFs


This python script searches the scene for two objects, one labeled "Camera" and one labeled "Mesh". The way I used it is I hit '0' on the keypad to get to camera view, shift+f to take control of the camera, select the target mesh object (with or without existing vertices), and simply execute the scipt with alt+p while hovering over the text editor. Based on the target cameras orientation, several rays are generated and marched along with a distance estimator. Upon reaching a certain distance (epsilon) to the surface, a vertex is created and added to the mesh. The density of vertices, and distribution is controlled by where you place and orient the camera, so you should expect to approach it like taking images for photogrammetry, taking pictures of interesting features, and getting as much of the topology mapped as possible.

Various parameters to play around with are the number of x and y scans, the distance estimator, the epsilon value, etc. Its not a perfect script, but the results can be quite intriguing.
