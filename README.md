# Decagon

*Decagon* is a graph convolutional neural network (GCN) approach for multirelational link 
prediction in multimodal graphs. 

It is a general approach for multirelational link prediction in any multimodal network. 
Decagon handles multimodal graphs with large numbers of edge types. It works on simple and 
multimodal graphs. Please check the [project page](http://snap.stanford.edu/decagon) for more details.
  
## Usage

Decagon has been used to solve problems in computational pharmacology, specifically to model 
*polypharmacy side effects of drug pairs (i.e., drug combinations)*.

Using Decagon, we construct a multimodal graph of protein-protein interactions, drug-protein target interactions, and the polypharmacy side effects, which are represented as drug-drug interactions, where each side effect is an edge of a different type. Decagon then predicts the exact side effect, if any, through which a given drug combination manifests clinically.

![Polypharmacy graph](/images/polypharmacy-graph.png)

Decagon species a graph convolutional neural network architecture based on this multimodal graph to model and predict polypharmacy side effects.
  
![Polypharmacy side effect prediction](/images/decagon-architecture-1.png)

The setup for this problem using a dummy dataset is outlined in:

    main.py
    
The actual datasets are available for download from [project page](http://snap.stanford.edu/decagon).

## Citing

If you find *Decagon* useful for your research, please consider citing:

    @article{Zitnik2018,
      title     = {Modeling polypharmacy side effects with graph convolutional networks.},
      author    = {Zitnik, Marinka and Agrawal, Monica and Leskovec, Jure},
      journal   = {},
      volume    = {},
      number    = {},
      pages     = {},
      year      = {},
      publisher = {}
    }

## Miscellaneous

Please send any questions you might have about the code and/or the 
algorithm to <marinka@cs.stanford.edu>.

## Dependencies

Decagon is tested to work under Python 2.7.

The required dependencies for Decagon are [NumPy](http://www.numpy.org) >= 1.13, [NetworkX](https://networkx.github.io/) >= 2.0, and [TensorFlow](https://www.tensorflow.org/) >= 1.1.

## License

Decagon is licensed under the MIT License.
