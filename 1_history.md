
We had a frontend app and many Haskell apps with:

*  Data Type (HKD pattern)
*  2-way binding Data Type <-> UI
*  fixed set of SemanticArrows called Atoms (SemanticArrow - internal effect system)
*  logic solver that knew how to combine Atoms to populate data

Challenge:

How do we expose this to Python?
Jason implemented the answer "extending" GraphQL
... and then we kept expanding ...
