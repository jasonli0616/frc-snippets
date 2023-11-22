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



## Requirements

[WPILib](https://github.com/wpilibsuite/allwpilib/releases) should be installed, and you should be using their version of VSCode.

## Release Notes

### 2024.0.4

- Use year-based version numbers
- Update for WPILib 2024 changes

### 0.0.3

- Remove controller snippets (due to 2023 change in WPILib)

### 0.0.2

- Add controller snippets
- Reformat README.md
- Add license

### 0.0.1

- Initial release of FRC Snippets

## Disclaimer:
This VSCode extension is in no way related to Visual Studio Code, Microsoft, First Robotics, WPILib, or any other company/organization.