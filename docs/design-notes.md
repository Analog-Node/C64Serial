# Design Notes

## Project Goals

- Simple, reliable C64 User Port → RS-232 adapter
- Open hardware with clear attribution
- Easy to manufacture and assemble
- Minimal active components

## Non-Goals

- USB serial support
- Integrated modem or firmware
- Bus-powered peripherals beyond RS-232 conversion

## Electrical Design

- RS-232 voltage conversion via MAX232-compatible IC
- External charge-pump capacitors per datasheet
- Protection against incorrect cable insertion

## Open Questions

- Should UP9600 wiring be supported?
  - Fixed wiring
  - Jumper-selectable
  - Separate board variant

- How many handshake lines should be exposed?
  - TX/RX only
  - RTS/CTS
  - Full modem control

## Licensing Considerations

- Current work is derived from Plus4Serial (CC BY-NC-SA 4.0)
- Alternative licensing is being discussed with the upstream author
- Clean-room redesign may be pursued if required
