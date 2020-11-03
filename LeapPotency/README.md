#### Dependencies:
- LeapPotency &#8594; ClassicPotency

#### Requirements:
- **LP1** "Clabjects and references with a leap potency of n can be instantiated exactly n meta-levels below, but not at intermediate meta-levels." This is conceptually equivalent to skipping the instantiation of the model element at the intermediate levels. Only nodes and edges can have leap potency assigned.

- **LP2** Classic potency and leap potency cannot be used in conjunction on a model element, as their semantics would overlap.

- **LP3** Similarly to classic potency, the leap potency of a model element must be less than or equal to its level.

- **LP4** On an instantiation, the leap potency of the instance must be 0.

#### References:
- de Lara, J., Guerra, E., Cobos, R., Moreno-Llorena, J.: Extending Deep Meta-Modelling for Practical Model-Driven Engineering. The Computer Journal 57(1), 36–58 (2012). [URL](https://www.doi.org/10.1093/comjnl/bxs144) 
