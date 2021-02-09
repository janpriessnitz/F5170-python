### Exercise 1

Concentration (m<sup>-3</sup>) divided by time (s) gives the unit of m<sup>-3</sup>s<sup>-1</sup> . The unit of the rate constant must be m<sup>3</sup>s<sup>-1</sup> for a reaction involving two reactants and m<sup>6</sup>s<sup>-1</sup> for a reaction involving three reactants. In general, the unit of a rate constant for a reaction of N reactants is m<sup>3(N-1)</sup>s<sup>-1</sup>

### Exercise 2

According to the equation of state for ideal gas, the concentration of particles (regardless of the species) is N/V = p/(kT). Sum of all species' concentrations has to add up to this overall concentration: [Ar] + [Ar<sup>+</sup>] + [Ar<sup>\*</sup>] + [Ar<sup>+</sup><sub>2</sub>] = N/V = p/(kT). This gives us the actual concentration of ground state argon: [Ar] = p/(kT) - [Ar<sup>+</sup>] + [Ar<sup>\*</sup>] + [Ar<sup>+</sup><sub>2</sub>] .

Note: In the code, I saw that in the expression for concentration of ground-state Argon, concentration of Ar<sup>+</sup><sub>2</sub> is halved. This makes sense - if we set p/(kT) as an initial constant, we want to conserve the number of Argon atoms in the gas and Ar<sup>+</sup><sub>2</sub> actually consists of 2 atoms. However, in general, pressure of the gas should not be constant for constant number of atoms and volume. As the concentration of Ar<sup>+</sup><sub>2</sub> grows, the pressure should fall.

### Exercise 3

The unit of the constant is electronvolt, since it needs to cancel out with the temperature given in electronvolts.

The physical meaning of its constant is the excitation/ionization energy. More precisely, its the energy difference between the initial and final state of argon (reaction number 4 - energy difference between excitation state and ionization state).

I think that in cold gas, the main ionization channel will be reaction number 4 joined with reaction number 1. This channel will be mainly limited by the speed of reaction number 1, since the linear constant is a lot smaller and the energy difference is higher than that of reaction 4. However, it will still be faster than reaction number 3 with higher energy difference.

In hot gas, the high temperature will diminish the importance of the energy difference and reaction number 3 is going to be the fastest because of the larger linear constant. Reaction number 3 will then become the main ionization channel.

### Exercise 4

d[Ar<sup>\*</sup>]/dt = 1\*k<sub>1</sub>\*[e]\*[Ar] +
(-1)\*k<sub>2</sub>\*[e]\*[Ar<sup>\*</sup>] +
(-1)\*k<sub>4</sub>\*[e]\*[Ar<sup>\*</sup>] +
1\*k<sub>6</sub>\*[e]\*[Ar<sup>+</sup><sub>2</sub>] +
(-2)\*k<sub>10</sub>\*[Ar<sup>\*</sup>]\*[Ar<sup>\*</sup>] +
(-1)\*k<sub>11</sub>\*[Ar<sup>\*</sup>]\*[Ar]

d[Ar<sup>+</sup>]/dt = 1\*k<sub>3</sub>\*[e]\*[Ar] +
1\*k<sub>4</sub>\*[e]\*[Ar<sup>\*</sup>] +
(-1)\*k<sub>5</sub>\*[e]\*[e]\*[Ar<sup>+</sup>] +
1\*k<sub>7</sub>\*[e]\*[Ar<sup>+</sup><sub>2</sub>] +
(-1)\*k<sub>8</sub>\*[Ar<sup>+</sup>]\*[Ar]\*[Ar] +
1\*k<sub>9</sub>\*[Ar<sup>+</sup>]\*[Ar] +
1\*k<sub>10</sub>\*[Ar<sup>\*</sup>]\*[Ar<sup>\*</sup>]

d[Ar<sup>+</sup><sub>2</sub>]/dt = (-1)\*k<sub>6</sub>\*[e]\*[Ar<sup>+</sup><sub>2</sub>] +
(-1)\*k<sub>7</sub>\*[e]\*[Ar<sup>+</sup><sub>2</sub>] +
1\*k<sub>8</sub>\*[Ar<sup>+</sup>]\*[Ar]\*[Ar] +
(-1)\*k<sub>9</sub>\*[Ar<sup>+</sup>]\*[Ar]

d[e]/dt =
1\*k<sub>3</sub>\*[e]\*[Ar] +
1\*k<sub>4</sub>\*[e]\*[Ar<sup>\*</sup>] +
(-1)\*k<sub>5</sub>\*[e]\*[e]\*[Ar<sup>+</sup>] +
(-1)\*k<sub>6</sub>\*[e]\*[Ar<sup>+</sup><sub>2</sub>] +
1\*k<sub>10</sub>\*[Ar<sup>\*</sup>]\*[Ar<sup>\*</sup>]

### Exercise 5

![Output5](https://github.com/janpriessnitz/F5170-python/blob/master/6_Balance/exercise5.png)

The script outputs this plot, which is expected.

### Exercise 6

The equilibrium electron density increases roughly exponentially as we linearly increase the electron temperature. If we look at the table of reactions, we notice that electron concentration is increased by reactions number 3, 4 and 10 and decreased by reactions number 5 and 6. While the rate of reactions number 3 and 4 grows with electron temperature, rate of reactions 5 and 6 decreases with electron temperature. The time derivative of electron concentration thus increases with increasing electron temperature.

The ignition time decreases roughly exponentially as we increase the electron temperature.

For Te = 2.0 eV, [Ar<sup>+</sup>] dominates over [Ar<sup>+</sup><sub>2</sub>] both in the ignition and the equilibrium phase and this does not change for higher electron temperature.

Interesting behavior can be seen for electron temperatures between 1.0 eV and 2.0 eV. For 1.0 eV, the dominance is completely switched. However, for 1.5 eV, [Ar<sup>+</sup><sub>2</sub>] dominates in the ignition phase, but [Ar<sup>+</sup>] in the equilibrium phase.

### Exercise 7

Equilibrium electron density increases with increasing pressure, but the ratio between electron and neutral concentration decreases. As we increase the overall concentration, the ionization degree falls. That is directly explained by the Saha ionization equation, which states that the ionization degree is inversely proportional to concentration of ions (= concentration of electrons in plasma)

The ignition time seems to be inversely proportional to pressure.

### Advanced

![Output5](https://github.com/janpriessnitz/F5170-python/blob/master/6_Balance/advanced.png)
