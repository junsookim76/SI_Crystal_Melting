## List of Folders and Files

Below is a summary of the folder and file structure used in this repository.

---

### **Folder name**: `{REFCODE}_{FORCEFIELD}_{SYSTEM}`

- **REFCODE**:  
        - `NTROMA01` (for nitromethane)  
        - `ACETAC07` (for acetic acid)
- **FORCEFIELD**:  
        - `CGenFF`, `GAFF`, `GAFF2`, `OPLS 1.14*CM1A`, `OPLS 1.14*CM1A-LBCC`
- **SYSTEM**:  
        - `S` (solid alone)  
        - `LS` (liquid/solid)  
        - `VLSV` (vapor/liquid/solid/vapor)  
        - `VSV` (vapor/solid/vapor)  
        - `CONTHEAT` (continuous heating)

---
### Configuration files for GROMACS simulations: *.gro

#### **File name**: 
    - conf_{XYZ}_{TEMP}K.gro
    - conf_{XYZ}_{TIME}ps.gro (for CONTHEAT)

- **XYZ**:  
        - `x`, `y`, `z` (for different orientations)
- **TEMP**:  
        - Temperature values within the ranges considered in our publication   
- **TIME**:   
        - Simulation times within the durations considered in our publication

---  
### MD Simulation Parameters: *.mdp

#### **File name**:  
    - grompp_{XYZ}_{TEMP}K.mdp  
    - grompp_{XYZ}_{TIME}ps.mdp (for CONTHEAT)

#### **Example file**:  
    - grommp_x_200K.mdp


---

### Topology Inputs: *.topol, *.itp, *.ff

#### **File name**:  
- **File name for CGenFF NTROMA01**  
  `topol.top / ntma.itp / ntma.prm / charmm36-jul2022.ff`
- **File name for CGenFF ACETAC07**  
  `topol.top / charmm36.ff`
- **File name for GAFF NTROMA01**  
  `topol.top / NTROMA01_SINGLE_GMX_gaff.itp`
- **File name for GAFF ACETAC07**   
  `topol.top / acooh01_GAFF0.itp`   
- **File name for GAFF2 NTROMA01**  
  `topol.top / NTMA_GAFF2.itp`   
- **File name for GAFF2 ACETAC07**   
  `topol.top / ACETAC07.itp`   
- **File name for OPLS 1.14*CM1A NTROMA01**   
  `topol.top / nitromethane_1.itp`   
- **File name for OPLS 1.14*CM1A ACETAC07**   
  `topol.top / AC07_CM1A.itp`   
- **File name for OPLS 1.14*CM1A-LBCC NTROMA01**  
  `topol.top / nitromethane_1.itp`   
- **File name for OPLS 1.14*CM1A-LBCC ACETAC07**   
  `topol.top / AC07_LBCC.itp`


---

### **Potential Energy as a Function of Time**: `*.xvg`

#### **File name**:  
    - ener_{XYZ}_{TEMP}K.xvg  
    - ener_{XYZ}_{TIME}ps.xvg (for CONTHEAT)
---

### **Representative Movies**

#### **Folder name**: `NTROMA01_MOVIES`
#### **File name**:  
    - CGenFF_SL_X_{TEMP}K.mpg  

- **Crystal Growth and Melting Using CGenFF (Solid/Liquid)**  


---

> **Note**:  
> "QuickTime Player" on macOS may have difficulty playing these movie files.  
> We recommend using alternative media players such as **GOM Player** or **VLC Media Player**
