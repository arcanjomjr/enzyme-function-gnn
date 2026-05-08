This project implements a Graph Neural Network to predict enzyme function based on their structures. Specifically, it distinguishes between oxidoreductases (EC 1) and transferases (EC 2) in _Escherichia coli_.

The model was built for learning purposes and is very simple. The vertices of the graph are the alpha-carbons of the protein, there is and edge between two vertices when their distance is less than 8Å. The initial feature vectors of the vertices are the one-hot encoding of the corresponding amino acids. The model architecture is composed of five graph convolution layers, global mean pooling, and a final linear prediction head.

The model achieves 90% accuracy on the balanced test set.