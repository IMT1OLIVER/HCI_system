# HCI_system
Jasne, w takim razie zmodyfikujmy tekst tak, aby jeszcze wyraźniej podkreślić, że to był Twój samodzielny projekt (Independent Project), zachowując przy tym profesjonalny, inżynierski styl.

Oto zaktualizowana wersja README na GitHub:

As the sole developer and author of this project, I engineered an innovative Human-Computer Interface (HCI) that redefines operating system interaction by eliminating the need for manual input. My primary objective was to independently design a solution that assists individuals with motor impairments or enhances ergonomic efficiency in specialized technical environments. The system relies on advanced real-time image analysis to precisely map head movements to mouse cursor coordinates.

The software architecture was built from the ground up using the OpenCV library, which I utilized to implement object detection algorithms and process live video streams. A key engineering feat of my work is the integration of Haar Cascade classifiers for face detection, combined with custom image segmentation methods to recognize specific objects that trigger click actions. By introducing a "neutral zone" and optimizing the movement step (move_step), I successfully minimized noise and jitter, ensuring smooth and reliable control.

For the operating system integration layer, I chose the pynput library to provide low-level control over input devices. I was responsible for synchronizing the vision module with the control module to ensure minimal latency, which is critical for real-time systems. The program dynamically interprets the position of the face relative to the frame's center; the detection of a predefined object (such as a smartphone) immediately generates a system interrupt corresponding to a left mouse click.

During the validation phase, I independently conducted a series of performance and training tests that significantly improved the system's effectiveness. I optimized the detection parameters myself, which resulted in an increase in gesture recognition precision from initial low values to approximately 90% after user training. The technical documentation includes detailed confusion matrices and analysis of metrics such as sensitivity and accuracy, confirming the engineering rigor of my research.

While the system achieves full functionality as intended, I view this solution as a foundation for further development toward more complex gestures and multi-monitor support. In future iterations, I plan to replace classic Haar Cascades with Deep Learning models to increase the system's robustness against varying lighting conditions. This project serves as proof that through individual effort and accessible Python libraries, one can create a powerful assistive tool that significantly enhances digital accessibility.
