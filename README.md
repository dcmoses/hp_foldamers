# hp_foldamers
Project for PHYS 230 at University of  California, Merced

Part 1

display_hp_foldamer produces a graphical representation of the best configuration of an HP foldamer as determined by the simulated annealing program modelo2 by Hania Kranas https://github.com/hansiu/modelo2-HPmodelSimulation.

get_landing_pad_length determines the length of the best catalytic hydrophobic "landing pad" as described by Guseva et al. (PNAS, 2017) on the outside of the best configuration of an HP foldamer as determined by modelo2.

The file produced by modelo2 is traj.pdb. I have provided two such files (renamed based on the polymer being simulated) for use in running my example trials.

Part 2

hp_gillespie_simulation simulates the polymerization of hydrophobic (H) and polar (P) monomers as described by Guseva et al. using the Gillespie algorithm (J Chem Phys, 1977).

References/Sources:
E. Guseva et al., Foldamer hypothesis for the growth and sequence differentiation of prebiotic polymers, PNAS, 2017.
H. Kranas, HP model simulation, github.com/hansiu/modelo2-HPmodelSimulation, 2016.
D. Gillespie, Exact Stochastic Simulation of Coupled Chemical Reactions, Journal of Chemical Physics, 1977.
