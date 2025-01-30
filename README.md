# Variational Quantum Algorithms for Ground-State Properties and Analysis of the spin- $\frac{1}{2}$ Kagome Heisenberg Model

---

## Detailed Theory : 
The Kagome lattice is a hexagonal star shaped lattice structure and is an exaple of spin sheet. An inifitely expanding structure of a 2D local structure. We employ VQE to probe GS properties and find out more about the energy spectra using SSVQE etc. 

---

### Tasks done yet : 
1. Try it out for simpler geometries like triangle and rectangle. Find energies, use a random su2 ansatz and run tests for the same against the connectivity graph hamiltonian. 
2. Check whether min eigval matches with the vqe generated minimum value. 
3. Now try error mitigation using ZNE etc.
4. Test trotter theory and check time evolution for theoretically derived minimum energy state.

---

### Workflow :

1. Choose a good ansatz with $n_1$ qubits, then choose "better" and "larger-sized" lattices. Show optimization parallely once succesful runs are observed..
2. PROBLEM AND STEP 1 : Before all that, build the ground state of the kagome heisenberg lattice. (Use whatever theory is required XXZ spin chain or Bethe Ansatz or whatever I couldn't care less)
3. PROBLEM AND STEP 2 : Build the hamiltonian correctly for the model at hand (heisenberg model for the kagome lattice). (The heisenberg can have first order and second order correlations which might be difficult to capture...)
4. After including the first order corrections heisenberg, test the results using any optimizer... (more fine correlations and energies can be incorporated later)
5. Check for different ansatzes - show improvement (expected)
6. For computational overload you _MIGHT_ try using ADAPT-VQE algorithm.
7. Validate the ground state energy and find error %.
8. Refine the cost function to find other function values...
---