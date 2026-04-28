# PhoneGesture AI

This project uses smartphone accelerometer data and Edge Impulse to classify three simple gestures: idle, shake and tilt. The aim is to demonstrate an edge AI workflow using a mobile device as the sensing platform and WebAssembly/Node.js as the local deployment environment.

## Workflow

1. Smartphone accelerometer data was collected using Edge Impulse.
2. Three labels were used: idle, shake and tilt.
3. Spectral features were generated from 2-second accelerometer windows.
4. A small neural network classifier was trained in Edge Impulse.
5. The model was evaluated using validation, model testing and live classification.
6. The trained model was exported as a WebAssembly/Node.js deployment.

## Dataset

- Sensor: smartphone accelerometer
- Frequency: 62.5 Hz
- Sample length: 2000 ms
- Classes: idle, shake, tilt

## Results

After refining the tilt gesture to a consistent backward movement, the final model achieved 100% accuracy on validation and model testing. Live classification also correctly identified example idle, shake and tilt gestures.
