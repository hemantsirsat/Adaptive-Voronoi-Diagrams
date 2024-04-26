
# ADAPTIVE VORONOI DIAGRAMS FOR LEAKAGE DETECTION IN COMPOSITE MANUFACTURING

___

-- Studienarbeit --

### Description

___

The production of Carbon Fiber Reinforced Polymer(CFRP) components requires that the material preforms of an application-specific geometry, which is consolidated with the help of heat and pressure. During this process, the pressure is applied through a vaccum setup. The workpiece is covered by vaccum film that is made airtight by sealand tape along the edges. In practice, it may occur that the vaccum bag contains leakages which are in most of the cases not visible to the human eye. These leakages can cause serious defect that damages the final product making in unusable.

The underlying assumption is that the positions of potential leakage are close to the vaccum ports that have large flow values. This fits well with the idea of Voronoi diagrams. The idea is to create Voronoi regions for every vaccum port and the Voronoi edge will act as a hyperplane separating two Voronoi regions(halfspaces). Since, two Voronoi region will share a single Voronoi edge it is important to understand that moving one hyperplane in any direction will have an effect on two or more Voronoi regions.

The hyperplane is represented using the equation 
    \(\mathbf{w}^T \mathbf{y} + b = 0\) where \(\mathbf{w} \in \mathbb{R}^n\) and \(b \in \mathbb{R}\).

### Goals

___

1. Become familiar with Voronoi diagrams [1] and the fact that each Voronoi region can be represented as the intersection of a finite number of halfspaces.
2. Appropriately parameterize the halfspaces contained in a Voronoi diagram and develop a machine learning framework to learn them from data.
3. Apply your framework using the leakage detection dataset provided by DLR.
4. Compare your machine learning framework with appropriate classical machine learning methods for the same task in terms of training time, data requirements, model complexity, and accuracy

### References

___

1. Lionetto, Francesca. "Carbon Fiber Reinforced Polymers." Materials 14, no. 19 (2021): 5545. [DOI](10.3390/ma14195545)
2. Kumar, Salu, and Sandipan Roy. "Finite element analysis of aircraft wing using carbon fiber reinforced polymer and glass fiber reinforced polymer." IOP Conference Series: Materials Science and Engineering 402, no. 1 (2018): 012077. [DOI](10.1088/1757-899X/402/1/012077)
3. Mitchell, T.M. Machine Learning. McGraw-Hill International Editions, 1997.
4. Ripley, B.D. Pattern Recognition and Neural Networks. Cambridge University Press, 2007.
5. Singhal, G., S. Panwar, K. Jain, and D. Banga. "A comparative study of data clustering algorithms." International Journal of Computer Applications 83, no. 15 (2013): 41-46. [DOI](10.5120/14528-2927)
6. Jolly, Kevin. Machine learning with scikit-learn quick start guide: classification, regression, and clustering techniques in Python. Packt Publishing Ltd, 2018.
7. Bellelli, Francesco. “The Fascinating World of Voronoi Diagrams.” [Online] Built In, 2023. [URL](https://builtin.com/data-science/voronoi-diagram)
8. Aurenhammer, Franz. "Voronoi diagrams—a survey of a fundamental geometric data structure." ACM Comput. Surv. 23, no. 3 (1991): 345–405. [DOI](10.1145/116873.116880)
9. Aurenhammer, Franz, and Rolf Klein. "Chapter 5 - Voronoi Diagrams." In Handbook of Computational Geometry, edited by J.-R. Sack and J. Urrutia, 201-290. North-Holland, 2000. [DOI](https://doi.org/10.1016/B978-044482537-7/50006-1)
10. Joswig, Michael, and Thorsten Theobald. "Voronoi Diagrams." In Voronoi Diagrams, 81-98. Springer, 2013. ISBN, [DOI](10.1007/978-1-4471-4817-3_6)
11. Pokojski, Wojciech, and Paulina Pokojska. "Voronoi diagrams - inventor, method, applications." Polish Cartographical Review 50, no. 3 (2018): 141-150. [DOI](10.2478/pcr-2018-0009)
12. Hochreiter, Sepp, and Jürgen Schmidhuber. "Long Short-Term Memory." Neural Computation 9, no. 8 (1997): 1735-1780. [DOI](10.1162/neco.1997.9.8.1735)
13. Gallier, Jean. "Dirichlet--Voronoi Diagrams and Delaunay Triangulations." In Geometric Methods and Applications: For Computer Science and Engineering, 301-319. Springer New York, 2011. [DOI](10.1007/978-1-4419-9961-0_10)
14. Pisner, Derek A., and David M. Schnyer. "Chapter 6 - Support vector machine." In Machine Learning, edited by Andrea Mechelli and Sandra Vieira, 101-121. Academic Press, 2020. [DOI](https://doi.org/10.1016/B978-0-12-815739-8.00006-7)
15. Zhang, Liang, and Adrian W. Cross. "Potentials of Machine Learning in Vacuum Electronic Devices Demonstrated by the Design of a Magnetron Injection Gun." IEEE Transactions on Electron Devices 68, no. 6 (2021): 3028-3033. [DOI](10.1109/TED.2021.3075166)
16. Plucknett, W., L. G. S. Giraldo, and J. Bae. "Metric learning in freewill eeg pre-movement and movement intention classification for brain machine interfaces." Frontiers in Human Neuroscience 16 (2022):. [DOI](10.3389/fnhum.2022.902183)
17. Hishinuma, Kazuhiro, and Hideaki Iiduka. "Incremental and Parallel Machine Learning Algorithms With Automated Learning Rate Adjustments." Frontiers in Robotics and AI 6 (2019). [DOI](10.3389/frobt.2019.00077)
18. Aggarwal, Charu C. "An Introduction to Outlier Analysis." In Outlier Analysis, 1-34. Springer International Publishing, 2017. [DOI](10.1007/978-3-319-47578-3_1)
19. Goodfellow, I., Y. Bengio, and A. Courville. Deep Learning. MIT Press, 2016. [URL](https://books.google.de/books?id=Np9SDQAAQBAJ)
20. Hakimi, Milad, and Arrvindh Shriraman. "TapeFlow: Streaming Gradient Tapes in Automatic Differentiation." In 2024 IEEE/ACM International Symposium on Code Generation and Optimization (CGO), 81-92. IEEE, 2024. [DOI](10.1109/CGO57630.2024.10444805)
21. van Heeswijk, Wouter. Implementing Actor Networks for Discrete Control in TensorFlow 2.0. 2020.
22. Edelsbrunner, H., and Raimund Seidel. "Voroni Diagrams and Arrangements." Discrete & Computational Geometry 1 (1986): 25-44. [URL](http://eudml.org/doc/130979)
23. Berg, M. d., O. Cheong, M. v. Kreveld, and M. H. Overmars. "Computational geometry." (2008). [DOI](10.1007/978-3-540-77974-2)
24. Ghahramani, Zoubin. "Unsupervised Learning." In Advanced Lectures on Machine Learning: ML Summer Schools 2003, Canberra, Australia, February 2 - 14, 2003, Tübingen, Germany, August 4 - 16, 2003, Revised Lectures, edited by Olivier Bousquet, Ulrike von Luxburg, and Gunnar Rätsch, 72-112. Springer Berlin Heidelberg, 2004. [DOI](https://doi.org/10.1007/978-3-540-28650-9_5)
25. Tensorflow's [Writing a training loop from scratch](https://www.tensorflow.org/guide/keras/writing_a_training_loop_from_scratch)
26. Tensorflow ' [Better performance with tf.function](https://www.tensorflow.org/guide/function)