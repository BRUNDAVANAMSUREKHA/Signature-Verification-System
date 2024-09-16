# Signature Matching System

This is a Python-based Signature Matching System that uses **Tkinter** for the graphical user interface (GUI), **OpenCV** for image capturing and processing, and **SSIM** (Structural Similarity Index) from the `skimage` library for comparing the similarity between two signature images. The system allows users to either capture signatures through a webcam or browse and select existing image files, and it determines the similarity percentage between two signatures.

## Features

- **Capture Signatures**: Capture two signatures using your webcam.
- **Browse Signatures**: Browse and load signature images from your file system.
- **Compare Signatures**: Calculates similarity between two signatures using SSIM.
- **Feedback**: Notifies whether the signatures match or not based on a predefined threshold (85%).

## Technologies Used

- **Python**: Programming language.
- **Tkinter**: For creating the GUI.
- **OpenCV**: For image capturing and processing.
- **skimage**: For the SSIM (Structural Similarity Index) algorithm to compare images.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/signature-matching.git
    cd signature-matching
    ```

2. **Install dependencies**:
    You need to install the following libraries to run this project:
    
    ```bash
    pip install opencv-python-headless
    pip install numpy
    pip install scikit-image
    ```

3. **Run the application**:
    ```bash
    python main.py
    ```

## How It Works

1. **Capture Image**: 
    - Click on the `Capture` button to capture a signature image through the webcam. The image will be stored in a temporary folder (`./temp`) for later comparison.

2. **Browse Image**: 
    - Alternatively, you can click the `Browse` button to select an existing signature image from your file system.

3. **Compare Signatures**:
    - Once both images are loaded (either by capturing or browsing), click the `Compare` button to check the similarity between the two signatures.
    - The application uses the SSIM algorithm to compute the similarity percentage.
    - If the similarity is above the threshold of 85%, a success message is displayed, indicating that the signatures match.
    - If the similarity is below 85%, a failure message is shown, indicating that the signatures do not match.

## Outcome

![image](https://github.com/user-attachments/assets/5691a17d-c946-46cd-af52-7125ebf07f1e)
![image](https://github.com/user-attachments/assets/926c24f6-233e-4fee-b457-f5045e11adef)
![image](https://github.com/user-attachments/assets/6ec9ef28-ca42-4d8b-b1e5-2bd43d228ce5)
![image](https://github.com/user-attachments/assets/096e504c-9117-4d88-8c95-e3f697b9c617)
![image](https://github.com/user-attachments/assets/c660eb46-7674-4584-a72d-a4d24b48aa18)

## Future Enhancements
1. **Contour Detection**: Enhance the accuracy of signature matching by incorporating contour detection.
2. **Support More Formats**: Extend support to additional image formats (e.g., TIFF, BMP).
3. **Data Storage**: Log comparison results in a database or file for future reference.
   
## License
This project is licensed under the MIT License.

This should be ready to use and easily copied. Let me know if you need any adjustments!
