<div align="center">

<img src="https://img.shields.io/badge/SIH%202026-VITBSIH26--388-blueviolet?style=for-the-badge" />
<img src="https://img.shields.io/badge/detection→isolation-%3C%202s-success?style=for-the-badge" />
<img src="https://img.shields.io/badge/BOM-%3C%20₹1%2C800%2Fnode-informational?style=for-the-badge" />

# ⚡ Closed-Circuit — sentinel-lv

**Automatic detection and isolation of snapped low-voltage overhead conductors.**

> A live wire on the ground draws < trip current in dry earth —  
> fuses and OC relays stay silent. People die. We fix that.

---

## How it works

```
Capacitive E-field probe (non-contact, 50 Hz)
        ↓ STM32L4 / ESP32-S3 · SX1262 LoRa mesh
        ↓ quorum of neighbours must agree
        ↓ Gateway at feeder head
        ↓ Isolates in < 2 s
        ↓ Cloud observes · alerts · audits
```

**No false trips in bench tests · < 5 mA avg · ≥ 300 m LoRa LOS · BOM < ₹1,800/node**

---

## Repositories

| Repo | Contents |
|------|----------|
| [protocol](https://github.com/sentinel-lv/protocol) | Frozen shared contract — `PROTOCOL.md`, test vectors, `decide()` spec |
| [platform](https://github.com/sentinel-lv/platform) | Frontend · Backend · Simulator — deploys together |
| [edge](https://github.com/sentinel-lv/edge) | Firmware (STM32/ESP32 + SX1262) · Gateway (LoRa concentrator + relay) |
| [hardware](https://github.com/sentinel-lv/hardware) | KiCad schematics · BOM · characterisation data · enclosure STLs |

---

## Demo

> **Simulated feeder · live consensus engine**  
> Every demo runs a virtual 12-node KSEB feeder with a real arbiter.  
> No 230 V hardware is implied unless the M5 rig is on stage.

---

<sub>Built for KSEBL · VIT Bhopal · SIH 2026</sub>

</div>
