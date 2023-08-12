A parity bit is appended to the actual data. It then can be recalculated upon receiving the data and checked against the value sent. Only single bit errors can be detected.

## Calculation
To calculate the value of the parity bit, simple sum the bits and ignore the carry.

$$
\displaylines{
	p = (x_1 + x_2 + \dots + x_n) \mod 2 \\
	p_{1010} = (1 + 0 + 1 + 0) = 0 \\
	p_{1110} = (1 + 1 + 1 + 0) = 1 \\
}
$$
