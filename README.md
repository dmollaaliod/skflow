# Scikit Flow

This is a simplified interface for TensorFlow, to get people started on predictive analytics and data mining.

## Installation

First, make sure you have TensorFlow and Scikit Learn installed, then just run:

    pip install git+git://github.com/google/skflow.git

## Usage

Example usage:

    import skflow
    from sklearn import datasets, metrics
    iris = datasets.load_iris()
    classifier = skflow.TensorFlowClassifier(n_classes=3)
    classifier.fit(iris.data, iris.target)
    score = metrics.accuracy_score(classifier.predict(iris.data), iris.target)
    print "Accuracy:", score



