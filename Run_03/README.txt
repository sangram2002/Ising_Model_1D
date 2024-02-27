RUN 2 DATA

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
	
