# Application Usage Tutorial Generation using AI

This project aims to help users create custom tutorials for mobile applications.

## How it works

1. The user inputs a video screen recording of them using a certain application. eg. Using the VITian App to check exam schedule.
2. The project uses video_formatting.ipynb to add black bars to the sides of the video to reformat it to a desired aspect ratio.
3. The user then inputs a step by step proces of the actions taken in the video. eg. "Tap on Academics", "Select Timetable", etc.
4. The project will then prompt the user to mention timestamps for each of these steps. eg."Tap on Academincs" -> 1:21
5. The project uses an LLM to alter the steps given by the user into better narrator text. eg."Tap on Academics" -> "Open the academics section"
6. Similarly, we also generate text to appear on screen as text boxes for the user.
7. The narrator text is converted into voice audio using a text-to-voice model of choice.
8. The text boxes and the narrator audio are added into the video.
