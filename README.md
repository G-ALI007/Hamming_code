# BPSK BER Performance Analysis in AWGN and Rayleigh Channels

## Overview
This repository contains a collection of MATLAB simulations designed to analyze the Bit Error Rate (BER) performance of Binary Phase Shift Keying (BPSK) modulation. It evaluates system performance under both Additive White Gaussian Noise (AWGN) and Rayleigh fading channels. Additionally, it explores the improvements provided by Forward Error Correction (FEC), specifically Hamming (7,4) coding, data Interleaving, and soft/hard decision decoding.

## Repository Contents

* **`script_bpsk_ber_awgn_hamming_7_4_code_soft_hard_decoding.m`**
  Computes the BER for BPSK in an AWGN channel using Hamming (7,4) code, and compares the results of both soft and hard decision decoding methods.

* **`BPSK_AWGN.m`**
  A comparative simulation of BER performance between Hamming-coded and uncoded BPSK over an AWGN channel.

* **`BPSK_Rayleigh.m`**
  Simulates a Rayleigh Fading Channel, analyzing the system's BER with Hamming coding and illustrating the effect of adding data interleaving to combat burst errors.

* **`script_ber_bpsk_rayleigh_channel.m`**
  Calculates and plots the simulated versus theoretical BER for BPSK modulation specifically over a Rayleigh fading channel.

## Requirements
* MATLAB (Tested and fully compatible with version 2022b)
* Communications Toolbox (required for functions like `comm.RayleighChannel`, `encode`, `decode`, `intrlv`, etc.)

## Acknowledgments
* Portions of this repository (`script_bpsk_ber_awgn_hamming_7_4_code_soft_hard_decoding.m` and `script_ber_bpsk_rayleigh_channel.m`) are based on the original work by Krishna Pillai (dsplog.com).
