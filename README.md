# AQUAFUR
![](https://user-images.githubusercontent.com/83724898/117202883-5c5d3000-adbc-11eb-998a-dc662f796f75.png)
## Summary
Our idea with the Aquafur was to create a product that would automatically refill your pet's water bowl seamlessly, while everyone is away at work and alert the owner of the pet's drinking habits to key them in on their dogs health. The Aquafur was also intended to send a text message to the owner, altering them of every time the valve was opened, and the bowl was filled. Although we did get the automatic refilling capabilities to work reliably, the Bluetooth component of this project (that sent the notification) was completely unreliable. 

***

## Design
### Materials
* Plastic Water Reservoir
* Bowl
* Float Switch
* Orbit 1-in Plastic Electric Inline Irrigation Valve
* Arduino RedBoard
* Breadboard
* 1k ohm resistor
* NPN Transistor
* DPDT Relay 1A/125V AC (2A/30V DC)
* 24 V Power Supply
* BlueSmirf Bluetooth Component
* Sealant 

### Assembly 
> Physical Components 
1. Cut a 1 inch hole in the bottom middle of the water reservoir. 
2. Secure the valve inside the water reservoir, with the wires placed outside.
3. Cover the remaining hole with the sealant of your choice, we used 100% silicone caulking. 
4. Place the reservoir with the attached (and sealed) valve on a stand that is tall enough to fit the bowl under the spout. 
5. Place the bowl under the spout and fill your reservoir.
6. Connect the valve to the circuit via the white and red jumper cables. 

![](https://user-images.githubusercontent.com/83724898/117204999-06d65280-adbf-11eb-8bee-f6652c4eee71.png)

> Circuitry 
 
![](https://user-images.githubusercontent.com/83724898/117203782-73505200-adbd-11eb-8ba0-ca95a06ea24c.png)

> Code

![](https://user-images.githubusercontent.com/83724898/117206219-93cddb80-adc0-11eb-8746-4eab4932fbc8.png)
![](https://user-images.githubusercontent.com/83724898/117206548-ffb04400-adc0-11eb-84ce-29bbab206bee.png)
![](https://user-images.githubusercontent.com/83724898/117206641-19518b80-adc1-11eb-8f7a-915fece89698.png)

***

## Testing

### Procedures
A multimeter was used to test to ensure that the correct voltages were entering each component. Ultimately the multimeter was used to ensure that 24 V were going into the irrigation valve. To test the application, the MIT App inventor app was used on a Samsung device. After each line of code was added the app was ran using the software t ensure that it was working properly. Alot of troubleshooting was done at this stage to 
get connection to the BlueSmirf. Make sure you use a Samsung device, as the BlueSmirf does not connect to iPhones. 

### Results
 The system was tested a different water bowl levels. First it was tested to see if it would fill up when the float sensor was closed. This proved to be successful. Then it was tested to see if it stopped flowing when the water level rose and the sensor was open. This also proved to be successful. To attempt to get better flow it was tetsed to see if more water in the tank allowed for more water to flow through the valve. This test was unsuccessful because the water flow did not increase with added water in the tank. The app was continuously tested to see if it was successful. Unfortunately due to poor connection with the blueSmirf and other unknown circumstances the app was not successful. It is believed that the code would work but it was impossible to test it with the state of the bluetooth connection. 

### Discussion
The system has many restrictions. It must be connected to a 24V power source to supply enough power to the irrigation valve. The bluetooth connection was very spotty. If this project is recreated we recommend that a better bluetooth device is used. Another limitation is that with the valve that was used the water comes out very slowly. This would not be good practice in a household with a large dog that drink water quickly. This design would be more suited for a cat.
