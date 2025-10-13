# AG-Codes-for-Grover-Oracle


### Features

- **AG Code Oracles**: Grover oracles for AG code parameter optimization
- **Hermitian Curves**: Specialized implementation for well-known AG codes
- **Quantum Decoding**: Grover-based decoding algorithms for AG codes
- **Curve Arithmetic**: Mathematical operations on algebraic curves

### Usage Examples

```python
from extensions.ag_codes import HermitianCurveOracle

# Create oracle for Hermitian curve over F_4
hermitian_oracle = HermitianCurveOracle(q=2)

# Construct decoding oracle
oracle = hermitian_oracle.construct_quantum_decoding_oracle(
    received_word=[0,1,0,1,0,1,0],
    error_weight=1
)
