# Firmware Engineering Tech Interview

## Debugging

> How would you go about locating the cause of a stack overflow or watchdog timer reset?

> In most IDEs, when in debugging, a call stack window can be used to see what function calls were made
	when the overflow occurred. If in a FreeRTOS environment, this along with a stack overflow hook can
	be used to determine the task that is overflowing so it can be resized or optimized.
	
> For watchdog timer resets, I would try to implement an event handler and use the context of that interrupt
	to find the offending piece of code.
	