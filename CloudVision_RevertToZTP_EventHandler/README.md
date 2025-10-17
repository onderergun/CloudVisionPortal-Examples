# Revert To ZTP Event Handler

During a ZTP operation, when CloudVision (CV) pushes the designed config to the device and the device reloads, the communication channel to CV can be broken due to a faulty designed config (incorrect default route, mgmt IP address issue, etc.). If this event handler is added to the designed config, it would force the device back into ZTP mode if the connectivity to CV is broken after the device reloads with the desired configuration.

# Usage

This event handler works for EOS versions >= `4.24.0` and TerminAttr/Streaming Agent versions between `[1.30.0, 1.42.0)`

TerminAttr/Streaming Agent running on the device can be upgraded as part of the ZTP process by configuring the **ZTP Upgrade Version** tab of the Software Management Studio.
