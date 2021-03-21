# SF65
## A ZMK-Powered BLE Keyboard with visible surface-mount components proudly displayed.

> :warning: **This is an untested project.** Do not use to create your own copy unless you are willing to debug the hardware and/or firmware. 

## Flash bootloader
Bootloader is pre-loaded on assembled pcbs. If you source your own BLE module you will need to unlock the module and flash the bootloader using the Nordic nrf command line tool. 
```
$ nrfjprog --recover --log 
```
```
$ nrfjprog -f nrf52 --program firmware/bootloader/COBO_nrf52840_bootloader-0.3.2-184-g64ea299_s140_6.1.1.hex
```

------------------------------------
## Upload Firmware 

- See ZMK docs for instructions on setting up ZMK and custimizing firmware.  
	* https://zmkfirmware.dev/docs/user-setup/
	* https://zmkfirmware.dev/docs/customization 
- Default *.uf2 files are pre-loaded on assembled pcbs. If you sourced and assembled your own pcb, you can file deafult pre-built firmware here: 
	- https://github.com/ericrlau/COBO-zmk-config/releases

## PCB
- Source files for pcb are in this repo. They are split into three kicad projects:
	- SF65: main pcb, left and right combined. 
	- (ToDo) SF65_Bottom: Bottom cover PCB. 
	- (ToDo) SF65_Plate: Switch plate PCB. 
	- NOTE: KiCad files are created with nightly KiCad 5.99 builds, they are not compatible with current stable release of KiCad 5.
- Bill of materials [Link](./PCB/bom/ibom.html)

## ToDo 
- Test prototypes.
- Create switch plate.
- Create bottom Cover.
- Create bottom foot to angle board.
- Fix silk screen arrow on 1U key to right of spacebar. 


## Images

#### Prototype Build

#### Main PCB
![Main TOP](./PCB/images/SF65_Top.jpg)
![Main BOTTOM](./PCB/images/SF65_Bottom.jpg)

#### FR4 Plate

#### Bottom PCB




