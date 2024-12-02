# React Native Llama

<p align="center">
  <img src="./assets/images/rnllama.png" width="200" alt="rnllama Logo">
</p>

A React Native mobile application for running LLaMA language models using ExecuTorch. This example is for iOS only for now.

## Features

- Run LLaMA models directly on device, build the UI using React Native
- Tested using Llama 3.2 SpinQuant 1B on iPhone 12 Pro


## Prerequisites

- Node.js & npm
- Xcode

## Installation

1. Clone the repository: `git clone git@github.com:pytorch/executorch.git`

2. Navigate to the root of the repository: `cd executorch`

3. Install dependencies: `./install_requirements.sh --pybind xnnpack && ./examples/models/llama/install_requirements.sh`

4. Follow the instructions in the [README](https://github.com/pytorch/executorch/blob/main/examples/models/llama/README.md#option-a-download-and-export-llama32-1b3b-model) to export a model as `.pte`

6. Navigate to the example: `cd examples/demo-apps/react-native/rnllama`

7. Install dependencies: `npm install`

8. Run the app: `npx expo run:ios --device` and select a USB connected iOS device

9. Find the device in finder, and place the exported `.pte` model and the downloaded tokenizer under the app.

10. Select the model and tokenizer in the app to start chatting:

![Select model](./assets/images/select_model.png)

