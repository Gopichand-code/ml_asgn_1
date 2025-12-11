Project Overview

This project investigates the implicit bias of gradient descent in overparameterised neural networks. Although such networks have enough capacity to memorise arbitrary labels, they frequently generalise well in practice—even without explicit regularisation. This behaviour has become one of the most important topics in modern machine learning, challenging classical views of the bias–variance trade-off.

The goal of this study is to provide clear empirical and conceptual evidence that gradient descent naturally prefers simple, large-margin, and low-complexity solutions. Through controlled experiments involving noisy labelled data, the results highlight how optimisation—not architectural constraints—drives generalisation.

Key Findings

Perfect memorisation without overfitting collapse
The model reaches 100% accuracy on the noisy training set while maintaining stable generalisation performance on the clean test set.

Monotonic growth of weight norms
The magnitude of learned weights grows steadily throughout training, even after perfect interpolation. This is consistent with theoretical results showing that gradient descent moves toward maximum-margin solutions.

Increasing classification margin
Decision margins continue to increase long after achieving perfect training accuracy, indicating convergence toward geometrically simpler and more robust decision boundaries.

Alignment with theoretical predictions
The behaviours observed match analytical findings from implicit bias research in linear classifiers and extend naturally to deep networks.

Dataset Summary

The experiments use a binary subset of the CIFAR-10 dataset (airplane vs. automobile).
To reveal implicit regularisation more clearly, 20% of training labels are randomly corrupted, while the test set remains unaltered.
This setup ensures that perfect interpolation requires memorising noise, making implicit bias effects easier to observe.

Figures Included

Training vs. test accuracy over epochs

Weight-norm evolution during training

Classification margin growth

Each figure is accompanied by alt-text descriptions and high-contrast, accessible visual design.

Accessibility Notes

Colour-blind-friendly palettes were used for all charts.

Alt-text descriptions are provided for every figure.

Clear, hierarchical headings support screen-reader navigation.

No reliance on colour-only cues for interpretation.

License

This work is distributed under the MIT License, allowing others to reuse and adapt the material with proper attribution.
