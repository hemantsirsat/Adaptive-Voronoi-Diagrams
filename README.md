
# ADAPTIVE VORONOI DIAGRAMS FOR LEAKAGE DETECTION IN COMPOSITE MANUFACTURING

___

-- Studienarbeit --

### Description

___

The production of Carbon Fiber Reinforced Polymer(CFRP) components requires that the material preforms of an application-specific geometry, which is consolidated with the help of heat and pressure. During this process, the pressure is applied through a vaccum setup. The workpiece is covered by vaccum film that is made airtight by sealand tape along the edges. In practice, it may occur that the vaccum bag contains leakages which are in most of the cases not visible to the human eye. These leakages can cause serious defect that damages the final product making in unusable.

The underlying assumption is that the positions of potential leakage are close to the vaccum ports that have large flow values. This fits well with the idea of Voronoi diagrams. The idea is to create Voronoi regions for every vaccum port and the Voronoi edge will act as a hyperplane separating two Voronoi regions(halfspaces). Since, two Voronoi region will share a single Voronoi edge it is important to understand that moving one hyperplane in any direction will have an effect on two or more Voronoi regions.

The hyperplane is represented using the equation \(\mathbf{w}^T \mathbf{y} + b = 0\) where \(\mathbf{w} \in \mathbb{R}^n\) and \(b \in \mathbb{R}\).

### Goals

___

1. Become familiar with Voronoi diagrams [1] and the fact that each Voronoi region can be represented as the intersection of a finite number of halfspaces.
2. Appropriately parameterize the halfspaces contained in a Voronoi diagram and develop a machine learning framework to learn them from data.
3. Apply your framework using the leakage detection dataset provided by DLR.
4. Compare your machine learning framework with appropriate classical machine learning methods for the same task in terms of training time, data requirements, model complexity, and accuracy

### References

___

1. F. Aurenhammer and R. Klein, “Voronoi diagrams.,” Handbook of computational geometry, vol. 5, no. 10, pp. 201–290,
2000.
2. Tensorflow's [Writing a training loop from scratch](https://www.tensorflow.org/guide/keras/writing_a_training_loop_from_scratch)
3. Tensorflow ' [Better performance with tf.function](https://www.tensorflow.org/guide/function)