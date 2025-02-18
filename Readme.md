# Wild Animal Detection Using AI

This project is a wild animal detection system using YOLO-V8, a state-of-the-art object detection model. The system is designed to detect various wild animals in real-time using a webcam feed and send the detection results to a remote server.

## Features

- Real-time wild animal detection using YOLO-V8.
- Live video feed from the webcam.
- Detection results are sent to a remote server.
- Web interface for viewing the live feed and detection results.

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/wildlife-detection-system.git
    cd wildlife-detection-system
    ```

2. Install Anaconda:
    Follow the instructions [here](https://www.digitalocean.com/community/tutorials/how-to-install-the-anaconda-python-distribution-on-ubuntu-22-04) to install Anaconda.

3. Update your PATH:
    ```sh
    export PATH=~/anaconda3/bin:$PATH
    ```

4. Create and activate a new conda environment:
    ```sh
    conda create -n wild python==3.9
    conda init
    # Reboot your terminal or system if necessary
    conda activate wild
    ```

5. Install the required packages:
    ```sh
    python3 -m pip install django
    pip install ultralytics
    ```

6. Apply the migrations:
    ```sh
    python3 manage.py migrate
    ```

7. Update your system and install necessary libraries:
    ```sh
    sudo apt update
    sudo apt install libgl1-mesa-glx
    ```

8. Update ALLOWED_HOSTS in settings.py:
    ```python
    ALLOWED_HOSTS = ['your_public_ipv4_address']
    ```

9. Run the development server:
    ```sh
    python3 manage.py runserver 0.0.0.0:8000
    ```

10. Edit inbound rules to add port 8000 for anywhere IPv4.

11. Open your web browser and go to [http://your_public_ipv4_address:8000/](http://your_public_ipv4_address:8000/) to view the application.

## Usage

- Navigate to the home page to start the webcam feed.
- The system will detect wild animals in real-time and display the results on the screen.
- Detection results are sent to a remote server for further processing.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](http://_vscodecontentref_/20) file for details.

## Acknowledgements

- [YOLO-V8](https://github.com/ultralytics/yolov8) for the object detection model
- [Django](https://www.djangoproject.com/) for the web framework
- [OpenCV](https://opencv.org/) for the computer vision library


