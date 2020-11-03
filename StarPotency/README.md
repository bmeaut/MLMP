#### Dependencies:
- StarPotency &#8594; ClassicPotency

#### Requirements
- **SP1** "If an isonym i is instance of a clabject c and c has a potency of * then i can have * or any non-negative number as potency. * is represented in the model by the integer value -1 because the potency is of type integer." Therefore, the potency value must either be a non-negative number (similarly to classic potency) or -1, which represents star potency. Moreover, after an instantiation, the potency of the instance can be of any value.

- **SP2** Star potency can be assigned to nodes, edges, and fields.

- **SP3** Star potency cannot be used in conjunction with classic potency on the same model element.

- **SP4** "If the corresponding Feature of its type t has a * potency the Feature in i can have a non-negative or * potency." This means that star potency features are only allowed in clabjects that have a star potency themselves.

#### References:
- Gerbig, R.: The level-agnostic modeling language: Language specification and tool implementation. Master’s thesis, Mannheim (2011). [URL](https://madoc.bib.uni-mannheim.de/37153/1/arbeit.pdf)
