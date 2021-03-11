#### Dependencies:
- ClassicPotency &#8594; BasicModule

#### Requirements:
- **CP1** "As its name implies, the level of a model element is an integer representing the model level in which the element resides." Therefore, every model element (node, edge, field) must be assigned a level n, which reflects that said model element is on level n.

- **CP2** The level of a model element must be greater than or equal to 0.

- **CP3** The level of a field must be equal to the level of the containing node.

- **CP4** Levels are separated by the instantiation relationship. The instance of a model element is on the level exactly one less than that of the model element.

- **CP5** A cross-level reference is an edge that runs between two nodes that are on different levels. Cross-level references are not allowed. Strictly speaking, this requirement relates to "strict meta-modeling" frameworks like the OCA.

- **CP6** "The potency of a model element is an integer that defines the depth to which a model element can be instantiated." Therefore, every model element must have potency assigned.

- **CP7** "... potency of a model element cannot be greater than its level ..."

- **CP8** The potency of a model element must be greater than or equal to 0.

- **CP9** "The act of instantiating a model element obviously reduces its potency by one." Thus, the instance of a model element has a potency value that is exactly one less than that of the model element.

- **CP10** "Elements whose potency is 0 cannot be instantiated, regardless of their level number."

- **CP11** "A model element which has an isAbstract slot containing the value true has a potency of 0." Abstract nodes must have a potency of 0 and thus cannot be instantiated.

- **CP12** "A field with potency 0 represents a slot, and therefore must have a value. However, a field of higher potency may or may not have a value, depending on whether it is a simple field or a dual field. ... A simple field is a field which does not have a value unless it has potency 0... A dual field is a field which has a value even for potencies greater than zero."

- **CP13** When instantiating a node, only fields with a potency greater than 0 appear in the instance node (with potencies reduced by exactly 1).

- **CP14** "Another good example of a model element with potency 0 is the inheritance relationship between two elements, as it can not be further instantiated." Thus, inheritance is a special edge with a potency of 0.

- **CP15** When inheriting between two nodes, the descendant must inherit every field of the parent, which has a potency greater than 0. This requirement is our interpretation, as we believe it better reflects and restricts the semantics of inheritance.

#### References:
- Atkinson, C., Kühne, T.: The essence of multilevel metamodeling. In: Proceedings of the 4th International Conference on The Uniﬁed Modeling Language, Modeling Languages, Concepts, and Tools, pp. 19–33. Springer-Verlag, Berlin, Heidelberg (2001). [URL]( http://dl.acm.org/citation.cfm?id=647245.719475)
