# micro:bit MOVE Motor Rotation Counting

A MakeCode extension prototype for estimating wheel rotations on a motorized micro:bit project from elapsed time and an assumed motor speed.

## Blocks

- `start motor with speed`: resets the counter, records the start time, and calls the motor-control helper.
- `get wheel rotations`: estimates completed rotations from elapsed time and RPM.

## Install in MakeCode

1. Open <https://makecode.microbit.org/>.
2. Create a project and choose **Extensions**.
3. Paste `https://github.com/wcchun1234/microbit-move-motor-rotation-counting` into the search box.
4. Select the extension.

## Prototype status

This repository is an instructional scaffold. `moveMotor()` is not implemented and `calculateRPM()` currently returns a fixed 120 RPM. The speed argument is therefore not yet connected to hardware or the estimate. Calibrate the RPM for your motor, wheel, voltage, load, and surface before using the result.

For accurate physical measurement, prefer a wheel encoder or other sensor over time-based estimation.

## Development

The extension metadata is in `pxt.json` and the blocks are implemented in `main.ts`. Use Microsoft MakeCode for micro:bit to test changes on hardware.
