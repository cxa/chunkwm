### HEAD -  not yet released

----------

### version 0.3.6

#### other changes

- fixed an issue that caused applications to be ignored by chunkwm due to slow startup-time (#329)

----------

### version 0.3.5

#### other changes

- fixed an issue that caused chunkwm to crash if the user tried to query a non-existing cvar (#378)

----------

### version 0.3.4

#### other changes

- fixed an issue where a window would incorrectly be deemed invalid due to an obscure issue with registering notifications.

----------

### version 0.3.3

#### cvar changes

- added new option to set logging-output in the config-file:
  `chunkc core::log_file <stdout | stderr | /path/to/file>`

----------

### version 0.3.2

#### other changes

- fixed an issue with identifying monitors by arrangement.

----------

### version 0.3.1

#### launch argument

- removed launch argument to set logging-level. logging-level is set in the config-file!

#### other changes

- fixed a race-condition that could cause plugin-commands to be attempted to be ran before
  the plugin was successfully loaded.

- fixed an issue that could cause argument parsing in plugin-commands to fail due to not properly
  resetting the state of *getopt*.

----------

### version 0.3.0

#### launch argument

- added new launch argument to set logging-level:
  ```
  chunkwm --log-level <option>
  <option>: none | debug | warn | error
  ```

#### cvar changes

- added new option to select logging-level during runtime:
  `chunkc core::log_level <none | debug | warn | error>`

#### other changes

- plugin commands are now ran through the main event-queue, for safety-reasons.

----------

### version 0.2.36

changes from previous versions are unavailable..
