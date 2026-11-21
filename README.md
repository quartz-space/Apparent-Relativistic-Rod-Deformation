# Two-Light-Year Stick: True Shape vs. Observer View

An interactive 2D physics visualization exploring why a two-light-year stick swung at one end does **not** move rigidly or appear straight—comparing its **real-time physical curve** against the **time-delayed apparent shape** seen by an observer due to finite wave speed and light-travel delay.

---

## What It Demonstrates

* **Mechanical Wave Lag:** Moving one end launches a wave down the rod at a finite propagation speed (`vWave`), rather than moving the entire stick instantaneously.
* **Optical / Light-Travel Delay:** Light from different segments along the rod takes time to reach the observer (`obsY`), shifting what is *seen* relative to where segments actually are at simulation time `t`.
* **True vs. Apparent Geometry:** Lets you contrast the instantaneous physical curve of the rod against the apparent curve reconstructed from delayed light/photons (`showPhotons`).

---

## State & Parameters

Based on the saved visualization state:

| Parameter | Current Value | Role |
| --- | --- | --- |
| `vWave` | `0.27` | Wave propagation speed along the rod (normalized units/s) |
| `freq` | `0.45` | Oscillation / swing frequency driving the rod (`Hz` in sim units) |
| `obsY` | `-18` | Observer position offset along the vertical axis |
| `isPlaying` | `true` | Controls whether the real-time animation loop is running |
| `showPhotons` | `true` | Toggles display of photon/light-delay cues or apparent observer view |

---

## How to Interact

1. **Play / Pause (`isPlaying`):** Pause at any moment to inspect how far the wave has traveled along the rod versus what the observer sees.
2. **Adjust Wave Speed (`vWave`):** Lower speeds pack more bends/ripples along the rod and increase lag; higher speeds make the rod respond faster along its length.
3. **Adjust Swing Frequency (`freq`):** Higher frequencies create tighter, more frequent waves along the rod; lower frequencies produce broader curves.
4. **Move Observer Position (`obsY`):** Change where the observer sits relative to the rod to see how distance/angle alters arrival times and apparent shape.
5. **Toggle Photon / Delay View (`showPhotons`):** Switch or compare light-travel / photon cues to separate optical delay from physical wave propagation.

---

## Physical Caveats

* **Scale & Relativistic Limits:** Treating a macroscopic solid rod as two light-years long is a conceptual thought experiment; real materials fracture, buckle, or vaporize under extreme stresses, and no causal signal or physical wave can exceed the speed of light ($c$).
* **Normalized Simulation Units:** Lengths, frequencies, and wave speeds use normalized simulation units to make slow wave propagation and light-lag visible on human timescales.
