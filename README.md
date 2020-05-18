# hp_foldamers
Project for PHYS 230 at University of  California, Merced

This project, inspired by the work of Guseva et al. (PNAS, 2017), uses the Gillespie algorithm to investigate the kinetics of the growth of hydrophobic-polar (HP) polymers of hydrophobic and polar monomers. In particular, we are interested in the effect of catalysis that might be provided by HP "foldamers" (folded HP polymers) with hydrophobic "landing pads" three or more residues long that may transiently bond with hydrophobic ends of growing chains and stabilize them in position, thereby increasing the reaction rate associated with further polymerization.

Part 1

display_hp_foldamer produces a graphical representation of the best configuration of an HP foldamer as determined by the simulated annealing program modelo2 by Hania Kranas (https://github.com/hansiu/modelo2-HPmodelSimulation).

get_landing_pad_length determines the length of the best catalytic hydrophobic "landing pad" as described by Guseva et al. (PNAS, 2017) on the outside of the best configuration of an HP foldamer as determined by modelo2.

The file produced by modelo2 is traj.pdb. I have provided two such files (renamed based on the polymer being simulated) for use in running my example trials. They should be placed in the same directory as the Jupyter notebook.

Part 2

hp_gillespie_simulation simulates the polymerization of hydrophobic (H) and polar (P) monomers as described by Guseva et al. using the Gillespie algorithm (J Chem Phys, 1977).

References/Sources:

E. Guseva et al., Foldamer hypothesis for the growth and sequence differentiation of prebiotic polymers, PNAS, 2017.

H. Kranas, HP model simulation, github.com/hansiu/modelo2-HPmodelSimulation, 2016.

D. Gillespie, Exact stochastic simulation of coupled chemical reactions, Journal of Chemical Physics, 1977.
