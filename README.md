

<h1 align="center">SonicClassifier - AI-Powered Music Classification</h1>

<p align="center">
  <img src="./assets/logo.jpeg" alt="sonicclassifier-logo" width="120px" height="120px"/>
  <br>
  <em>SonicClassifier distinguishes between human & AI-generated music with precision, offering real-time classification through an easy-to-use API.</em>
  <br>
</p>

## Disclaimer

_Please be informed that SonicClassifier is currently a conceptual project. The information provided in this README outlines the intended plan and design for the project. As of now, the project is in the ideation phase and has not been implemented. It serves as a blueprint, laying down the foundational ideas and prospective features of what SonicClassifier aims to achieve upon realization. Details and specifications might evolve as development begins, aligning with technical, functional, and user experience optimizations._

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
Interact with the API through HTTP requests. Here is a sample way for using `curl` to classify an audio file:

```bash
curl -X POST -H "Content-Type: audio/mpeg" --data-binary "@audiofile.mp3" http://api.sonicclassifier.com/classify
```
The API will return a JSON response with the classification results.

### Using the Python Package:
Import the `sonicclassifier` package and use its functions directly in your Python scripts. Here’s a basic example:

```python
import sonicclassifier

# Initialize the classifier
classifier = sonicclassifier.Classifier()

# Classify an audio file
result = classifier.classify('path/to/audiofile.mp3')
# OR Classify a Midi file
result = classifier.classify_midi('path/to/midifile.mid')

# Print the classification result
print(result)
```
Replace `'path/to/audiofile.mp3'` or `'path/to/midifile.mid'` with the actual path to your audio file or the midi file.

*More examples and documentation will be provided upon the completion of the development phase.*



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

The architectural diagram below illustrates how the SonicClassifier API server interacts with different entities to identify AI-generated music.

<p align="center">
  <img src="./assets/Systems Diagram SonicClassifier.png" alt="System Diagram" width="600"/>
</p>

### Description

The diagram showcases the workflow between the SonicClassifier API server and different entities. Users can utilize the API to send audio files to the API server for classification. The server processes and passes the file onto the appropriate AI model. The AI model returning the result to the API server which in turn returns the result as an HTTP response.

### Workflow

1. **User Interaction:** Users or application server send audio files through API.
2. **API Server:** The add-on communicates with the SonicClassifier API server, sending the audio files for classification.
3. **Processing:** The API server classifies the audio files distinguishing between human & AI-generated.
4. **Response:** Classification results are sent back to the requester.

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
