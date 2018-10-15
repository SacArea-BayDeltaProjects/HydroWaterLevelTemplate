# WaterLevelTemplate
Simple Water Level program for use with Campbell Scientific CR1000 or CR6.
This can be used for a single station or to calculate the difference in head between two stations using a Master/Slave configuration.

Use Customize Constants function to tell the master datalogger which port to look for the slave datalogger in.
The variable "SlaveCom" is referring to the port that the Master Datalogger uses to communicate with the Slave.
CR1000 CANNOT USE ComRF. If using RF radio on CR1000, set radio up to use either the RS232 port or CS I/O. If CS I/O, use ComSDC7 for "SlaveCom".
If using CR6 with internal radio, use ComRF. If it's necessary to add other possible links for either system, we can do so.

Port Selection for Pressure Sensor Data wire: For CR1000, use either C3 or C5. For CR6, use C3 or U5. This made it easier to be consistent with variable names.
