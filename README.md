# Application Usage Tutorial Generation using AI

This project aims to help users create custom tutorials for mobile applications.

## How it works

1. The user inputs a video screen recording of them using a certain application. eg. Using the VITian App to check the exam schedule.
2. We separate the audio from the video and store it separately to be transcribed.
3. The project uses video_formatting.ipynb to add black bars to the sides of the video to reformat it to a desired aspect ratio.
4. The user then inputs a step-by-step process of the actions taken in the video. This can be acquired by transcribing the audio. eg. "Tap on Academics", "Select Timetable", etc.
5. The project will then acquire timestamps of each step based on the transcribed text timings. eg. "Tap on Academics": 4.9
6. The project uses an LLM to alter the steps given by the user into better narrator text. eg."Tap on Academics" -> "Open the academics section"
7. We also print out step text onto the video using the timestamps.
8. The narrator text is converted into voice audio using a text-to-voice model of choice.
9. The text boxes and the narrator audio are added into the video.

## Here is an example of a generated video

https://github.com/Anand-G-Murugan/Task-Tutorial-Generation/assets/87412613/c9e17c9d-2e85-4722-bb72-0443c7e8cee5

