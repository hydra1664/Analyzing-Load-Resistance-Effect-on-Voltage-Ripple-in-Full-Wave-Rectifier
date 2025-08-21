# Full-Wave Rectifier: Load Resistance Effect on Voltage Ripple

## Objective
The goal of this project was to understand how different load resistances affect the voltage ripple in a full-wave rectifier circuit with a capacitor filter. By varying the load resistor while keeping all other parameters constant, I was able to observe how the capacitor discharges under different conditions.

## Circuit Setup
The circuit is a standard full-wave rectifier built using:
- One AC voltage source  
- Four diodes in a bridge configuration  
- One capacitor filter  
- One load resistor  

The load resistance was changed across several values (100 Ω, 1 kΩ, and 10 kΩ) to study its impact on the output ripple.

## Simulation and Observations
Using LTSpice, I ran transient simulations and measured the output voltage across the load for each resistance value.

- At 100 Ω, the capacitor discharged much faster since more current was drawn. This resulted in a higher ripple and a less stable DC output.  
<img width="1920" height="1080" alt="100 Minimum Voltage" src="https://github.com/user-attachments/assets/3efdf45f-9d9c-4882-be13-b33c0ad5544e" />
<img width="1920" height="1080" alt="100 Maximum Voltage" src="https://github.com/user-attachments/assets/ae30c97f-3cf7-4984-854a-1952d5b69f00" />

- At 1 kΩ, the capacitor held its charge longer, reducing the ripple and producing a cleaner waveform.  
<img width="1920" height="1080" alt="1k Minimum Voltage" src="https://github.com/user-attachments/assets/040c8393-b3af-485b-b020-f9fc687d9b9b" />
<img width="1920" height="1080" alt="1k Maximum Voltage" src="https://github.com/user-attachments/assets/a7bf76d1-5d75-45ea-a016-690ef401cdd8" />

- At 10 kΩ, the discharge rate was even slower, making the output almost flat with very small ripple.  
<img width="1920" height="1080" alt="10k Minimum Voltage" src="https://github.com/user-attachments/assets/c923588d-d29b-4ae3-96fb-ab62cc5e26d1" />
<img width="1920" height="1080" alt="10k Maximum Voltage" src="https://github.com/user-attachments/assets/03eb3f6a-d009-46f5-8f42-bd8e2b242e74" />

The images above are simulation plots showing the minimum and maximum voltage points for each case.

## Conclusion
The results clearly show that load resistance plays a big role in determining the output ripple of a rectifier circuit. Lower resistance causes more ripple due to faster capacitor discharge, while higher resistance gives a smoother DC output. This is an important consideration in designing power supplies for circuits that require stable voltage.

## Files and Images
- Circuit simulation files are included in the `Circuit Files` folder  
- Simulation results are stored in the `Images` folder  
