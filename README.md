<h1 align="center">
  <br>
  OM-GOD
  <br>
</h1>

<h4 align="center">
Ominichord [Gate of Divinity]. Mash-up of all the previous omnichords and more.
</h4>

<div align="center">

![KiCad](https://img.shields.io/badge/kicad-%2300578F.svg?style=for-the-badge&logo=kicad&logoColor=white)
![STM32](https://img.shields.io/badge/STM32-%23032F34.svg?style=for-the-badge&logo=stmicroelectronics&logoColor=white)
![Texas Instruments](https://img.shields.io/badge/Texas%20Instruments-%23DC440E.svg?style=for-the-badge&logo=texas-instruments&logoColor=white)

</div>

<p align="center">
  <a href="#key-features">Key Features</a> •
  <a href="#design-process">Design Process</a> •
  <a href="#pcb">PCB</a> •
  <a href="#bom">BOM</a> •
  <a href="#journal">Development Journal</a> •
  <a href="#credits">Credits</a> •
  <a href="#license">License</a>
</p>

## Key Features

- **STM32H7 microcontroller** for high-performance processing
- **Texas Instruments DACs and amplifiers** for professional audio quality
- **MIDI connectivity** for external device integration
- **USB-C programming and power delivery**
- **Battery-powered portable design**
- **Cherry MX mechanical switches** for tactile feedback
- **48-button chord matrix** (4 rows × 12 buttons)
- **Rotary encoders** for parameter control
- **LED display** for status and settings

## Design Process

<img src="assets/gdrive.png" alt="Google Drive Reference" width="600"/>

The OM-GOD project began with extensive research into existing omnichord designs and their features. After compiling schematics and manuals, I created a comprehensive feature list to guide the development process.

## PCB

Designed in KiCad with a focus on audio quality and modern features. Notable components:

- **STM32H7** microcontroller with 144 GPIO pins
- **PCM5122PW DAC** for high-quality audio conversion
- **TPA3116D2DAD Class D amplifier** for powerful audio output
- **BQ24610** battery charging circuit for portable operation
- **Multiple voltage regulators** (12V, 15V, 5V, 3.3V)
- **USB-C power delivery** with negotiator circuit
- **NFC antenna** for contactless communication

### Schematic Development

<img src="assets/schematic_initial.jpg" alt="Initial Schematic" width="500"/>
<img src="assets/schematic_final_2.png" alt="Final Schematic" width="500"/>

The schematic evolved through multiple iterations, starting with basic component selection and progressing to a complete audio system with power management, I/O interfaces, and user controls.

### Component Integration

<img src="assets/DAC_2.png" alt="DAC Wiring" width="400"/>
<img src="assets/buffer.png" alt="Buffer Wiring" width="400"/>

Key integration challenges included:

- Audio signal buffering for noise reduction
- Power distribution for multiple voltage rails
- Component placement optimization
- Signal integrity considerations

### PCB

<img src="assets/pcb.png" alt="PCB" width="400"/>

<img src="assets/pcb_back.png" alt="PCB" width="400"/>

The PCB layout was made to ensure a proper audio quality. All analog traces  and chips are on the bottom layer, while digital traces are on the top. Also, the gnd plane in the inner bottom layer acts as a faraday's cage, not letting them interfier with each other.

### Final Design

<img src="assets/CAD.png" alt="CAD Design" width="600"/>

The final design incorporates all planned features while maintaining a compact, portable form factor suitable for live performance.

## BOM

| Component  | Source        | Cost (USD)  |
| ---------  | ------        | ----------- |
| PCB        | JLCPCB        | $348.25     |
| SPEAKER    | MERCADO LIBRE | $7.00       |
| FLEX CABLE | MERCADO LIBRE | $4.42       |
| JST CABLE  | MERCADO LIBRE | $5.00       |
| **Total**  |               | **364.67** |

_Note: Speakers, keycaps, and case are already owned components from previous projects._

## Credits

This project uses:

- [KiCad](https://www.kicad.org/) - PCB design
- [STM32](https://www.st.com/en/microcontrollers-microprocessors/stm32h7-series.html) - Microcontroller
- [Texas Instruments](https://www.ti.com/) - Audio and power components
- [Fusion 360](https://www.autodesk.com/products/fusion-360/) - 3D modeling

## License

MIT

---

> GitHub [@Sojooo](https://github.com/Sojooo)
