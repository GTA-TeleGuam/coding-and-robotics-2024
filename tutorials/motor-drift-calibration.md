```package
microbit_robot=github:microsoft/microbit-robot
```

# Robot Calibration

## Robot Calibrate block
- Registers button A, B, A+B to change the radio group and drift.
- Puts motors to 80%.

Bias towards the button pressed during calibration (top down view).
A = bias towards right (--)
B = bias towards left (++)

```blocks
robot.elecfreaksCuteBot.start()
// @highlight
robot.calibrate()
```

## Calibrate motor drift until straight
Calibrate motor drift until straight

## Enter drift value
Use drift value from `||robot:robot calibrate||` and input into `||robot:robot set motor drift||`

```blocks
robot.elecfreaksCuteBot.start()
// @highlight
robot.setMotorDrift(-3)
```