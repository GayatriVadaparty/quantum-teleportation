# Quantum Teleportation- Making cartoon logic to reality
Have you ever thought how the world would be if teleportation is possible? Do you think it is possible? Seems like the answer is no. However, the researchers and scientists keep on working to make it true. Meanwhile, it is suggested to know something about No-Cloning Theorm and Quantum Teleportation protocol.
No-Cloning theorm
Let's understand this in simple terms. Suppose, Alice have to send quantum information to Bob. Precisely, she wants to send the qubit state |q⟩=α|0⟩+β|1⟩. The no-cloning theorm states that you cannot simply make an exact copy of an unknown quantum state. Hence, we can see that Alice can't simply generate a copy of |q⟩ and give the copy to Bob. We know that we can copy bits of information. However, the quantum qubits exists in superposition which leads them to remain uncopied.
In spite of that, here we have two classical bits and an entangled qubit pair, Alice can transfer her state |q⟩ to Bob. This phenomenon is called Quantum teleportation. In this method,transfer took place i.e, the Alice won't have the qubit |q> anymore.

Quantum Teleportation protocol
In order to transfer |q>, Alice and Bob must use a channel to send them an entangled qubit pair. Alice then performs some operations on her qubit, sends the results to Bob over a classical communication channel, and Bob then performs some operations on his end to receive Alice’s qubit.

A third person Clark ,now creates an entangled pair of qubits and gives one to Bob and one to Alice. This entangled pair is called Bell-state. In qiskit, Creating a Bell state between two qubits can be done by first transfering one of them to the X-basis ( |+⟩ and |−⟩) using a Hadamard gate, and then to applying a CNOT gate onto the other qubit controlled by the one in the X-basis.

Now, let us assume Alice got it's part q1 and bob's q2. Alice applies a CNOT gate to q1, controlled by |q⟩ (original qubit which she is trying to send Bob). Then Alice applies a Hadamard gate to |q⟩ .Hence, the qubit (|q⟩) Alice is trying to send is let's say q0.

Next, Alice applies a measurement to both qubits that she owns, q1 and |q⟩ , and stores this result in two classical bits. She then sends these two bits to Bob. Bob, who already has the qubit q2, then applies the following gates depending on the state of the classical bits:

00 here Does nothing, 01 -> Apply X gate, 10 -> Apply Z gate, 11 -> Apply ZX gate.

download (1).jfif

Mathematics behind Quantum Teleportation Protocol
Alice have to transfer |q⟩=α|0⟩+β|1⟩ (a random qubit) to Bob. She doesn't know the state of the qubit. For this, Alice and Bob take the help of the Clark(a third person). Clark made a pair of entangled qubits for Alice and Bob. The entangled qubits could be written in Dirac Notation as:

|q'⟩=1/√2(|00⟩+|11⟩) Alice and Bob each possess one qubit of the entangled pair,

|e⟩=1/√2(|0'>|0''⟩+|1'⟩|1''⟩) This creates a three qubit quantum system where Alice has the first two qubits and Bob the last one.

|q⟩⊗|e⟩=1/√2(α|0⟩⊗(|00⟩+|11⟩)+β|1⟩⊗(|00⟩+|11⟩))=1/√2(α|000⟩+α|011⟩+β|100⟩+β|111⟩)

Secondly, Now according to the protocol Alice applies CNOT gate on her two qubits followed by Hadamard gate on the first qubit. This results in the state:

(H⊗I⊗I)(CNOT⊗I)(|q⟩⊗|e⟩)

=(H⊗I⊗I)(CNOT⊗I)1/√2(α|000⟩+α|011⟩+β|100⟩+β|111⟩)

=(H⊗I⊗I)1/√2(α|000⟩+α|011⟩+β|110⟩+β|101⟩)

=1/2(α(|000⟩+|011⟩+|100⟩+|111⟩)+β(|010⟩+|001⟩−|110⟩−|101⟩))

Which can then be separated and written as:

=1/2(|00⟩(α|0⟩+β|1⟩)+|01⟩(α|1⟩+β|0⟩)+|10⟩(α|0⟩−β|1⟩)+|11⟩(α|1⟩−β|0⟩))

Then, Alice measures the first two qubit (which she owns) and sends them as two classical bits to Bob. The result she obtains is always one of the four standard basis states
|00⟩,|01⟩,|10⟩ ,and |11⟩ with equal probability. On the basis of her measurement, Bob's state will be projected to, |00→(α|0⟩+β|1⟩)|01→(α|1⟩+β|0⟩)|10→(α|0⟩−β|1⟩)|11⟩→(α|1⟩−β|0⟩). Finally, Bob, on receiving the bits from Alice, knows he can obtain the original state |q⟩ by applying appropriate transformations on his qubit that was once part of the entangled pair. The transformations he needs to apply are:

image.pngTherefore, Bob can recreate the qubit which is transferred by Alice by applying some operations on it.

Now, let's think about what we can do with this Teleportation. I believe, Teleportation is done in three ways. THe first says the object get completely scanned by light and they recreated with the beam again. The second says, There will be dismantle of the object into many simplier particles and all parts realligned together and thus object recreated. Lastly, there will some kind of 'spooky action' or magic which makes the object disappears somewhere at a particular point of time and reappeared somewhere in the later time.

Is human Teleportation possible?
First, let's make our idea cleared out of compilicated things. When you could teleport yourself, it takes the transition time. Unlike light which takes least time, we consisting of matter takes time greater than light takes. It could be the accurate reason though.

download.jfif

Now, let's think about what is going to be teleported. Interestingly, according to cartoon or science fiction logic, we can teleport across obstacles. However, particles of matter can't be passed through obstacle barriers because many of them interact too strongly with real world atoms. Since, we cannot have control over our environment, it became a difficult question to answer about teleportation of matter.

The spontaneous 'time' relative probelm is discussed. In addition to that, we have another barrier called energy. When you're moving from one place to another, you require some energy whether it can be chemical energy or kinetic energy.While conserving energy, there must be still a minimum energy utilised there too.

This is how i understood how teleportation works which is quite interesting.
