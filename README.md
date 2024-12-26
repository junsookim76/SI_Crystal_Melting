># SI_Crystal_Melting

>Supporting Data 
>
>for "Melting point prediction of organic crystals using direct molecular dynamics simulations" 
>
>by Chi, Han, Won, and Kim (2025)

The list of folders and files included is as below.
## Configuration files for GROMACS simulations: *.gro
   - **folder name**: {REFCODE}\_{FORCEFIELD}\_{SYSTEM}
   - **file name**:
       conf\_{XYZ}\_{TEMP}K.gro
   - **file name for CONTHEAT**:
       conf\_{XYZ}\_{TIME}ps.gro
     
	- REFCODE: NTROMA01 (for nitromethane) or ACETAC07 (for acetic acid)
	- FORCEFIELD: CGenFF, GAFF, GAFF2, OPLS_CM1A (for OPLS 1.14*CM1A), OPLS_LBCC (for OPLS 1.14*CM1A-LBCC)
 	- SYSTEM: S (for solid alone), LS (for liquid/solid), VLSV (for vapor/liquid/solid/vapor), 
  		VSV (for vapor/solid/vapor), CONTHEAT (for continuous heating)
	- XYZ: x (for x-oriented systems) or y (for y-oriented systems), or z (for z-oriented systems)
	- TEMP: temperature values within the ranges considered in our publication
	- TIME: simulatio times within the durations considered in our publication

	- example folder: NTROMA01_CGenFF_VLSV
 	- example file: conf_x_200K.gro
     
## MD simulation parameters: *.mdp
   - **file name**:
       grompp\_{XYZ}\_{TEMP}K.mdp
   - **file name for CONTHEAT**:
       grompp\_{XYZ}\_{TIME}ps.mdp

 	- example file: grommp_x_200K.mdp

## Topology inputs: *.topol, *.itp, *.ff
   - **file name for CGenFF NTROMA01**:
   - topol.top / ntma.itp / ntma.prm / charmm36-jul2022.ff
   - **file name for CGenFF ACETAC07**:
   - topol.top / charmm36.ff
   - **file name for GAFF NTROMA01**:
   - topol.top / NTRIMA01_SINGLE_GMX_gaff.itp
   - **file name for GAFF ACETAC07**:
   - topol.top / acooh01_GAFF0.itp
   - **file name for GAFF2 NTROMA01**:
   - topol.top / NTMA_GAFF2.itp
   - **file name for GAFF2 ACETAC07**:
   - topol.top / ACETAC07.itp
   - **file name for OPLS 1.14*CM1A NTROMA01**:
   - topol.top / nitromethane_1.itp
   - **file name for OPLS 1.14*CM1A ACETAC07**:
   - topol.top / AC07_CM1A.itp
   - **file name for OPLS 1.14*CM1A-LBCC NTROMA01**:
   - topol.top / nitromethane_1.itp
   - **file name for OPLS 1.14*CM1A-LBCC ACETAC07**:
   - topol.top / AC07_LBCC.itp


## Potential energy as a function of time: *.xvg 
   - **file name**:
       potener\_{XYZ}\_{TEMP}K.xvg
   - **file name for CONTHEAT**:
       potener\_{XYZ}\_{TIME}ps.xvg

## Representative Movies: 

   - Crystal Growth and Melting Using CGenFF (Solid/Liquid)
   - **folder name**: MOVIES
   - **file name**:
       CGenFF\_{SL}\_{X}\_{TEMP}K.mpg

    - We've observed that "QuickTime Player" on Mac might encounter difficulties in playing the movies. We suggest experimenting with alternative media players, such as GOM Player or VLC Media Player.
