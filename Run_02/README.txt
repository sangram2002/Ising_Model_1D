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
	
