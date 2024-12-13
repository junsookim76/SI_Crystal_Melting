># SI_Crystal_Melting

>Supporting Data 
>
>for "Melting point prediction of organic crystals using direct molecular dynamics simulations" 
>
>by Chi, Han, Won, and Kim (2025)

The list of folders and files included is as below.
## Configuration files for GROMACS simulations: *.gro
   - **folder name**: CONFIG\_INIT\_{REFCODE}\_{FORCEFIELD}\_{SYSTEM}
   - **file name**:
       conf\_{XYZ}\_{TEMP}K.gro

	- REFCODE: NTROMA01 (for nitromethane) or ACETAC07 (for acetic acid)
	- FORCEFIELD: CGenFF, GAFF, GAFF2, OPLS 1.14*CM1A, OPLS 1.14*CM1A-LBCC
 	- SYSTEM: S (for solid alone), LS (for liquid/solid), VLSV (for vapor/liquid/solid/vapor), 
  		VSV (for vapor/solid/vapor), CONTHEAT (for continuous heating)
	- XYZ: x (for x-oriented systems) or y (for y-oriented systems), or z (for z-oriented systems)
	- TEMP: temperature values within the ranges considered in our publication

	- example folder: CONFIG_INIT_NTROMA01_CGenFF_VLSV
 	- example file: NTROMA01_CGenFF_x_200K_init.gro
     
## MD simulation parameters: *.mdp
   - **folder name**: MDP\_{REFCODE}\_{FORCEFIELD}\_{SYSTEM}
   - **file name**:
       grompp\_{XYZ}\_{TEMP}K.mdp

	- example folder: MDP_NTROMA01_CGenFF_VLSV
 	- example file: NTROMA01_CGenFF_x_200K_grompp.mdp

## Topology inputs: *.topol, *.itp, *.ff
   - **folder name**: TOPOLOGY\_{REFCODE}\_{FORCEFIELD}
   - **file name for CGenFF NTROMA01**:
   - topol.top / ntma.itp / ntma.prm / charmm36-jul2022.ff
   - **file name for CGenFF ACETAC07**:
   - topol.top / charmm36.ff
   - **file name for GAFF**:
   - topol.top / NTROMA01_SINGLE_GMX_gaff.itp 
   - **file name for GAFF2**:
   - **file name for OPLS 1.14*CM1A**:
   - **file name for OPLS 1.14*CM1A-LBCC**:
     
## Energy outputs for calculation of potential energy: *.edr 
   - **folder name**: ENER\_{REFCODE}\_{FORCEFIELD}\_{SYSTEM}
   - **file name**:
       ener\_{XYZ}\_{TEMP}K.edr

## Potential energy as a function of time: *.xvg 
   - **folder name**: POTENER\_{REFCODE}\_{FORCEFIELD}\_{SYSTEM}
   - **file name**:
       potener\_{XYZ}\_{TEMP}K.xvg

## Representative Movies: 

   - Crystal Growth and Melting Using CGenFF (Solid/Liquid)
   - **folder name**: MOVIES
   - **file name**:
       potener\_{XYZ}\_{TEMP}K.xvg

    - We've observed that "QuickTime Player" on Mac might encounter difficulties in playing the movies. We suggest experimenting with alternative media players, such as GOM Player or VLC Media Player.
