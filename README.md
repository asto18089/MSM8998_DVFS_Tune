# MSM8998_DVFS_Tune
Reference DTS parameters for tuning a MSM8998 device's DVFS behaviour.

The parameters, as you can see, are contained in a whole, particular DTS file for the sake of completeness. Only the CPR3 and CPRh node are to be referenced and all other nodes should be ignored since there is no guarantee it will work on any device. It's pulled randomly from a set of eight(8) DTSes, and I don't know for now which one the device actually uses.

Please note that the parameters are highly customized to a particular device. It is, and always should, only for reference purpose. Compability with other devices should be treated as unknown prior to thorough, all-temp-band stress testing.

Summary of the changes:

1. Decreased open-loop and close-loop fuse adjustment voltage. The final corner voltages will be lowered since they are based on the interpolation result of the fuses.
2. [TO BE CONFIRMED] Applied a temperature offset on the Gold cluster. I cannot confirm its working by now, since the DVFS before the offset is already working quite fine. It indeed showed a freeze in high-load stress tests, but it cannot be steadily reproduced. Maybe It's a sign for coming quite close to the extreme:) 
