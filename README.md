# Ribosome Chemical Modification Files
This repository contains:
1) the PDB coordinate files for:  
    a) 70s ribosome (7k00.pdb)  
    b) pseudouridine (psuFH.pdb)  
    c) 3-methyl-pseudouridine (3tdFH.pdb)  
    d) 2-metyl-adenine (2ma.namd.pdb)  
    e) 5-hydroxyl-cytosine (c-7k00-5ocFH.pdb)  
2) The corresponding .vmd files for visualization in [VMD](https://www.ks.uiuc.edu/Research/vmd/).
3) The .tga image files generated using [Pov-Ray 3.6](https://www.povray.org/download/linux.php). 

## Detailed Notes:
- 7k00.pdb was downloaded from the [PDB](https://www.rcsb.org/structure/7k00) and is unaltered.
- psuFH.pdb and 3tdFH.pdb were based from the coordinates found in 7k00.pdb and the hydrogens were automatically generated using the [hydrogen adding server](http://molprobity.biochem.duke.edu/).
- 2ma.namd.pdb was based from the coordinates found in 7k00.pdb and the hydrogens were generating using VMD with the [CHARMM36 force field](http://mackerell.umaryland.edu/charmm_ff.shtml#charmm) with the enclosed scripts in setup/2ma/. The hydrogen adding server erroneously placed only one hydrogen on an amino group when there should have been two.
- c-7k00-5ocFH.pdb is 5-hydroxyl-cytosine that was modeled based on the C 2501 coordinates in 7k00.pdb and the 5-hydroxymethyl-cytosine coordinates in [4hli.pdb](https://www.rcsb.org/structure/4HLI), then adding the hydrogens using the hydrogen adding server. The CHARMM36 force field does not have 5-hydroxyl-cytosine.
