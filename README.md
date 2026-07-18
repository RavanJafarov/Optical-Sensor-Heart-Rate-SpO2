# Optical Sensor Measurement (Heart Rate & SpO₂)

**Author:** Ravan Jafarov (Student ID: 12255135)  
**Course:** Capstone Design 2 | **Instructor:** Prof. Daeyu Kim  

## Objective
To measure heart rate (BPM) and oxygen saturation (SpO₂) using the MAX30105 optical sensor. The project involves reading raw Red (660 nm) and IR (950 nm) signals, detecting pulse peaks, and calculating SpO₂ using a polynomial approximation of the AC/DC modulation ratio.

## Contents
- `Optical Sensor Measurement (Heart Rate SpO₂).pdf`: Full experiment report, including Arduino code for raw signal reading, peak detection, and SpO₂ calculation.

## Key Findings
- **Measurements:** Average heart rate stabilized at 74–76 BPM, with SpO₂ levels between 95–99%.
- **Signal Processing:** IIR and EMA filters were applied to extract AC and DC components from the PPG signal.
- **SpO₂ Calculation:** The polynomial approach (`SpO₂ = -45.060*R² + 30.354*R + 94.845`) provided smooth and stable results, though minor noise and finger placement variations introduced a ±2% margin of error.
- **Conclusion:** The MAX30105 sensor reliably analyzes PPG signals for accurate biometric monitoring when properly filtered and calibrated.
