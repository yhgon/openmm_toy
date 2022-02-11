# log for 6hqv simulation 

## data preparation 
it takes 3 minutes
- 6hqv_A.pdb  (pdbfixer, select chain A, add missing atom)
- 6hqv_het.pdb ( add hydrogen)
- 6hqv_water.pdb ( add water pad 1nm) 

## exp01 1ns MD simulation to fix missing atom
- load 6hqv_het.pdb
- add water ( add water pad 1nm) 
- set 310 Kelvin
- initialize topo
- trajectory (csv per iter, PDB per 5k = 20psf) during 1ns. 
- finalize  topo

## exp02 40ns htMD simulation 
- add solvent(water + K+) 
- initial topo
- trajectory (csv, PDB)
- finalized topo

## exp03 1ms MD simulation
- initial topo
- trajectory
- finalized
