# adversarial.js

Break neural networks in your browser.

An interactive, in-browser demonstration of adversarial attacks on neural networks, implemented entirely in JavaScript.

## Get Started

Try the demo: [kennysong.github.io/adversarial.js](https://kennysong.github.io/adversarial.js)

![Demo Screenshot](https://raw.githubusercontent.com/kennysong/adversarial.js/main/docs/data/screenshot.png)

## Implementation

adversarial.js is completely implemented in JavaScript – so it can run entirely within your browser. We rely on TensorFlow.js.

The library supports the following attacks:

* [Fast Gradient Sign Method](https://arxiv.org/pdf/1412.6572.pdf) (L_inf attack)
* [Basic Iterative Method](https://arxiv.org/pdf/1607.02533.pdf) (L_inf attack)
* [Jacobian-based Saliency Map Attack](https://arxiv.org/pdf/1511.07528.pdf) (L0 attack)
* [Jacobian-based Saliency Map Attack, One-Pixel](https://arxiv.org/pdf/1511.07528.pdf) (L0 attack)
* [Carlini & Wagner](https://arxiv.org/pdf/1608.04644.pdf) (L2 attack)

The demo can break the following pre-loaded systems:

* MNIST (digit recognition)
* GTSRB (street sign recognition)
* CIFAR-10 (object recognition, small images)
* ImageNet (object recognition, large images)

## FAQ

[See the website](https://kennysong.github.io/adversarial.js/faq.html).

## Repo Structure

1. `src/adversarial.js`: The core adversarial.js library with all attacks
2. `docs/`: The interactive demo files. Explore the [live website](https://kennysong.github.io/adversarial.js).
3. `docs/js`:  Contains a copy of `adversarial.js`, in addition to many other JavaScript files for loading data and powering the demo
4. `docs/data`:  Contains (subsets) of datasets used in the demo.
