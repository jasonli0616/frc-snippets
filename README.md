# FRC Snippets - VSCode Extension

FRC Snippets is a VSCode extension made for the First Robotics Java library.

![Commands snippet demo](https://raw.githubusercontent.com/jasonli0616/frc-snippets/main/images/FRC%20Snippets%20-%20Command%20demo.png)
![Subsystem snippet demo](https://raw.githubusercontent.com/jasonli0616/frc-snippets/main/images/FRC%20Snippets%20-%20Subsystem%20demo.png)

## Examples

### Insert command boilerplate code

Prefix:

```
frccmd
```

Code snippet:

```java
import edu.wpi.first.wpilibj2.command.CommandBase;

public class ClassName extends CommandBase {

    private final Subsystem m_subsystem;

    public ClassName(Subsystem subsystem) {
        // Use addRequirements() here to declare subsystem dependencies.
        addRequirements(subsystem);
        
    }

    // Called when the command is initially scheduled.
    @Override
    public void initialize() {
        
    }

    // Called every time the scheduler runs while the command is scheduled.
    @Override
    public void execute() {
        
    }

    // Called once the command ends or is interrupted.
    @Override
    public void end(boolean interrupted) {
        
    }

    // Returns true when the command should end.
    @Override
    public boolean isFinished() {
        
        return false;
    }

}
```

### Insert subsystem boilerplate code

Prefix:

```
frcsys
```

Code snippet:

```java
import edu.wpi.first.wpilibj2.command.SubsystemBase;

public class ClassName extends SubsystemBase {

    public ClassName() {
        
    }

    @Override
    public void periodic() {
        // This method will be called once per scheduler run
        
    }

    @Override
    public void simulationPeriodic() {
        // This method will be called once per scheduler run during simulation
        
    }

}
```

### Declare Xbox Controller

Prefix:

```
frcdx
```

Code snippet:

```java
// Controller
private final XboxController sys_controller; // = new XboxController(0);
private final JoystickButton btn_main_A, btn_main_B, btn_main_X, btn_main_Y, btn_main_LBumper, btn_main_RBumper,
    btn_main_LAnalog, btn_main_RAnalog, btn_main_Back, btn_main_Start;
```

### Instantiate Xbox Controller

Prefix:

```
frcix
```

Code snippet:

```java
// Controller
sys_controller = new XboxController(0);
btn_main_A = new JoystickButton(sys_controller, XboxController.Button.kA.value);
btn_main_B = new JoystickButton(sys_controller, XboxController.Button.kB.value);
btn_main_X = new JoystickButton(sys_controller, XboxController.Button.kX.value);
btn_main_Y = new JoystickButton(sys_controller, XboxController.Button.kY.value);
btn_main_LBumper = new JoystickButton(sys_controller, XboxController.Button.kLeftBumper.value);
btn_main_RBumper = new JoystickButton(sys_controller, XboxController.Button.kRightBumper.value);
btn_main_LAnalog = new JoystickButton(sys_controller, XboxController.Button.kLeftStick.value);
btn_main_RAnalog = new JoystickButton(sys_controller, XboxController.Button.kRightStick.value);
btn_main_Back = new JoystickButton(sys_controller, XboxController.Button.kBack.value);
btn_main_Start = new JoystickButton(sys_controller, XboxController.Button.kStart.value);
```



## Requirements

WPILib should be [installed](https://docs.wpilib.org/en/stable/docs/zero-to-robot/step-2/wpilib-setup.html#wpilib-installation-guide), and you should be using their version of VSCode.

## Release Notes

### 0.0.2

- Add controller snippets
- Reformat README.md

### 0.0.1

- Initial release of FRC Snippets

## Disclaimer:
This VSCode extension is in no way related to Visual Studio Code, Microsoft, First Robotics, WPILib, or any other company/organization.