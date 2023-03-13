ode_tts
===

This repo contains the implementation of my TTS model named ODE-TTS for my study.

The purpose of this repo is to confirm that effect of noise compared with grad_tts.  

At least in this problem, noise in trajectries between distributions has important role that not only act as reguralization but also promotes to learn high-frequency features.  

In my experiments, Grad-TTS generates high-fidelity mel-spectrograms properly by probability flow ode, but ODE-TTS cannot generate ones.  

Then I have a question that if noise makes learning high-frequency features, adding constant noise to ode trajectries like Conditional Flow Matching can be effective?

As a result, it works a little better, but is significantly less effective than Grad-TTS.  
Generated mel-spectrograms by ODE with noise are so smoothed.
