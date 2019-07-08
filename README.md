# digiNRG - Whole Home Power Monitoring with ESPHome
Whole home power monitoring and additional circuits with ESPHome and Home Assistant.  Other home automations can also use this implementation as well with the MQTT option.

Video Demostration and Setup - 

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

### Sample ESPHome YAML Configurations
digi_nrg_2chan32.yaml - Included in this repo   
digi_nrg_6chan32.yaml - Included in this repo  

![alt text](https://raw.githubusercontent.com/digiblur/digiNRG_ESPHome/master/jpgs/2chan_board.jpg "2 Channel")  
![alt text](https://raw.githubusercontent.com/digiblur/digiNRG_ESPHome/master/jpgs/6chan_board.jpg "6 Channel")  
![alt text](https://raw.githubusercontent.com/digiblur/digiNRG_ESPHome/master/jpgs/sct_100a.jpg "SCT")  

