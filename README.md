# MK60EC1 Long Code

> **Repository description:** MK60EC1 calculator — VIN + ABS module → long code hex for VCDS. Brazil-import Jetta 2009–2016 (1K0907379 AD/BL/CC). Single HTML file, works offline.

Static calculator in a single file: [`index.html`](index.html).

**Scope:** Brazil-import Jetta **2009–2016** · ABS module **MK60EC1** (1K0907379 AD / BL / CC).

## How to use

1. Open `index.html` in your browser (double-click — works on `file://`).
2. Enter the VIN (17 characters).
3. Choose module, brakes, ESP mode, and extras.
4. Copy the long code and write it in VCDS (Coding-07, module 03).

## Features

- VIN → long code (CC / BL / AD)
- Brake sizes 280 / 288 / 312 mm
- ESP/ASR mode (byte 19, CC module)
- Long Coding Helper (byte-by-byte decode)
- Migration between module indices

## Hiding code (View Source)

**You cannot hide HTML/JS in a web page.** The browser must download and run the code — View Source, DevTools (F12), and “Save page” always expose it.

Client-side obfuscation or “encryption” only slows casual reading; anyone can decode it in seconds. Real protection means running the logic on a **server** (API), not in the browser.

## Disclaimer

Educational tool only. Verify in VCDS before writing. Back up the module’s original long code.
