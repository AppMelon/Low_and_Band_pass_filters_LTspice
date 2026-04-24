# Filter Design and Simulation

## 1. Low-Pass RC Filter

### Circuit
RC low-pass filter with:
- R = 10kΩ
- C = 10nF

### Transfer Function
H(s) = 1 / (1 + sRC)

### Cutoff Frequency
fc = 1 / (2πRC) ≈ 1.59 kHz

### Observation
- Passes low frequencies
- Attenuates high frequencies
- Roll-off: -20 dB/decade

---

## 2. Band-Pass RLC Filter

### Circuit
- L = 1.5 mH
- C = 56 nF
- R = 238 Ω

### Transfer Function
H(s) = R / (R + sL + 1/(sC))

### Resonant Frequency
f0 = 1 / (2π√(LC)) ≈ 5.5 kHz

### Behavior
- Attenuates low and high frequencies
- Passes mid-frequency range (1 kHz – 10 kHz)

---

## 3. Simulation

Simulations performed using LTspice with AC analysis:
- Low-pass shows expected roll-off
- Band-pass shows peak near resonance

---

## 4. Files
- lowpass.asc
- bandpass.asc
