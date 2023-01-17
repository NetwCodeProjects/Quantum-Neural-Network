# Quantum-Neural-Network
Mostly starting points or 
initializations for complex quantum programs.

# Quantum Neural Network 4-Qubit

This code creates a quantum circuit with four quantum registers (qreg_q) and four classical registers (creg_c). The circuit applies a Hadamard gate to the first qubit, applies a controlled-X gate between the first and second qubits, applies another controlled-X gate between the second and third qubits, applies a Hadamard gate to the fourth qubit, applies a barrier, and then measures all four qubits.

It is important to note that this circuit is not a complete quantum neural network. It is only a part of it that generates an input state. To build a full quantum neural network, one needs to create a quantum circuit that represents the neural network's architecture and also the training algorithm to update the weights.

# Deutsch-Jozsa algorithm

Deutsch-Jozsa algorithm, is a quantum algorithm that solves a specific problem known as the "Deutsch-Jozsa problem".

This code creates a quantum circuit with three quantum registers (qreg_q) and three classical registers (creg_c). The circuit applies a Hadamard gate to the second qubit, applies a controlled-X gate between the second and third qubits, applies another controlled-X gate between the first and second qubits, applies a Hadamard gate to the first qubit, applies a barrier, and then measures the first and second qubits. After another barrier, it applies an X gate and a Z gate to the third qubit, both controlled on the measurement results of the first and second qubits, respectively, and finally measures the third qubit.

# neuralnet_compression_qautoencoders

This code creates a quantum circuit that contains two layers, an encoding layer and a decoding layer.

The encoding layer starts by applying a Hadamard gate to the first qubit, which puts it in a superposition of the |0⟩ and |1⟩ states. Then it applies a controlled-X gate between the first and second qubits. This creates a controlled-NOT gate between the first and second qubits. Another controlled-X gate is applied between the second and third qubits, and a Hadamard gate is applied to the fourth qubit.

The decoding layer starts by applying a Hadamard gate to the third qubit, then it applies a controlled-X gate between the third and second qubits and between the second and first qubits. Finally, it applies a Hadamard gate to the fourth qubit.

The circuit ends with a barrier operation and the measurement of all four qubits. The measurements of all four qubits are then used to update the weights of a quantum neural network.

It is important to note that this code is not a complete quantum neural network, as it does not contain any training algorithm or any additional gates that would be used to update the weights of the network. It is only a part of the circuit that encodes and decodes the input state.
