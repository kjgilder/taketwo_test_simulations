# taketwo_test_simulations
Single, multi, and mode-selector simulation test files


## multi folder:
### `constant_leader.slx`: 
We adjusted the a0, v0, and x0 constants for both leader and ego to test different scenarios (including leader stationary)
  
Tests with this controller:
* Regular Leader with Constant Speed
* Stand-Still Leader
* No Leader

### `oscillating_leader.slx`: 
The leader's acceleration input is a sine wave, and we adjusted the amplication and frequency of this wave to test different leader behaviors

Tests with this controller:
* Smooth Leader Oscillations
* Steep Leader Oscillations
  

