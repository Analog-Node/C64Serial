# Design Notes

## Goals

- Standalone C64 User Port → RS-232 adapter
- Simple, reliable, manufacturable
- Compatible with standard RS-232 devices
- Optional support for UP9600 wiring

## Non-Goals

- Not a modem
- No USB or TTL serial conversion
- No firmware or active logic beyond level shifting

## Open Questions

- UP9600 support via jumper or fixed wiring
- Handshake line support vs minimal TX/RX only
