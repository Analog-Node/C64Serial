# C64 User Port Pin Mapping

This document describes the intended mapping between Commodore 64 user
port signals and RS-232 signals for the C64Serial adapter.

This is a planning document and may change prior to PCB release.

---

## Minimum Required Signals

| C64 User Port | CIA Signal | Function | RS-232 Signal |
|--------------|------------|----------|---------------|
| PA2          | TXD        | Transmit | TXD           |
| PB0          | RXD        | Receive  | RXD           |
| GND          | GND        | Ground   | GND           |

---

## Optional Handshake Signals (TBD)

| C64 User Port | Function | RS-232 |
|--------------|----------|--------|
| PA3 / PB1    | RTS/CTS  | RTS/CTS |
| PA4 / PB2    | DTR/DSR  | DTR/DSR |

Final selection of handshake signals is pending design review.

---

## Notes

- User port signals are TTL-level and may be inverted relative to RS-232.
- Level shifting is expected to be handled via MAX232-compatible devices.
- Support for UP9600-style wiring is under consideration.
