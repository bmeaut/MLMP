#### Dependencies:
- Order &#8594; ClassicPotency

#### Requirements
- **O1** "The order of a modeling element can be regarded as a measure of its set-theoretic classification power, since it corresponds to the maximum depth of the “type-of” relationships originating from an element." In our interpretation, order can only be assigned to nodes.

- **O2** The order of a node must be less than or equal to its level.

- **O3** The order of a node must be greater than or equal to its potency.

- **O4** "Abstract classes are restricted to having indirect instances (through their subclasses)." Therefore, the order of an abstract node and its fields must be greater than 0.

- **O5** "Pure instances, typically representing domain particulars, have order zero, since they do not classify any instances." Therefore, a model element with a potency value 0 must have an order of 0.

#### References:
- Kühne, T.: Exploring potency. In: Proc. of the 21th ACM/IEEE International Conference on Model Driven Engineering Languages and Systems, MODELS ’18, pp. 2–12. ACM, New York, NY, USA (2018). DOI 10.1145/3239372.3239411
- Kühne, T.: A story of levels. In: Proceedings of MODELS 2018 Workshops, Copenhagen, Denmark, 2018, pp. 673–682 (2018). URL http://ceur-ws.org/Vol2245/multi_paper_5.pdf

