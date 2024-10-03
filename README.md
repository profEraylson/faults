Datasets used in the paper 'Improving Fault Classification in Electrical Power Systems Using Multiple Classifier Systems'

The first dataset, referred to here as Dataset 1, was generated using ATPDraw software (https://www.atpdraw.net/). This dataset simulates the 138 kV section of a substation, including two transmission lines connected to the substation bus. Each line was considered as a load of 36 MW and 18 Mvar. Various types of faults were simulated between circuit breakers and line outputs, covering phase-to-ground, phase-to-phase, phase-to-phase-to-ground, and three-phase faults. Current measurements were taken at the transformer connection breaker on the main bus and at the line connection breakers sharing the same bus. Additionally, the voltage at the line outputs was measured. The simulation lasted 200 seconds, with data collected at 0.01-second intervals, resulting in a database of 20,000 samples. This database is structured as follows: the features columns represent voltage measurements at the outputs of the two lines for phases A, B, and C. Following these columns are current measurements in the circuit above the circuit breakers.
The classes are categorized as follows:
* Class 0: No faults
* Class 1: Phase-to-ground faults
* Class 2: Phase-to-phase faults
* Class 3: Phase-to-phase-to-ground faults
* Class 4: Three-phase faults


The second dataset (referred to as Dataset 2), derived from https://github.com/leandroensina/FADbF, was adapted to include only the energy variables of current and voltage signals, along with their Root Mean Square (RMS) values. As the system is three-phase, the final database contains twelve attributes and two variables that can be used as targets: fault location and fault type. The first is used to locate where the fault occurred and has discrete values between 4.14 and 414, each representing a distance in kilometers. The second variable has categorical values indicating the phases in which the fault occurred, such as AB, BC, and BG. In the present work, fault type was used as the target. The classes are categorized as follows:
* Class 0: Fault AB
* Class 1: Fault ABC
* Class 2: Fault ABG
* Class 3: Fault AC
* Class 4: Fault ACG

