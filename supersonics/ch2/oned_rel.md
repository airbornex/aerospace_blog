# 2.2 One Dimensional Flow Relations

```{code-cell} python
:tags: [executable]
import numpy as np
# Calculate Mach number for a given speed and speed of sound
speed = 1230  # m/s (example: speed of an aircraft)
speed_of_sound = 343  # m/s (at sea level)
mach_number = speed / speed_of_sound
print(f"Mach Number: {mach_number:.2f}")
```