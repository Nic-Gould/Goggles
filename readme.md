# OpenHUDware.self
Like fpvcam/VR goggles but with front cam, environmental sensors. Designed as an opensource development platform for OpenHUD. Display a customisable dashboard. Weather widget, hud apps. Additional environmental awareness such as facial recognition, mood detection, low light filters, zoom, directional mic? Track hand, gensture input, on hud items

The initial project is a learning exercise that explores what can be acheived with readily available, resource constrained, cheap microcontrollers and components. Once the project architechture is in place, later versions may employ improved hardware and functionality. 

### components
* 7 inch LCD screen
* ESP32CAM w/ 5MP PLUS OV5642
* ESP32-S3-WROOM-1-N8 DEV BRD @ AU$22.31
* MPU-9250 GY-9250 9-axis gyro AU $11.79
* A google cardboard like set of goggles. These are available on amazon for about $15.
* Lattice Crosslink Plus FPGA LIF-MDF6000-6UMG64I 

**NOTES**
* I'd probably just use an android phone and some goggles, as the android phone provides cameras, gyro, screen, ram and processing power as well as software support for most of the required tasks. IIRC the newer pixel phones also include a TPU core for hardware acceleration of computervision and AI tasks. 
* Initial design used 2 x esp32cam and 2 x 3.5inch lcd screens with the aim of providing stereoscopic vision. For ease of development this was simplified. Parralell processing of stereo streams was cumbersome. Maybe in a future implementation.
* Better FPGAs by lattice support direct conversion of TF models into FPGA "code". Would recommend spending the extra money lol...