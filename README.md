# SI_Crystal_Melting

>Supporting Data 
>
>for "Melting point prediction of organic crystals using direct molecular dynamics simulations" 
>
>by Chi, Han, Won, and Kim (2025)

The list of folders and files included is as below.
## Configuration files for GROMACS simulations: *.gro
   - **folder name**: CONFIG\_INIT\_{REFCODE}\_{FORCEFIELD}\_{SYSTEM}
   - **file name**:
       {REFCODE}\_{FORCEFIELD}\_{XYZ}\_{TEMP}K\_init.gro

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
       {REFCODE}\_{FORCEFIELD}\_{XYZ}\_{TEMP}K\_grompp.mdp

	- example folder: MDP_NTROMA01_CGenFF_VLSV
 	- example file: NTROMA01_CGenFF_x_200K_grompp.mdp

## Topology inputs: (topology files - *.topol, *.itp)
   - folder name: TOPOLOGY\_{REFCODE}\_{FORCEFIELD}
   - files and subfolders:
       circ(70,76,82,90)_lin32_topol.top
       topol_(circular, linear)_DNA_chain_(A,B).itp 
   - files for weak restraints in each subfolders
       posre_linear_DNA_chain_(A3,B3).itp
     
## Energy outputs for calculation of potential energy: *.edr 
  * Configuration files for analysis and visualization: (coordinates of DNA and ions)
    - folder name: trajectory_for_visualization
    - files:
       circ(70,76,82,90)_lin32_set(1,2,3,4)_init_DNAion.gro 
 	     circ(70,76,82,90)_lin32_set(1,2,3,4)_DNAion_dt10ns.xtc

## Potential energy as a function of time: *.xvg 
  * Configuration files for analysis and visualization: (coordinates of DNA and ions)
    - folder name: trajectory_for_visualization
    - files:
       circ(70,76,82,90)_lin32_set(1,2,3,4)_init_DNAion.gro 
 	     circ(70,76,82,90)_lin32_set(1,2,3,4)_DNAion_dt10ns.xtc

## Movies
  * Movies: (movie of one trajectory for each DNA rotaxane)
    - folder name: movie_files
    - files:

    - We've observed that "QuickTime Player" on Mac might encounter difficulties in playing the movies. We suggest experimenting with alternative media players, such as GOM Player or VLC Media Player.
