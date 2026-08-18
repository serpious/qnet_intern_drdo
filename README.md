# QNetwork Internship at SAG, DRDO [22 June - 31 July]
This file briefly summarizes my work done and topics studied during internship, updated regularly during the intern period. <br>
_Last updated: 15 July 2026_

**22 June - 28 June** <br>
General review and discussion of QNetwork topics and concepts, including mathematical formalism:
- entanglement swapping
- fidelity purification
- E91 protocol; quantum teleportation
- quantum network topology

**29 June - 15 July** <br>
- Centralized CHSH based widest-bottleneck routing algorithm code: simulating on meshes of 10, 15, 20 and 50 nodes and analysing the results.
- Making a short literature review on routing in quantum netwoks: routing protocols, path selection policies, metrics.
- Analysis of 50-node mesh design in CHSH algo; summarizing why purification-based routing is necessary in practical use.

**15 July - 31 July** <br>
- Dynamic Quantum Mesh Routing: A 15-node Quantum Network Mesh, where each link has some dynamic physical noise. There are two layers:
  - Physical Layer: Simulates sending entangled qubits over noisy channel and measure S.
  - Control Layer: Uses S-values to decide best path using the CHSH bottleneck algorithm, and as the edges evolve over time, sweep changed edges and makes decision whether to switch to a new path/drop-off completely if all fall below S = 2.0.
The quantum part is the entangled quantum links and how their weights are measured, where is the routing decision algorithm is classical.<br>
*Code for final algorithm will be added soon....*
