# Dual-tone-Multi-frequency-DTMF-signaling-schemes

## Project Description

This project involves using Matlab to perform various tasks related to time-frequency analysis and spectrograms. The objective is to become familiar with the notion of time-frequency analysis, particularly with Dual-tone Multi-frequency (DTMF) signaling schemes.

## Introduction

### DTMF

- DTMF is a signaling scheme used in Touch-Tone systems where each key press is represented by a combination of two tones.
- Eight frequencies are arranged to accommodate 16 characters, operating at a sampling rate of 8 kHz.

### Time-Frequency Analysis

- Many practical signals are non-stationary, meaning their frequency-domain representation changes over time.
- Time-frequency analysis determines when specific frequency components are present in a signal.
- Fourier analysis provides high-frequency resolution but no time information.

## Steps

Use Matlab to perform the following tasks:

1. **Generate DTMF Signal**: Write a Matlab function `x = sym2TT(S)` to generate a 100 ms time-domain signal for a given DTMF symbol S.
2. **Create DTMF Sequence**: Generate a signal containing a sequence of DTMF symbols representing your cell phone number with 20 ms guard intervals.
3. **Add Noise**: Create a signal contaminated with additive white Gaussian noise (variance 0.1).
4. **Store Audio**: Save the generated signal as a .wav file.
5. **Plot Signal**: Plot the noisy signal in the time domain.
6. **Plot Spectrum**: Use FFT to plot the magnitude spectrum of the noisy signal in the frequency range 600 Hz to 1700 Hz.
7. **Create Spectrograms**: Write Matlab code to create spectrograms using different window sizes and types (rectangular and blackman).

### Additional Analysis

- Identify window sizes with the worst time-domain and frequency-domain resolutions.
- Determine the optimal trade-off between time and frequency resolutions.
- Compare frequency resolution between rectangular and blackman windows for a given size.

### DTMF Decoding

- Research the Matlab `goertzel` function to decode DTMF symbols.
- Write Matlab code to decode the noisy signal and verify the decoded sequence.

## Useful Matlab Commands

- `randn`, `fft`, `fftshift`
- `audioread`, `audiowrite`
- `rectwin`, `blackman`
- `imagesc`, `flipud`, `colorbar`
- `set(gca,'YDir','normal')`, `axis`, `goertzel`
