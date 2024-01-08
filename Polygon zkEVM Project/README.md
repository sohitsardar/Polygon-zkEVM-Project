# Polygon zkEVM

This repository contains a Circom circuit that checks a specific condition regarding input signals `a` and `b` and outputs the result in signal `q`.

Our goal is to prove you know the inputs A (0) & B (1) that yield a 0 output.


## Circuit Description

The `AssesmentCircuit` is designed to check if `q` is 0 when `a` is 0 and `b` is 1. The circuit utilizes logical gates such as AND, NOT, and OR to implement the required logic.

### Signal Inputs

- `a`: Input signal `a`.
- `b`: Input signal `b`.

### Signal Outputs

- `q`: Output signal that holds the result of the circuit.

### Circuit Logic

1. An AND gate (`andGate`) takes `a` and `b` as inputs and outputs the result to the signal `x`.
2. A NOT gate (`notGate`) takes `b` as an input and outputs the negation of `b` to the signal `y`.
3. An OR gate (`orGate`) takes `x` and `y` as inputs and outputs the result to the signal `q`.

The final output `q` will be 0 if `a` is 0 and `b` is 1; otherwise, it will be 1.

## Usage

To use this circuit, follow these steps:

1. Clone the repository:

2. Make sure you have Circom (2.0.0) installed on your system.

3. Compile the circuit:

4. Optionally, you can generate a constraint system and a witness using snarkjs:

5. Execute the circuit and get the output:


6. Verify the proof:

## Contributing

We welcome contributions to improve this Circom circuit or add new functionalities. If you find any issues or want to suggest improvements, please feel free to open an issue or submit a pull request.

## License

This Circom circuit is licensed under the [MIT License](LICENSE).

## Author

Sohit
