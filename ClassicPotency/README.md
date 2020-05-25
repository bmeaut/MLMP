#### Dependencies:
- ClassicPotency &#8594; BasicModule

#### Requirements:
- **C1** "As its name implies, the level of a model element is an integer representing the model level in which the element resides." Therefore, nodes, edges, and fields must be assigned a level n, which marks that a model element is on level n.

- **C2** The level of a model element must be greater than or equal to 0.

- **C3** The level of a field must be equal to the level of the containing node.

- **C4** Levels are separated by the instantiation relationship. When an instantiation occurs, the level of the instance must decrease by 1. Thus, the level of an instance must be less than the level of its meta by 1.

- **C5** A cross-level reference is an edge that runs between two nodes that are on different levels. Cross-level references are not allowed.

- **C6** "The potency of a model element is an integer that defines the depth to which a model element can be instantiated." Therefore, every model element must have potency assigned.

- **C7** "... potency of a model element cannot be greater than its level ..."

- **C8** The potency of a model element must be greater than or equal to 0.

- **C9** The potency of a field must be less than or equal to the potency of the containing node.

- **C10** "The act of instantiating a model element obviously reduces its potency by one."

- **C11** "Elements whose potency is 0 cannot be instantiated, regardless of their level number."

- **C12** The potency of all fields contained in an abstract node must be greater than 0.

- **C13** "A model element which has an isAbstract slot containing the value true has a potency of 0." Abstract nodes must have a potency of 0 and thus cannot be instantiated.

- **C14** "A field with potency 0 represents a slot, and therefore must have a value. However, a field of higher potency may or may not have a value, depending on whether it is a simple field or a dual field. ... A simple field is a field which does not have a value unless it has potency 0... A dual field is a field which has a value even for potencies greater than zero."

- **C15** Fields with a potency of 0 in the meta node must be omitted from the instance node. In our interpretation, this means that the instance node - and thus nodes instantiated from it - does not contain fields with a potency of 0.

- **C16** "Another good example of a model element with potency 0 is the inheritance relationship between two elements, as it can not be further instantiated." Thus, inheritance is a special edge with a potency of 0.

- **C17** During an inheritance between two nodes, the descendant must inherit every field of the parent. This requirement was deduced by us, as it reflects the most commonly used semantics of inheritance.

#### References:
- Atkinson, C., Kühne, T.: The essence of multilevel metamodeling. In: Proceedings of the 4th International Conference on The Uniﬁed Modeling Language, Modeling Languages, Concepts, and Tools, pp. 19–33. Springer-Verlag, Berlin, Heidelberg (2001). URL http://dl.acm.org/citation.cfm?id=647245.719475
