# Sign language

This repository contains code for hand sign detection using the OpenCV and MediaPipe libraries. The program captures video from the webcam and detects various hand gestures in real-time.

## Requirements

- OpenCV
- MediaPipe

## Functionality

The program performs the following tasks:

1. Initializes the necessary libraries and captures video from the webcam.
2. Processes each frame and detects hand landmarks using the MediaPipe library.
3. Determines the status of each finger (folded or unfolded) based on the detected landmarks.
4. Prints the status of each finger and performs the corresponding action for specific gestures:
   - "STOP" gesture: If the thumb, index, middle, ring, and little fingers are folded and the palm is facing downwards, it prints "STOP" on the screen.
   - "FORWARD" gesture: If the thumb is unfolded and pointing forward while the other fingers are folded, it prints "FORWARD" on the screen.
   - "BACKWARD" gesture: If the thumb is unfolded and pointing backward while the other fingers are folded, it prints "BACKWARD" on the screen.
   - "LEFT" gesture: If the thumb is folded and the index, middle, ring, and little fingers are unfolded, and the hand is tilted to the left, it prints "LEFT" on the screen.
   - "RIGHT" gesture: If the thumb is folded and the index, middle, ring, and little fingers are unfolded, and the hand is tilted to the right, it prints "RIGHT" on the screen.
   - "LIKE" gesture: If all fingers are folded and the thumb is positioned higher than the other fingers, it prints "LIKE" on the screen.
   - "DISLIKE" gesture: If all fingers are folded and the thumb is positioned lower than the other fingers, it prints "DISLIKE" on the screen.

5. Draws the detected hand landmarks and connections on the video frame.
6. Displays the processed video with the detected hand gestures.

## License

The code in this repository is licensed under the [MIT License](LICENSE).

Feel free to modify and use the code according to your needs.
