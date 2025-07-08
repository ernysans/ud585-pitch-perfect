# ud585-pitch-perfect
Intro to iOS App Development with Swift Project


|     |     |
| --- | --- |
| ![](https://lh7-rt.googleusercontent.com/u/0/docsd/ANYlcfAk4AxtE1UjECUwVgbd0xZ6mwORvjDXUVj6YrhtHiQZJ0-75SRcJEmC3ObRR-OWsOV0rXr7VBAO-8nTgsM5I-uFcYzqOe4Fvy2Lmi401bXWdVCZS_x7GK91XR-EhsgH4W3qUpBojlh2TyP1Yy8xfE5Ht4zVTQdah8gNQmM8ZhsZetQQNiqyjHunzSZH8rcBbVfOJKKUUlLM-v1tYm20CQYywCsZWSrZcoOH-qZnkzFDgkv4DqFPCh5cj7tQtwIP6BTrPtyDfbHZeWBFDYSuMY8-nroZiod6LZhtp-ug4ADFTkWj9i1LKu5TtM--FP6cbUFIIqY0vJIhqPvDA640RYA0gblEPPm1ApBAobiR0kYLkewVY0_mKuqMt4G2JLJ5hOt2VH7t0d6GPCX5FxZVBxxc30etT5POumG_hkDVj7EhaHnP9rMyP2_mQ5qH7LI4SPAewESlP40QSliYlSmcUcPF0pj4cbyPyASGmwIR-SRnal-bxDnNaArngfNLpxP4j3VtA5K5mNgRM_T5fzPjhgdyJAV5AkukPorZtt50a569N6JKlOquE4WGd5NSthHlANNUg0B7w1dsBXAX5YGhR3zxZTB4IAOsgl2VbYkyl5y9-KngNsuxgTdTZ4noueUmYX3s0nD_WJnd4duV-OSdqkJso0pd0gKCqYusrhJj_yuTb4s8pnq19wFK8rSCyosTQOhYJ8Wp7ya_jQDUUFV0blnWqjyyorvkd38Gvhhori9jhRWhyHc0RLTLjDYpQ-1Iqi0_Gyb_WZjnV3268lpdfzpxX8T4z_jmKRrHA8GMU7BO0oZspZ3M9QsH1KkOc4AGV-DIpFQK0DtDfvuwbeVHEoNfzmZlhqSXfYxP5f93kpj95nNShXwSNOM3j8pJ4R5isBgtuEz7kySoaF4rLRXL) | Project 1: Pitch Perfect<br><br>iOS Developer Nanodegree |

|     |     |
| --- | --- |
| Criteria | Meets Specifications |
| # Basic Functionality |     |
| The app contains two scenes of content: one for recording an audio file, and one for playing the audio with different effects. | The app contains two pages of content (one each for recording and playing audio), and uses UINavigationController to navigate between these two scenes. |
| All UI elements (buttons and text) are appropriately formatted for iPhone and iPad Portrait and Landscape layouts. | UI elements are appropriately positioned on the screen for iPhone and iPad portrait and landscape layouts. |
| # Actions and Outlets |     |
| The app uses IBAction methods to record audio and playback sounds. | The app connects each button on the Storyboard to the correct IBAction method. |
| Labels and buttons are shown or hidden as appropriate. | In the first scene, the Recording label and the Stop button are disabled and enabled appropriately:<br><br>When no recording is taking place the Stop button is disabled.<br><br>While recording is taking place the Stop button is enabled and the Record button disabled |
| # AVAudioRecorder |     |
| The first scene of the app uses AVAudioRecorder to record audio. | The app successfully uses AVAudioRecorder to record audio. |
| # Delegates and Segues |     |
| The app uses the audioRecorderDidFinishRecording() method to determine when the audio has finished recording. | The app uses the delegate pattern and implements the audioRecorderDidFinishRecording() method. |
| The app programmatically triggers a segue from the first scene to the second by using the performSegueWithIdentifier() method. | The app does not use a Storyboard segue hardcoded to the Stop button. A segue from the first scene to the second is programmatically triggered via performSegueWithIdentifier(). |
| # UINavigationController |     |
| The app allows users to re-record audio after a recording is complete. | The app allows the user to re-record by navigating back to the first scene from the second. |
| # Sound Effects |     |
| The second scene of the app contains the following audio effects: Snail (slow), Rabbit (fast), Chipmunk (high pitch), Darth Vader (low pitch), Echo and Reverb. | The second scene of the app contains the following buttons for audio effects: Snail (slow), Rabbit (fast), Chipmunk (high pitch), Darth Vader (low pitch), Echo and Reverb. All six buttons work properly to play the associated sounds. |
| # Code Quality |     |
| Code is effectively abstracted. | Potentially repetitive blocks of code  are effectively abstracted into reusable methods. |
| Code adheres to [Swift naming and style conventions](https://www.google.com/url?q=https://github.com/github/swift-style-guide&sa=D&source=editors&ust=1751989763409079&usg=AOvVaw3dHJOAqZZCxBsl5fdrR9Vt). | Code adheres to [Swift naming and style conventions](https://www.google.com/url?q=https://github.com/github/swift-style-guide&sa=D&source=editors&ust=1751989763409393&usg=AOvVaw2xto9G38P9dBhN0LgZq-rq). |
| Code uses appropriate and effective comments. | Code is readable and easy to follow. Any code that may be hard to understand is commented effectively. |

Once you have a functioning app, consider adding more features to make your app stand out! Here are some suggestions:

*   Use UIStackViews for the RecordSoundsViewController view too. You already use UIStackViews in the PlaySoundsViewController, try adding them to the RecordSoundsViewController.
*   Add a UILabel to the audio playback view that shows the duration of the recorded audio. You’ll need to read up on [Apple’s documentation for AVAudioPlayer](https://www.google.com/url?q=https://developer.apple.com/library/ios/documentation/AVFoundation/Reference/AVAudioPlayerClassReference/index.html&sa=D&source=editors&ust=1751989763410828&usg=AOvVaw1ODtWHheXloDkwU15NLfWq) to figure out how to do this.
