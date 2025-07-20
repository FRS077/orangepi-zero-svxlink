# Shield OrangePi zero SvxLink

The purpose of this PCB is to easily interface one or two radio transceivers with an Orange Pi Zero. This makes it easy to create a simplex or duplex SvxLink access point.

It is assembled on top of the Orange Pi Zero and connected to the radios by two mini DIN connectors.

## Built With

- KiCad v7 - _Open Source CAD software_
- KiCad v7 Librairies - _Symbols, footprints and 3D models librairies_
- LCSC - _Electronic parts provider_ & JLCPCB - _Board manufacturing_

## Specifications

### Mini DIN Pinout

| No Pin | Simplex / Duplex RX | Duplex TX |
| :----: | :-----------------: | :-------: |
|   1    |      Audio Out      | Audio Out |
|   2    |       Ground        |  Ground   |
|   3    |         PTT         |    PTT    |
|   4    |   Audio In (9600)   |   _N/C_   |
|   5    |   Audio In (1200)   |   _N/C_   |
|   6    |       Squelch       |   _N/C_   |

PTT is connected on the Orange Pi Zero to PA07 and Squelch to PA10.

### Solder bridge selectors

| Name  | Usage                                     |         Choice A          |   Choice B    |
| :---: | :---------------------------------------- | :-----------------------: | :-----------: |
|  JP1  | Select the audio input                    | Audio In 1200 _(default)_ | Audio In 9600 |
|  JP2  | Select simplex/duplex mode (audio output) |        Duplex mode        |  Simplex mode |
|  JP3  | Select simplex/duplex mode (PTT)          |        Duplex mode        |  Simplex mode |

## Authors

- **Quentin Rahms** - _Intial work_
- **Alexis Moyart** - _Completion_

## License

This project is licensed under the MIT License - see the LICENSE.md file for details