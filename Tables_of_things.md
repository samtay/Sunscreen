# Dungeon Master's tables of FHE things

## BFV notes

When using a plain modulus large enough for batching, generating relin keys fails at `N=1024,2048`.

## Noise budget impact at minimum plain modulus to support batching of a single operation

| n     | Add  | Mul+relin |
|-------|------|-----------|
| 1024  | N/A  | N/A       |
| 2048  | N/A  | N/A       |
| 4096  | ~0   | ~26       |
| 8192  | ~0   | ~28       |
| 16384 | ~0   | ~29       |
| 32768 | ~0   | ~30       |

## Noise budget at minimum plain modulus to support batching

| n    | 1024 | 2048 | 4096 | 8192 | 16384 | 32768 |
|------|------|------|------|------|-------|-------|
| bits | N/A  | N/A  | 49   | 149  | 365   | 800   |
