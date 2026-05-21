# Moth Hybrid - ZMK Config

## Overview
- Keyboard: Moth Hybrid (71 keys, split)
- Controller: Seeed Studio XIAO nRF52840 Plus
- Firmware: ZMK

## Structure
- board/ -> Separate GitHub repo: zmk-component-xiao-ble-plus
- config/ -> Your zmk-config repo (includes shield under boards/shields/moth_hybrid/)

## Pin Mapping
### Rows (both halves): D10, D9, D8, D7, D19
### Cols Left: D0, D1, D2, D3, D4, D5, D6
### Cols Right: D0, D1, D2, D3, D4, D5, D6, D11, D12

## Setup
1. Create repo zmk-component-xiao-ble-plus with board/ contents
2. Create repo zmk-config-moth-hybrid with config/ contents
3. Update west.yml with your GitHub username
4. Push -> GitHub Actions builds -> download .uf2 artifacts
5. Flash left half first (BLE central), then right half
