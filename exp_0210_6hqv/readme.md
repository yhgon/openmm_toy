# log for 6hqv simulation 
- 6hqv_A.pdb  (pdbfixer, select chain A, add missing atom)
- 6hqv_het.pdb ( add hydrogen)
- 6hqv_water.pdb ( add water 0.1nm) 

## exp01 1ns MD simulation to fix missing atom
- load 6hqv_het.pdb
- add water 
- set 310 Kelvin
- initialize topo
- trajectory (csv, PDB)
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
