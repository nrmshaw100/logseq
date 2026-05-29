### Ardupilot method
	- ardupilot relies on their extended Kalman Filter
		- Filter model:
		  $$\mathbf{x_k} = f(\mathbf{x}_{k-1}, u_{k-1}) + \mathbf{w}_{k-1} \\
		  \mathbf{z_k} = h(\mathbf{x}_{k}) + \mathbf{v}_{k} $$
		- rotor momentum drag is proportional to speed, tends to be dominant drag term (as opposed to bluff body drag)
		-