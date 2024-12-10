# SI_Crystal_Melting

The list of folders and files included is as below.
 * Configuration files for GROMACS simulations: (coordinates of nitromethane and acetic acid): *.gro
   - folder name: CONFIG\_{REFCODE}\_{FORCEFIELD}\_INIT
   - file name:
       {REFCODE}\_{FORCEFIELD}\_{XYZ}\_{TEMP}K\_init.gro

	REFCODE: NTROMA01 for nitromethane or ACETAC07 for acetic acid
	FORCEFIELD: CGenFF, GAFF, GAFF2, OPLS 1.14\*CM1A, OPLS 1.14\*CM1A-LBCC
	XYZ: x or y or z for x-oriented or y-oriented, or z-oriented systems
	TEMP: temperature values within the ranges considered in our publication
     
 * MD parameters: (parameters for MD simulation): *.mdp
   - folder name: mdp_NTROMA01_CGenFF_init
   - files:
       NTROMA01_CGenFF_x_200K_grompp.mdp
       NTROMA01_CGenFF_x_205K_grompp.mdp
       NTROMA01_CGenFF_x_210K_grompp.mdp
       NTROMA01_CGenFF_x_215K_grompp.mdp
       NTROMA01_CGenFF_x_220K_grompp.mdp
       NTROMA01_CGenFF_y_200K_grompp.mdp
       NTROMA01_CGenFF_y_205K_grompp.mdp
       NTROMA01_CGenFF_y_210K_grompp.mdp
       NTROMA01_CGenFF_y_215K_grompp.mdp
       NTROMA01_CGenFF_y_220K_grompp.mdp
       NTROMA01_CGenFF_z_200K_grompp.mdp
       NTROMA01_CGenFF_z_205K_grompp.mdp
       NTROMA01_CGenFF_z_210K_grompp.mdp
       NTROMA01_CGenFF_z_215K_grompp.mdp
       NTROMA01_CGenFF_z_220K_grompp.mdp
     
 * Topology inputs: (topology files - *.topol, *.itp)
   - folder name: topology
   - files and subfolders:
       circ(70,76,82,90)_lin32_topol.top
       topol_(circular, linear)_DNA_chain_(A,B).itp 
   - files for weak restraints in each subfolders
       posre_linear_DNA_chain_(A3,B3).itp 
  * Configuration files for analysis and visualization: (coordinates of DNA and ions)
    - folder name: trajectory_for_visualization
    - files:
       circ(70,76,82,90)_lin32_set(1,2,3,4)_init_DNAion.gro 
 	     circ(70,76,82,90)_lin32_set(1,2,3,4)_DNAion_dt10ns.xtc 
  * Movies: (movie of one trajectory for each DNA rotaxane)
    - folder name: movie_files
    - files:
		   rotax_70_3.mpg 
		   rotax_76_3.mpg 
		   rotax_82_1.mpg 
 		   rotax_90_1.mpg
    - We've observed that "QuickTime Player" on Mac might encounter difficulties in playing the movies. We suggest experimenting with alternative media players, such as GOM Player or VLC Media Player.
