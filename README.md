# vibe-net

## What is this?

This is a neural network that can recognize a handwritten digit (hardcoded to an ASCII art 7).

## How do I use it?

1. Open `neural_net_viz.html` in your browser.
1. **Step Neuron (`Step Neuron`)**: Steps through the feed-forward pass one single neuron at a time. The active line connections light up and the current neuron's value will update.
1. **Finish Layer (`Finish Layer`)**: Fast-forwards completing the calculations for all the neurons in the current layer.
1. **Start Backpropagation (`Step: Backprop Phase`)**: After the Output Layer finishes predicting, the "Step Neuron" button becomes a "Step: Backprop Phase". This triggers the network to calculate the Cost Gradient. This process highlights lines in Red/Blue depending on the weights needed to be increased or decreased to hit the target.
1. **Train Step (`Train Step`)**: Fast-forwards the entire forward and backward propagation and adjusts the weights automatically. It dynamically slows down to visually animate the backward pass.
1. **Train to Epsilon (`Train to Epsilon`)**: Set your desired target loss in the `Epsilon` input box, and click this button to continuously run entire training epochs until the network's Total Cost drops below that threshold.
1. **Reset (`Reset`)**: Reinitializes the neural network with random weights and clears all current states.

### Inspecting the Network
You can hover over any neuron or input pixel to view its given value. You can also hover over the connection lines between neurons to inspect the connection weight and cost gradient during the backpropagation phase.