# Specialized Technology, Fundamental Concepts 

## Specialized Technology
Computer Vision

## Concepts
This project will apply computer vision to the faces in a photograph to detect the location of each face in the image and facial landmarks will be detected. The percentage of faces that pass all three checks then gives the photograph its score and category.It also ranks and displays the final shortlisting photo.

For example, the photogaphe upload large number of photo and the sytem will calculate the score and categorise them (Good ≥ 90%, Fair 70–89%, Poor < 70%) and shotlisted the best photo.

## Frameworks, models, methods and tools 
- Face detector (MTCNN, RetinaFace or MediaPipe): finds each face in the photograph and returns a box around it, so every later check is done face by face.
- Facial landmark detection: marks key points on each face, such as the corners of the eyes and the lips, to measure the state of a facial feature.
- Eye Aspect Ratio (EAR): compares the height of an eye with its width, using the landmark points, to decide whether the eye is open or closed.
- Head pose estimation: works out the direction the head is turned from the landmarks, to check whether the person is facing the camera.
- OpenCV (Python): loads, resizes and prepares the photographs, and links the steps together.

## How it fits the problem: 
The system checks the same face conditions a photographer checks by eye (eyes open, mouth in a proper state), and applies the same rules to every photograph.

## Benefits:
- It saves time on the repetitive face checks.
- It gives consistent results, which matters because fatigue weakens decisions.
- Each failing face is marked with a reason, and the photographer keeps the final choice.

## Limitations:
- Accuracy may fall with glasses, hair over the eyes, side views, small faces and poor lighting.
- Fixed thresholds may not suit every face, for example a smile with teeth read as an open mouth.
- Photographs contain faces, which are personal data, so keep processing on the user’s device and get permission for test photographs.

## Alternative and choice: 
A trained CNN eye-state classifier can handle unusual faces better but needs a large labelled dataset and is harder to explain. I would choose the landmark-based approach because it needs no training data, is easy to explain, and fits a student project timeline.

## Resources
- Asperti, A., & Filippini, D. (2023). Deep learning for head pose estimation: A survey. SN Computer Science, 4(4), Article 349. https://doi.org/10.1007/s42979-023-01796-z
- Chen, J., Wang, M., & Hsia, C.-H. (2025). Artificial intelligence and machine learning in sensing and image processing. Sensors, 25(6), Article 1870. https://doi.org/10.3390/s25061870
- Dewi, C., Chen, R.-C., Jiang, X., & Yu, H. (2022). Adjusting eye aspect ratio for strong eye blink detection based on facial landmarks. PeerJ Computer Science, 8, Article e943. https://doi.org/10.7717/peerj-cs.943
- Khabarlak, K., & Koriashkina, L. (2022). Fast facial landmark detection and applications: A survey. Journal of Computer Science & Technology, 22(1), Article e02. https://doi.org/10.24215/16666038.22.e02
- Li, Y., Lee, H. H. M., & Blasco-Arcas, L. (2025). Computer vision in branding: A conceptual framework and future research agenda. Journal of Business Research, Article 115329. https://doi.org/10.1016/j.jbusres.2025.115329