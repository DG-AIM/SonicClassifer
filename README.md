<h1 align="center">SonicClassifier - AI-Powered Music Classification</h1>

<p align="center">
  <img src="./assets/logo.jpeg" alt="sonicclassifier-logo" width="120px" height="120px"/>
  <br>
  <em>SonicClassifier distinguishes between human & AI-generated music with precision, offering real-time classification through an easy-to-use API.</em>
  <br>
</p>

<p align="center">
  <a href="https://www.sonicclassifier.com"><strong>www.sonicclassifier.com</strong></a>
  <br>
</p>

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Architecture][£Architecture]
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Installation

Provide a detailed step-by-step process on how to install and set up SonicClassifier. Include any system prerequisites, and the commands to install them, and the SonicClassifier itself.

```bash
# Example: Install via pip
pip install sonicclassifier
```

## Usage

Describe the general usage, examples of commands, or scripts users can run to interact with SonicClassifier. Add code samples and examples to make this section as detailed as necessary.

```python
# Example Python code to interact with the API
import sonicclassifier

# Code continues...
```

## API Documentation

Provide an overview of the API, including the endpoints, parameters, and expected responses. Link to detailed API documentation if available.

- Endpoint 1: Description and usage
- Endpoint 2: Description and usage

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

Information on how others can contribute to SonicClassifier. Include guidelines for submitting pull requests, reporting bugs, or proposing new features.

1. Fork the repo
2. Create your feature branch (```git checkout -b feature/fooBar```)
3. Commit your changes (```git commit -am 'Add some fooBar'```)
4. Push to the branch (```git push origin feature/fooBar```)
5. Create a new Pull Request

## License

Include the license information here. Link to the LICENSE file in the repository.

[MIT License](LICENSE)

## Acknowledgements

Give credit to authors, contributors, or mention any other support you received while working on this project.
