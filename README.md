# hp_foldamers
Project for PHYS 230 at University of  California, Merced

This project, inspired by the work of Guseva et al. (1), uses the Gillespie algorithm to investigate the kinetics of the growth of hydrophobic-polar (HP) polymers of hydrophobic and polar monomers. In particular, we are interested in the effect of catalysis that might be provided by HP "foldamers" (folded HP polymers) with hydrophobic "landing pads" three or more residues long that may transiently bond with the hydrophobic end of a growing chain and with a hydrophobic monomer, stabilizing the chain and the monomer in position and thereby increasing the reaction rate associated with the addition of the monomer to the chain. The Guseva paper proposes that such catalysis may have been an important factor in the early evolution of biomolecules.

Part 1

display_hp_foldamer produces a graphical representation of the best configuration of an HP foldamer as determined by the simulated annealing program modelo2 by Hania Kranas (2). It takes a trajectory file produced by modelo2 as input.

get_landing_pad_length determines the length of the best catalytic hydrophobic "landing pad" as described by Guseva et al. (1) on the outside of the best configuration of an HP foldamer as determined by modelo2. It takes a trajectory file produced by modelo2 as input.

The trajectory file produced by a modelo2 simulated annealing process is traj.pdb. I have provided two such files (renamed based on the polymer being simulated) for use in running the example trials I have included in the Jupyter notebook. Those files should be placed in the same directory as the Jupyter notebook.

Part 2

hp_gillespie_simulation simulates the polymerization of hydrophobic (H) and polar (P) monomers as described by Guseva et al. using the Gillespie algorithm (3), which incorporates a Monte Carlo step into the choice of the next reaction and the time interval before the next reaction. Simulations can be run with or without a rate boost due to "catalysis" for the addition of hydrophobic monomers to growing chains with hydrophobic ends capable of transiently binding to catalytic "landing pads" on catalytic foldamers that are assumed to exist in the system. (The assumption of catalytic foldamers in the system is different from the simulations described in the Guseva paper, in which foldamers are produced by polymerization in the course of the simulations.) The state of the system is stored at intervals so that the time evolution of the system can be observed.

References:

1. E. Guseva et al., Foldamer hypothesis for the growth and sequence differentiation of prebiotic polymers, PNAS, 2017.

2. H. Kranas, HP model simulation, https://github.com/hansiu/modelo2-HPmodelSimulation, 2016.

3. D. Gillespie, Exact stochastic simulation of coupled chemical reactions, Journal of Chemical Physics, 1977.
