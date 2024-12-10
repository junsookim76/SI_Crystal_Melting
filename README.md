# SI_Crystal_Melting

The list of folders and files included is as below.
 * Configuration files for simulations: (coordinates of DNA, water, ions)
   - folder name: config_prod
   - files:
       circ(70,76,82,90)_lin32_set(1,2,3,4)init.gro
       circ(70,76,82,90)_lin32_set(1,2,3,4)final.gro
 * MD parameters: (parameters for MD simulation)
   - folder name: mdp
   - files:
       grompp.mdp
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
