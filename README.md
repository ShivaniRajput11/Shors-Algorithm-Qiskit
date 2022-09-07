# Shors-Algorithm-Qiskit-

Let's understand:

### What is the Shor’s Algorithm

Shor’s Algorithm is a quantum algorithm for integer factorisation. Simply put given an odd integer N it will find it’s prime factors. 

The algorithm consists of 2 parts: 

Classical part which reduces the factorisation to a problem of finding the period of the function. This is done classically using a normal computer.

Quantum part which uses a quantum computer to find the period using the Quantum Fourier Transform.

### For the algorithm the steps are as follows: 

```bash 
Pick a random number A such that A < N

Computer the greatest common divisor (GCD) of and N

if the gcd != 1 then we found a factor of N

If not then run the quantum circuit that uses a Quantum Fourier Transform

If the period is odd then go back to step 1

Otherwise we have found the factors of N

```


### Implementation 

The algorithm can be implemented incredibly easily since Qiskit has a baked in function for the algorithm called Shor(N). 

Where N will be the integer you wish to factor. For example Shor(21) will find the prime factors for 21. 

So let's try it out
