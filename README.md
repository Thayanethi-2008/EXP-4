# EXPERIMENT NO. 4 – HALF WAVE AND FULL WAVE BRIDGE RECTIFIERS

| **Name:** | | **Reg. No.:** | |
|---|---|---|---|
| **Date:** | | **Batch / Section:** | |

---

## AIM

To study the half wave and full wave bridge rectifiers with and without filter and to observe their input and output waveforms using Proteus.

## COMPONENTS AND EQUIPMENT REQUIRED

| S. No. | Components / Equipment |
|:---:|:---|
| 1 | Diodes |
| 2 | Resistor (load) |
| 3 | Capacitors (filter) |
| 4 | Step-down transformer |
| 5 | Voltmeter |
| 6 | Ammeter |
| 7 | Breadboard |
| 8 | CRO |
| 9 | Connecting wires |
| 10 | Simulation software – Proteus Design Suite |

## THEORY

A rectifier changes AC to DC and is an essential part of a power supply. The unique property of a diode, permitting current to flow in only one direction, is utilised in rectifiers.

### Half wave rectifier

Mains supply is applied to the primary of the step-down transformer. All the positive half cycles of the stepped-down AC supply pass through the diode and all the negative half cycles are eliminated. The peak value of the output voltage is less than the peak value of the input voltage by about 0.6 V because of the voltage drop across the diode. For a half wave rectifier, **Vrms = Vm/2** and **Vdc = Vm/π**, where Vrms is the RMS value of the output, Vdc is the average value of the output and Vm is the peak value of the output.

### Full wave bridge rectifier

During the positive half cycle of the secondary voltage, diodes D1 and D3 are forward biased and D2 and D4 are reverse biased, so current flows through the secondary winding, D1, the load resistor and D3. During the negative half cycle, D2 and D4 are forward biased and D1 and D3 are reverse biased, so current flows through the secondary winding, D2, the load resistor and D4. In both half cycles the current through the load resistor is in the same direction. The peak output voltage is less than the peak input voltage by about 1.2 V due to the drop across two diodes. For a full wave bridge rectifier, **Vrms = Vm/√2** and **Vdc = 2Vm/π**.

### Filters

All rectifier outputs contain a considerable amount of ripple in addition to the DC component. To remove the AC components, a filter is connected at the output of the rectifier. Capacitor input, choke input, RC, CRC, LC and CLC filters are commonly used; the capacitor input filter is the simplest and cheapest. A high-value capacitor C is connected in shunt with the load resistor RL. The capacitor charges to the peak voltage when a half cycle appears at the output. After the peak, the capacitor discharges slowly through RL, since the diode is reverse biased by the capacitor voltage. Before the capacitor voltage drops substantially, the next output cycle arrives and the capacitor recharges to the peak.

## PROCEDURE

1. Wire up the half wave rectifier circuit without capacitor after testing all the components.
2. Switch on the mains supply. Observe the transformer secondary voltage waveform and the output voltage waveform across the load resistor simultaneously on the CRO.
3. Connect the capacitor filter across the load and observe the waveforms. Repeat for different capacitor values.
4. Repeat the above steps for the full wave bridge rectifier.
5. Simulate both rectifiers, with and without filter, in Proteus and capture the input and output waveforms on the virtual oscilloscope.

## CIRCUIT DIAGRAMS

### Half wave rectifier without filter

<img width="1600" height="952" alt="WhatsApp Image 2026-11-24 at 7 40 19 PM" src="https://github.com/user-attachments/assets/2cf780ef-ea62-40f4-9e79-be21760be79f" />



### Half wave rectifier with filter

<img width="1600" height="919" alt="WhatsApp Image 2026-11-24 at 7 40 28 PM" src="https://github.com/user-attachments/assets/0e9bf792-957f-4592-b53c-cb179625c4d4" />



### Full wave bridge rectifier without filter

<img width="1600" height="815" alt="WhatsApp Image 2026-11-24 at 7 43 45 PM" src="https://github.com/user-attachments/assets/a0793ff9-c52f-4dc0-8d9c-b6dfefabfb2e" />


### Full wave bridge rectifier with filter

<img width="1599" height="1092" alt="WhatsApp Image 2026-11-24 at 7 43 52 PM" src="https://github.com/user-attachments/assets/01df93a0-39e0-454d-8734-b010d9fb230b" />


## SIMULATION AND WAVEFORMS USING PROTEUS

Build each rectifier in Proteus, with and without the capacitor filter. Use the virtual oscilloscope to display the input (secondary) and output waveforms together, and paste the screenshots below.

### Half wave rectifier

<img width="1082" height="695" alt="WhatsApp Image 2026-11-23 at 11 42 44 PM" src="https://github.com/user-attachments/assets/3a3117bd-5745-4b0f-82ad-f5dd3e91903c" />
<img width="1367" height="852" alt="WhatsApp Image 2026-11-23 at 11 42 40 PM" src="https://github.com/user-attachments/assets/f7cd23fe-8cd5-4623-9679-595038fb81fc" />


### Full wave bridge rectifier 

<img width="1106" height="705" alt="WhatsApp Image 2026-11-23 at 11 42 51 PM" src="https://github.com/user-attachments/assets/45ee33a2-bf0f-41a8-ae40-c9e9628f3594" />
<img width="1377" height="882" alt="WhatsApp Image 2026-11-23 at 11 42 47 PM" src="https://github.com/user-attachments/assets/6b0e0a51-2208-4f2a-8123-902cd2ae2498" />

## TABULATION AND MODEL GRAPH
<img width="1198" height="1600" alt="image" src="https://github.com/user-attachments/assets/37a94928-e823-47a1-a4c9-640803a7b4be" />
<img width="1229" height="1599" alt="image" src="https://github.com/user-attachments/assets/7391c73c-0e88-4e89-b3a6-ebb39f59bb7d" />

## FORMULAE

### A. Half wave rectifier

- Average (DC) voltage: **Vdc = Vm / π**
- Average (DC) current: **Idc = Im / π**
- RMS voltage: **Vrms = Vm / 2**
- RMS current: **Irms = Im / 2**
- Ripple factor: **γ = √[(Vrms / Vdc)² − 1] = 1.21**
- Rectification efficiency: **η = Pdc / Pac × 100 = (Idc² RL) / (Irms² RL) × 100 = 40.6 %**
- Form factor: **FF = Vrms / Vdc = 1.57**
- Peak factor: **PF = Vm / Vrms = 2**
- Peak inverse voltage: **PIV = Vm**

### B. Full wave bridge rectifier

- Average (DC) voltage: **Vdc = 2Vm / π**
- Average (DC) current: **Idc = 2Im / π**
- RMS voltage: **Vrms = Vm / √2**
- RMS current: **Irms = Im / √2**
- Ripple factor: **γ = √[(Vrms / Vdc)² − 1] = 0.482**
- Rectification efficiency: **η = Pdc / Pac × 100 = (Idc² RL) / (Irms² RL) × 100 = 81.2 %**
- Form factor: **FF = Vrms / Vdc = 1.11**
- Peak factor: **PF = Vm / Vrms = √2 = 1.414**
- Peak inverse voltage: **PIV = Vm**

### C. With capacitor filter

- Half wave: **γ = 1 / (2√3 f C RL)**
- Full wave bridge: **γ = 1 / (4√3 f C RL)**

### D. Regulation

- **% Regulation = (VNL − VFL) / VFL × 100**

Vm – peak output voltage; Im – peak load current (Im = Vm / RL); RL – load resistance; f – supply frequency (50 Hz); C – filter capacitance; VNL – no-load voltage; VFL – full-load voltage.

## RESULT

Thus, the input and output waveforms of the half wave and full wave bridge rectifiers with and without filter were observed using Proteus.
