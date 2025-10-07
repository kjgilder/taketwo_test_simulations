# taketwo_test_simulations
Single, multi, and mode-selector simulation test files

# single folder:
### `single_sim.slx`:
We adjusted values of x0, v0, and sn to test:
* Stopped with No Leader
* Stopped with Sn = 0
* No Leader
* Small Space Gap
* Larger Space Gap

# multi folder:
Note: we used the Test Manager in MatLab and a variable block to run these different scenarios on all modes
### `constant_leader_sim.slx`: 
We adjusted the a0, v0, and x0 constants for both leader and ego to test different scenarios (including leader stationary)
  
Tests with this controller:
* Regular Leader with Constant Speed
* Stand-Still Leader
* No Leader

### `oscillating_leader_sim.slx`: 
The leader's acceleration input is a sine wave, and we adjusted the amplication and frequency of this wave to test different leader behaviors

Tests with this controller:
* Smooth Leader Oscillations
* Steep Leader Oscillations
  

### `random_leader_sim.slx`:
We created random leader behavior by using a band-limited white noise block (with transfer function and saturation) to test how ego reacts

Tests with this controller:
* Random Leader Behavior


### `switching_leader_sim.slx`:
We added a switch and step to switch between having a leader and no leader (simulated with a very large space gap)

Tests with this controller:
* Leader leaves during simulation
* Leader enters during simulation

# mode folder:

### `mode_sim.slx`:
We created several different inputs with the same mode selector controller and tracked whether the mode updates correctly and timely.

Tests:
* Detecting Smooth Leader
* Detecting Erratic Leader
* Detecting Changing Behavior from *Same* Leader
* Detecting Leader Entering
* Detecting Leader Exiting
* Detecting *Different* Leader


