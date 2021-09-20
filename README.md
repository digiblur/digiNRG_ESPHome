# digiNRG - Whole Home Power Monitoring with ESPHome
Whole home power monitoring and additional power circuits with ESPHome and Home Assistant. This implementation utilizes the ATM90E32AS based board from CircuitSetup. Other home automation software supporting MQTT can also use this integration.

Video Demostration and Setup - https://youtu.be/BOgy6QbfeZk

Update 2019/08/24 - For v1.2 of the board your voltage calibration will be high, >64,000. This is normal.

### Parts List
[Split Core Current Transformer 100A/50ma](https://amzn.to/2JtuRSt)  
[ESP32 NodeMCU](https://amzn.to/2XvEBAs)  
[CircuitSetup 6 Channel or 2 Channel Board](https://circuitsetup.us/index.php/product-category/power-management/)  
[9VAC Power Supply](https://amzn.to/2Jt4uMh)

### Sample Calibrations for SCT Sizes
If you have any to add or changes to these, pleast let us know! These are based on the 6 channel board with 1X gain.  
[SCT-013-000 100A/50ma](https://amzn.to/2JtuRSt) - 32498  
[SCT-013-050 50A/1V](https://amzn.to/2XzkyB3) - 15420  
[SCT-013-030 30A/1V](https://amzn.to/2FZLdB9) - 9210  

[SCT-024TSL-B27 200A/100mA](https://circuitsetup.us/product/200a-100ma-current-transformer-yhdc-sct-024-24mm/) - 12597 \*(2 chan board, gain_pga = 4X)

### Sample Calibrations for Gain Voltage (`gain_voltage`)
For the 2 channel board and the 9VAC power supply:
[SCT-013-000 100A/50ma](https://amzn.to/2JtuRSt) - 3900

### Sample ESPHome YAML Configurations
digi_nrg_2chan32.yaml - Included in this repo   
digi_nrg_6chan32.yaml - Included in this repo
Note: If you elected to add expansion boards, refer to the two physical jumpers on the top of each expansion board. They will identify each of the CS_PINs you will need to include in the 6 channel example above. You can then replicate the code and change the CS_Pin and CT identifiers.

![alt text](https://raw.githubusercontent.com/digiblur/digiNRG_ESPHome/master/jpgs/2chan_board.jpg "2 Channel")  
![alt text](https://raw.githubusercontent.com/digiblur/digiNRG_ESPHome/master/jpgs/6chan_board.jpg "6 Channel")  
![alt text](https://raw.githubusercontent.com/digiblur/digiNRG_ESPHome/master/jpgs/sct_100a.jpg "SCT")  
