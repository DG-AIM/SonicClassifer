
<h1 align="center">SonicClassifier - AI-Powered Music Classification</h1>

<p align="center">
  <img src="./assets/logo.jpeg" alt="sonicclassifier-logo" width="120px" height="120px"/>
  <br>
  <em>SonicClassifier distinguishes between human & AI-generated music with precision, offering real-time classification through an easy-to-use API.</em>
  <br>
</p>

## Disclaimer

Please be informed that SonicClassifier is currently a conceptual project. The information provided in this README outlines the intended plan and design for the project. As of now, the project is in the ideation phase and has not been implemented. It serves as a blueprint, laying down the foundational ideas and prospective features of what SonicClassifier aims to achieve upon realization.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Architecture](#Architecture)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Installation

The SonicClassifier will be accessible via an API and as a Python package. 

### API:
- The API will be hosted and accessible online, allowing easy integration for various applications including the Firefox plugin.
- Detailed API documentation will be provided for seamless usage and integration.

### Python Package:
- The package will be installable via pip, ensuring easy setup.
    ```bash
    pip install sonicclassifier
    ```
    
*Detailed installation instructions and resources will be provided as the development progresses.*


## Usage

SonicClassifier can be utilized through an intuitive API or directly via a Python package, offering flexibility for various use cases.

### Using the API:
Interact with the API through HTTP requests. Here is an example using `curl` to classify an audio file:

```bash
curl -X POST -H "Content-Type: audio/mpeg" --data-binary "@audiofile.mp3" http://api.sonicclassifier.com/classify
```
Replace `"audiofile.mp3"` with the path to your audio file. The API will return a JSON response with the classification results.

### Using the Python Package:
Import the `sonicclassifier` package and use its functions directly in your Python scripts. Here’s a basic example:

```python
import sonicclassifier

# Initialize the classifier
classifier = sonicclassifier.Classifier()

# Classify an audio file
result = classifier.classify('path/to/audiofile.mp3')

# Print the classification result
print(result)
```
Replace `'path/to/audiofile.mp3'` with the actual path to your audio file.

*More detailed examples and documentation will be provided upon the completion of the development phase.*



## API Documentation

Our API is designed to be robust and user-friendly, offering seamless interaction for audio file classification. At this stage of development, we are finalizing the specific endpoints, parameters, and expected responses to ensure optimal performance and usability.

### Preliminary Endpoints (Subject to Change):

- **Endpoint 1:** This endpoint will handle the submission of audio files and return initial classification results. Detailed descriptions and usage instructions are under development.

- **Endpoint 2:** Aimed at providing additional data and analytics, offering insights into the classification process.

### Documentation and Updates:

Comprehensive API documentation, including in-depth details of endpoints, parameters, request/response examples, error codes, and best practices for integration, will be made available as we approach the completion of the development phase. We are committed to ensuring that our documentation will be thorough and user-friendly to cater to developers of varying expertise levels.

### Stay Tuned:

We encourage potential users and contributors to stay tuned for upcoming updates. Your feedback during the testing phase will be invaluable in enhancing the functionality and usability of the SonicClassifier API.


## Architecture

Below is the architectural diagram that illustrates how the SonicClassifier API server interacts with the Firefox add-on to provide real-time audio file classification.

<p align="center">
  <img src="./assets/system-diagram.png" alt="System Diagram" width="600"/>
</p>

### Description

The diagram showcases the workflow between the SonicClassifier API server and the Firefox add-on. Users can utilize the add-on to send audio files to the API server for classification. The server processes and classifies the audio files, returning the results directly to the add-on in the user’s browser.

### Workflow

1. **User Interaction:** Users send audio files through the Firefox add-on.
2. **API Server:** The add-on communicates with the SonicClassifier API server, sending the audio files for classification.
3. **Processing:** The API server classifies the audio files distinguishing between human & AI-generated music.
4. **Response:** Classification results are sent back to the Firefox add-on and displayed to the user.

For a more detailed explanation of each component and their interactions, refer to the [Documentation](#documentation).



## Contributing

We warmly welcome contributions to the SonicClassifier project. Whether it's bug reports, code improvements, or new feature proposals, each contribution is appreciated, aiding in enhancing the effectiveness and usability of SonicClassifier.

### Contribution Steps:

1. **Fork the Repository:** Start by forking the SonicClassifier repository to your own GitHub account.

2. **Create a Feature Branch:** Create a new branch in your forked repository where you’ll work on your feature or bug fix.

3. **Commit Your Changes:** Make your changes and commit them to your feature branch.

4. **Push to Your Fork:** Push your changes to your forked repository on GitHub.

5. **Submit a Pull Request:** Go to the SonicClassifier repository and submit a pull request, ensuring to provide a comprehensive description of the changes.

### Reporting Bugs or Suggesting Features:

- **Bugs:** Report bugs via the issue tracker, providing detailed information to help us understand and address the issue effectively.

- **Feature Proposals:** We’re always eager to enhance SonicClassifier; suggest new features through the issue tracker, explaining the feature and its benefits.

Your contributions are invaluable and we're committed to reviewing and integrating them in a timely manner!

## License

SonicClassifier is licensed under the GNU General Public License. This ensures that it remains free and open-source, promoting software freedom and protection against proprietary restrictions. For detailed terms and conditions, please refer to the [GNU GENERAL PUBLIC LICENSE](LICENSE) file in the repository.

