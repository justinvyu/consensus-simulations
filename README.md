# consensus-simulations
iPython notebook experiments to compare different consensus algorithms (PoW, PoS)

# Proof of Work

Providing proof of work means solving a complicated problem that takes time and energy, but can be checked for validity instantly.

Examples of PoW:
1. Cryptographic hash function
  - Cryptographic hash functions are the most common.
2. Integer Factorization
3. Guided Tour Puzzle Protocol

Purpose: protects the blockchain from attackers by making it economically/computationally impractical and unreasonable to alter the chain for the attacker’s benefit.

# Proof of Stake

Proof of Stake (PoS) is a consensus algorithm that chooses “validators/forgers” in a network deterministically (based on how much “stake” they have in the network).

Differences from PoW:
1. No block rewards are generated: the validator/forger receives transaction fees instead
2. There is less wasted computation, since the forger is chosen to create the block.

Protecting from “bad forgers”:
- Some PoS algorithms require forgers to submit a deposit greater than the amount that he/she would receive from the transaction fees.
  - IF: the block is deemed accurate by other forgers, the deposit goes back to the forger
  - ELSE: the deposit does not go back to the forger, no transaction fees awarded either
