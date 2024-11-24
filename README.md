# Mbed-NTP library for MbedCE

The NTP (Network Time Protocol) client library is able synchronize your internal clocks with accurate time sources on the internet.
By leveraging the NTP protocol, these libraries enable devices to maintain precise timekeeping, which is crucial for various applications under MbedCE.

## How to start
1. Create a new project according to [MbedCE instructions](https://github.com/mbed-ce/mbed-os/wiki)
2. Add this as submodule to your project via `git submodule add --depth 1 https://github.com/mbed-ce-libraries-examples/mbed-NTP mbed-NTP`
3. The top level `CMakeList.txt` (in root of your project) should be modified according to [this wiki page](https://github.com/mbed-ce/mbed-os/wiki/MbedOS-configuration#libraries-in-your-application)
   ```
   #[[link MbedOS and its libraries (necessary everytime)]]
   target_link_libraries(${CMAKE_PROJECT_NAME}  mbed-os mbed-netsocket) 

   ### link user library (if needed)
   target_link_libraries(${CMAKE_PROJECT_NAME} mbed-ntp)
   ```
4. Make your program
5. Build the project

### Status:
This library is not tested yet.
