<p align="right"><a href="#pt">🇧🇷 Português</a> · <a href="#en">🇺🇸 English</a></p>

<p align="center">
  <img src="assets/header.svg" width="100%" alt="Nicholas Seifert, UTFPR Campo Mourão: tela de osciloscópio com um seno e o PWM senoidal que ele modula">
</p>

<a id="pt"></a>

### Olá! Sou o Nicholas 👋

Engenheiro eletrônico formado pela **UTFPR – Campus Campo Mourão** (dez/2026),
com experiência em **compatibilidade eletromagnética (EMC)**. Tenho perfil
multidisciplinar e adaptativo: transito entre eletrônica de potência, circuitos
analógicos, sistemas embarcados e software, e gosto de entender cada bloco de
um CI até conseguir reproduzi-lo em simulação.

#### 〰️ [Gerador de formas de onda DDS em FPGA](https://github.com/nseiC/dds_waveform_generator) · TCC

<a href="https://github.com/nseiC/dds_waveform_generator">
  <img src="https://raw.githubusercontent.com/nseiC/dds_waveform_generator/main/docs/jogo/preview.svg" width="100%" alt="Animação do DDS: a roda de fase avança um passo M a cada clock e a LUT desenha um seno em degraus">
</a>

Gerador de sinais por **Síntese Digital Direta** feito do zero, do VHDL ao conector de saída.
Gera seno, rampa, sinc ou uma forma arbitrária (como um ECG sintético de 120 bpm), de 0 a
262 kHz com resolução de 2,33 mHz, com controle pelo PC via Virtual JTAG. Projeto em andamento.

| Parte | O que tem |
|---|---|
| [**Digital**](https://github.com/nseiC/dds_waveform_generator/tree/main/fpga) | VHDL na DE2-115 (Cyclone IV): acumulador de fase de 32 bits, PLL de 10 MHz, LUTs 1024 × 8, Virtual JTAG e testbench no GHDL |
| [**Analógica**](https://github.com/nseiC/dds_waveform_generator/tree/main/analog) | Placa própria com DAC0800, conversor I→V, filtro Sallen-Key de 1 MHz e saída push-pull; projeto no Altium e simulação no LTspice |
| [**Interface**](https://github.com/nseiC/dds_waveform_generator/tree/main/GUI) | GUI em Python que envia frequência, forma de onda e LUT arbitrária pelo USB-Blaster |

#### ⚡ [LTSpice-behavioral-IC-lib](https://github.com/nseiC/LTSpice-behavioral-IC-lib)

Biblioteca de macromodelos comportamentais de controladores de fontes
chaveadas para LTspice / ngspice, feitos a partir dos datasheets e notas de
aplicação dos fabricantes. Cada modelo vem com testes de regressão que conferem
o modelo contra as tabelas do datasheet e com exemplos em malha fechada.

| CI | Função | Exemplos |
|---|---|---|
| [**SG3524**](https://github.com/nseiC/LTSpice-behavioral-IC-lib/tree/main/SG3524) | controlador PWM | buck, boost, buck-boost inversor, push-pull |
| [**UC3854**](https://github.com/nseiC/LTSpice-behavioral-IC-lib/tree/main/UC3854) | PFC boost por corrente média | PFC de 250 W da U-134, FP 0,995 |
| [**L6599A**](https://github.com/nseiC/LTSpice-behavioral-IC-lib/tree/main/L6599A) | controlador ressonante LLC meia-ponte | LLC 12 V / 150 W da AN3233, burst, hiccup, fonte completa PFC + LLC |

#### 🛠️ Ferramentas

<p>
  <img alt="LTspice" src="https://img.shields.io/badge/LTspice-0B1626?style=flat-square">
  <img alt="ngspice" src="https://img.shields.io/badge/ngspice-0B1626?style=flat-square">
  <img alt="VHDL" src="https://img.shields.io/badge/VHDL-0B1626?style=flat-square">
  <img alt="Intel Quartus" src="https://img.shields.io/badge/Quartus-0B1626?style=flat-square&logo=intel&logoColor=FF9A3D">
  <img alt="Altium Designer" src="https://img.shields.io/badge/Altium%20Designer-0B1626?style=flat-square">
  <img alt="Python" src="https://img.shields.io/badge/Python-0B1626?style=flat-square&logo=python&logoColor=FF9A3D">
  <img alt="C" src="https://img.shields.io/badge/C-0B1626?style=flat-square&logo=c&logoColor=FF9A3D">
  <img alt="LaTeX" src="https://img.shields.io/badge/LaTeX-0B1626?style=flat-square&logo=latex&logoColor=FF9A3D">
  <img alt="Git" src="https://img.shields.io/badge/Git-0B1626?style=flat-square&logo=git&logoColor=FF9A3D">
</p>

#### 📫 Contato

<!-- coloque aqui seu LinkedIn / e-mail, se quiser -->

---

<a id="en"></a>

### Hi! I'm Nicholas 👋

Electronic engineer, graduated from **UTFPR – Campo Mourão Campus** (Federal
University of Technology – Paraná, Dec 2026), with experience in
**electromagnetic compatibility (EMC)**. I have a multidisciplinary and
adaptable profile: I move between power electronics, analog circuits, embedded
systems and software, and I like to understand every block of an IC until I can
reproduce it in simulation.

#### 〰️ [FPGA DDS waveform generator](https://github.com/nseiC/dds_waveform_generator) · undergraduate thesis

<a href="https://github.com/nseiC/dds_waveform_generator">
  <img src="https://raw.githubusercontent.com/nseiC/dds_waveform_generator/main/docs/jogo/preview.svg" width="100%" alt="DDS animation: the phase wheel advances by M every clock and the LUT draws a stepped sine">
</a>

A **Direct Digital Synthesis** signal generator built from scratch, from the VHDL to the output
connector. It generates sine, ramp, sinc or an arbitrary waveform (such as a synthetic 120 bpm ECG), from
0 to 262 kHz with 2.33 mHz resolution, controlled from the PC over Virtual JTAG. Work in progress.

| Part | What's inside |
|---|---|
| [**Digital**](https://github.com/nseiC/dds_waveform_generator/tree/main/fpga) | VHDL on the DE2-115 (Cyclone IV): 32-bit phase accumulator, 10 MHz PLL, 1024 × 8 LUTs, Virtual JTAG and a GHDL testbench |
| [**Analog**](https://github.com/nseiC/dds_waveform_generator/tree/main/analog) | Custom board with a DAC0800, I→V converter, 1 MHz Sallen-Key filter and push-pull output; designed in Altium, simulated in LTspice |
| [**Interface**](https://github.com/nseiC/dds_waveform_generator/tree/main/GUI) | Python GUI that sends frequency, waveform and the arbitrary LUT over the USB-Blaster |

#### ⚡ [LTSpice-behavioral-IC-lib](https://github.com/nseiC/LTSpice-behavioral-IC-lib)

A library of behavioural macromodels of switch-mode power supply controllers
for LTspice / ngspice, built from the manufacturers' datasheets and
application notes. Each model comes with regression tests that check it
against the datasheet tables, and with closed-loop examples.

| IC | Function | Examples |
|---|---|---|
| [**SG3524**](https://github.com/nseiC/LTSpice-behavioral-IC-lib/tree/main/SG3524) | PWM controller | buck, boost, inverting buck-boost, push-pull |
| [**UC3854**](https://github.com/nseiC/LTSpice-behavioral-IC-lib/tree/main/UC3854) | average-current-mode boost PFC | U-134 250 W PFC, PF 0.995 |
| [**L6599A**](https://github.com/nseiC/LTSpice-behavioral-IC-lib/tree/main/L6599A) | resonant LLC half-bridge controller | AN3233 12 V / 150 W LLC, burst, hiccup, complete PFC + LLC supply |

#### 🛠️ Tools

<p>
  <img alt="LTspice" src="https://img.shields.io/badge/LTspice-0B1626?style=flat-square">
  <img alt="ngspice" src="https://img.shields.io/badge/ngspice-0B1626?style=flat-square">
  <img alt="VHDL" src="https://img.shields.io/badge/VHDL-0B1626?style=flat-square">
  <img alt="Intel Quartus" src="https://img.shields.io/badge/Quartus-0B1626?style=flat-square&logo=intel&logoColor=FF9A3D">
  <img alt="Altium Designer" src="https://img.shields.io/badge/Altium%20Designer-0B1626?style=flat-square">
  <img alt="Python" src="https://img.shields.io/badge/Python-0B1626?style=flat-square&logo=python&logoColor=FF9A3D">
  <img alt="C" src="https://img.shields.io/badge/C-0B1626?style=flat-square&logo=c&logoColor=FF9A3D">
  <img alt="LaTeX" src="https://img.shields.io/badge/LaTeX-0B1626?style=flat-square&logo=latex&logoColor=FF9A3D">
  <img alt="Git" src="https://img.shields.io/badge/Git-0B1626?style=flat-square&logo=git&logoColor=FF9A3D">
</p>

#### 📫 Contact

<!-- add your LinkedIn / e-mail here if you like -->
