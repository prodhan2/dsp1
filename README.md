Here is a modern, clean, and professional **Markdown version** of your DSP Lab-29 repository overview. It includes visual hierarchy, emoji icons for sections, and consistent formatting suitable for GitHub or documentation use:

---

# 📊 DSP LAB-29 — Signal Processing with Python

This repository contains Python code and visualizations for core **Digital Signal Processing (DSP)** concepts. Each notebook explores key operations like signal generation, sampling, convolution, and spectral analysis using libraries like NumPy, Matplotlib, and SciPy.

---

## 📂 Contents

### 🔹 1. Elementary Signal Generation

Create and plot the following signals:

* **Unit Step:**      `u(n)`
* **Ramp:**         `n · u(n)`
* **Exponential:**     `aⁿ · u(n)`
* **Sinusoidal:**      `sin(ωn)`, `cos(ωn)`

📄 **File:** `01_elementary_signals.ipynb`

---

### 🔹 2. Sampling & Aliasing

Visual demonstration of **aliasing** using:

* Analog Signal: `xₐ(t) = 3cos(100πt)`
* Sample Rates:

  * ✅ **200 Hz** (Nyquist Rate)
  * ❌ **75 Hz** (Aliasing Occurs)

📄 **File:** `02_sampling_aliasing.ipynb`

---

### 🔹 3. Maximum Oscillation at ω = π

Show that **ω = π** yields the fastest oscillation in:

```
x[n] = cos(ωn)
```

📄 **File:** `03_max_oscillation.ipynb`

---

### 🔹 4. Complex Analog Signal Sampling

Analog signal:

```
xₐ(t) = 3cos(2000πt) + 5sin(6000πt) + 10cos(12000πt)
```

Sampled at:

* 🔻 Below Nyquist
* ⚖️ At Nyquist
* 🔺 Above Nyquist

✅ Observe **aliasing** and **frequency folding** effects.

📄 **File:** `04_complex_sampling.ipynb`

---

### 🔹 5. LTI System Convolution

LTI System defined by:

* **Impulse Response:** `h[n] = u(n) - u(n−5)`
* **Input Signal:** `x[n] = u(n)`
* **Output via Convolution:** `y[n] = x[n] * h[n)`

📄 **File:** `05_convolution_lti.ipynb`

---

### 🔹 6. Correlation

Given:

```plaintext
x(n) = [1, 3, -2, 4]
y(n) = [2, 3, -1, 3]
z(n) = [2, -1, 4, -2]
```

✅ Compute:

* Cross-correlation between `x(n)` and `y(n)`
* Cross-correlation between `y(n)` and `z(n)`

📄 **File:** `06_correlation.ipynb`

---

### 🔹 7. Filter Realization

Implement:

* **Averaging Filter (6-point):**

  ```
  y[n] = (1/6)·(x[n] + x[n−1] + ... + x[n−5])
  ```
* **Differencing Filter (6-point):**

  ```
  y[n] = x[n] − x[n−6]
  ```

📄 **File:** `07_filter_realization.ipynb`

---

### 🔹 8. DFT and Windowing

Signal:

```
x[n] = sin(2π·1000t) + 0.5·sin(2π·2000t + 3π/4)
```

Tasks:

* DFT without window
* DFT with **Hamming** and **Hanning** windows

🔍 Observe:

* **Spectral leakage**
* **Window smoothing**

📄 **File:** `08_dft_windowing.ipynb`

---

### 🔹 9. Low-Pass FIR Filter Design

🧪 Steps:

* Add high-frequency noise to a signal
* Design **Low-Pass FIR Filter** using a Hamming window
* Apply filter using **convolution**
* Visualize output in time and frequency domains

📄 **File:** `09_fir_filter.ipynb`

---

## 📦 Requirements

Install dependencies:

```bash
pip install numpy matplotlib scipy
```

---


