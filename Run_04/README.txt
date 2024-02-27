RUN 2 DATA

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
	
