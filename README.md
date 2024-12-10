# SI_Crystal_Melting

The list of folders and files included is as below.
 * Configuration files for simulations: (coordinates of nitromethane and acetic acid): *.gro
   - folder name: config_NTROMA01_CGenFF_init (CGenFF for nitromethane)
   - files:
     
       NTROMA01_CGenFF_x_200K_init.gro/
       NTROMA01_CGenFF_x_205K_init.gro/
       NTROMA01_CGenFF_x_210K_init.gro/
       NTROMA01_CGenFF_x_215K_init.gro/
       NTROMA01_CGenFF_x_220K_init.gro/
       NTROMA01_CGenFF_y_200K_init.gro/
       NTROMA01_CGenFF_y_205K_init.gro/
       NTROMA01_CGenFF_y_210K_init.gro/
       NTROMA01_CGenFF_y_215K_init.gro/
       NTROMA01_CGenFF_y_220K_init.gro/
       NTROMA01_CGenFF_z_200K_init.gro/
       NTROMA01_CGenFF_z_205K_init.gro/
       NTROMA01_CGenFF_z_210K_init.gro/
       NTROMA01_CGenFF_z_215K_init.gro/
       NTROMA01_CGenFF_z_220K_init.gro/
   - folder name: config_NTROMA01_GAFF_init (GAFF for nitromethane)
   - files:
       NTROMA01_GAFF_x_200K_init.gro
       NTROMA01_GAFF_x_205K_init.gro
       NTROMA01_GAFF_x_210K_init.gro
       NTROMA01_GAFF_x_215K_init.gro
       NTROMA01_GAFF_x_220K_init.gro
       NTROMA01_GAFF_y_200K_init.gro
       NTROMA01_GAFF_y_205K_init.gro
       NTROMA01_GAFF_y_210K_init.gro
       NTROMA01_GAFF_y_215K_init.gro
       NTROMA01_GAFF_y_220K_init.gro
       NTROMA01_GAFF_z_200K_init.gro
       NTROMA01_GAFF_z_205K_init.gro
       NTROMA01_GAFF_z_210K_init.gro
       NTROMA01_GAFF_z_215K_init.gro
       NTROMA01_GAFF_z_220K_init.gro
       
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
