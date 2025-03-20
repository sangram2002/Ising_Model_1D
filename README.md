We study the one-dimensional Ising model by simulating it using Metropolis algo-
rithm. We measure the observables such as the average energy, magnetization, spe-
cic heat, susceptibility, and spin-spin correlator. Our results indicate the occurrence
of a second-order ferromagnetic phase transition. We nd the critical temperature
for the phase transition. We also simulate the one-dimensional Ising model but no
indication of phase transition is found from the simulations. Overall, our computed
results are in excellent agreement with the analytical results.

RUN 1 DATA

	# Define the parameters
	n_spins = 200
	spin_set = [-1.0, 1.0]
	timesteps = 250
	beta = 1.0
	n = 100 # Number of thermalized microstates to consider.
	J0 = 15.0
	 going from beta = 0.01 to beta = 3.0 in steps of 0.05
	 storing per spin data
	 Optimal Timesteps plot attached (energy v/s timesteps)
	 
	 Feedback: Cv, X not fitting well. Trying J0 = 1.0 next.
	
RUN 2 DATA

	# Define the parameters
	n_spins = 200
	spin_set = [-1.0, 1.0]
	timesteps = 250
	beta = 1.0
	n = 100 # Number of thermalized microstates to consider.
	
	J0 = 1.0
	 going from beta = 0.01 to beta = 3.0 in steps of 0.05
	 storing per spin data
	 Optimal Timesteps plot attached (energy v/s timesteps)
	 
	 Feedback: Cv, X fitting better. trying doubling number of spins next for better agreement. Optimal timesteps plot not helpful, seems like thermalization has already happend at zero timesteps (hot start!).

 RUN 3 DATA

	# Define the parameters
	n_spins = 400
	spin_set = [-1.0, 1.0]
	timesteps = 250
	beta = 1.0
	n = 100 # Number of thermalized microstates to consider.
	
	J0 = 1.0
	 going from beta = 0.01 to beta = 3.0 in steps of 0.05
	 storing per spin data
	 Optimal Timesteps plot attached (energy v/s timesteps)
	 
	 Feedback: Cv indeed fitting better. Doubling did make a significant improvement for Cv but not for X(?). Not sure what is going on there. Maybe at low temperatures the effects accumulate faster in magnetization? After all, for energy the deviation goes down but for magnetization the std increases with beta, causing worse fit for large beta. Took about 700 mins to run for 400 spins.
	 
	 RUN04 idea: Maybe introduce a small (1e-3) magnetic field and see if the deviation can be controlled? 
	
RUN 4 DATA

	# Define the parameters
	n_spins = 400
	spin_set = [-1.0, 1.0]
	timesteps = 250
	beta = 1.0
	n = 100 # Number of thermalized microstates to consider.


	J0 = 1.0 # The coupling constant is 1.
	H0 = 0.5 # The effect of magnetic field is now included.
	 going from beta = 0.01 to beta = 3.0 in steps of 0.05
	 storing per spin data
	 Optimal Timesteps plot attached (energy v/s timesteps)
	 
	 Feedback: h stabilizes the system well. While the stds. get too small, the fit of the magnetization and the susceptibility to the data is good. The schottky curve is observed in heat capcity, but we found no analytic expressions for it, so we did not compare it.
	

