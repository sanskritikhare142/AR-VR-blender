# AR-VR-blender
Capturing the motion of face and imitating it using a character on Blender.

# Procedure
1. Download Blender version 2.83
2. Download and import vincent character 3D model from blenderstudio.org in the blender project
3. Download the .yaml file to run the pre-trained model to capture the motion of the face
4. Import the Christmas tree 3D model (.stl file) and create a new material for it. Provide the colour to the material with a proper hex code.
5. Now go to the modelling tab on the navbar, select the edit mode and insert a cylinder object.
6. Using the scaling and moving option from the left pane, scale the cylinder and place it under the Christmas tree to depict its trunk.
7. Now create a new material for the cylinder and choose the appropriate colour for the material.
8. Group the Christmas tree and the trunk object to make it as a single object.
9. Now, for the vincent character, select a polygon/object for which you want to change the colour from the right pane and click on the material and write the hex code of the new colour.
10. Now zoom in and use the extrude option in the modelling tab and edit abject mode to create pimples on Vincent’s cheeks and chin.
11. Go to the Scripting tab in the top navbar, create a new file OpenCVAnim.py and write the code to create a Panel in the Object properties window. Save the file in the same directory.
12. Now create another new file and write the code to start video capture using OpenCV, process the image frames using .yaml model. Ensure that you give the correct path for the yaml file. Use haarcascade_frontal_face to detect the face using openCV. Using numpy array, define the coordinates of the face of vincent. Check the register button. Save the file in same directory OpenCVAnimOperator.py.
13. Now, go to Layout tab and start capturing the video using OpenCV capture option.
