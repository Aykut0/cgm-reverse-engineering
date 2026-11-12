# Reverse-Engineered CGM Board

A buildable re-design of the electronics of a commercial continuous glucose monitor.

![Assembled board](docs/images/cgm-board.jpg)

A CGM is a coin-sized patch that reads glucose continuously through a thin electrochemical sensor under the skin. I took a commercial device apart, traced how its electronics read the sensor and send the data out, and redrew the circuit as a round board that can be built and changed freely, as a base for trying new glucose sensors.

The glucose electrode produces a small current that follows the glucose level. A TI RF430FRL152H sensor interface biases the electrode, digitizes the signal and can be read over NFC, and an EM Microelectronic EM9304 module adds Bluetooth Low Energy for streaming to a phone. The board runs from a coin cell and keeps the round shape and central opening of the original, with the flexible sensor probe attached at the edge.

| Board with the flexible probe | Front |
|---|---|
| ![Board with the flexible probe](docs/images/cgm-board-with-probe.jpg) | ![Board front](docs/images/cgm-board-front.jpg) |

![Layout and 3D view in Altium Designer](docs/images/cgm-layout-in-altium.jpg)

## Files

```
hardware/altium/   Altium project (open CGM.PrjPcb), schematic, layout and libraries
docs/images/       photos
```

---

Yaşar Aykut Altuntop · Koç University · [LinkedIn](https://linkedin.com/in/aykutaltuntop) · [GitHub](https://github.com/Aykut0)
