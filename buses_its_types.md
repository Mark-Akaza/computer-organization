## *🚌 Buses in Computer Architecture*  
A *bus* is a communication system that transfers data between different components of a computer (CPU, memory, I/O devices). It consists of *wires (or traces on a motherboard)* that carry *data, addresses, and control signals*.

---

## *📌 Types of Buses*
There are three main types of buses in a computer:  

1️⃣ *Address Bus* (Single Direction →)  
2️⃣ *Data Bus* (Bidirectional ⇄)  
3️⃣ *Control Bus* (Single Direction or Bidirectional → or ⇄)  

---

### *1️⃣ Address Bus* 🚏 (Single Direction →)  
- *Purpose:* Carries memory or I/O addresses from the CPU to other components.  
- *Direction:* *Unidirectional* (Only from CPU to memory/I/O).  
- *Example:* If the CPU wants to read from memory location *1000, it sends **1000* through the address bus.  

📌 *More address lines = more memory can be accessed.*  
✅ Example:  
   - *16-bit address bus* → Can access *2¹⁶ = 65,536 (64 KB) memory locations*.  
   - *32-bit address bus* → Can access *4 GB* of memory.  
   - *64-bit address bus* → Can access *16 EB (Exabytes)* of memory.  

---

### *2️⃣ Data Bus* 🚏 (Bidirectional ⇄)  
- *Purpose:* Transfers actual data between CPU, memory, and I/O devices.  
- *Direction:* *Bidirectional* (CPU can *read* or *write* data).  
- *Example:* If the CPU wants to *add two numbers, it first fetches them through the **data bus, processes them, and then stores the result back via the **data bus*.  

📌 *More data lines = faster data transfer.*  
✅ Example:  
   - *8-bit data bus* → Can transfer *1 byte* at a time.  
   - *16-bit data bus* → Can transfer *2 bytes* at a time.  
   - *64-bit data bus* → Can transfer *8 bytes* at a time (modern CPUs).  

---

### *3️⃣ Control Bus* 🚏 (Single/Bidirectional → or ⇄)  
- *Purpose:* Carries control signals (commands) to *coordinate operations*.  
- *Direction:* *Both* unidirectional and bidirectional (depending on the signal).  
- *Example:* If the CPU wants to read from memory, it sends a *"READ" control signal* to memory via the control bus.  

📌 *Common Control Signals:*  
✔ *Read Signal:* Tells memory to send data.  
✔ *Write Signal:* Tells memory to store data.  
✔ *Interrupt Request (IRQ):* Sent from I/O devices to CPU (e.g., a key was pressed).  
✔ *Clock Signal:* Synchronizes operations in the CPU.  

---

## *🖥 How These Buses Work Together*
🔹 *Example:* The CPU wants to read data from memory:  
1️⃣ *CPU places the address* on the *Address Bus*.  
2️⃣ *Control Bus signals* a *READ operation*.  
3️⃣ *Memory places the data* on the *Data Bus*.  
4️⃣ *CPU receives the data* and processes it.  

---

## *🛣 System Bus vs Expansion Bus*
Computers also have different categories of buses:

### *1️⃣ System Bus (Internal Bus)*
- Connects CPU, memory, and internal components.
- Includes *Address Bus, Data Bus, and Control Bus*.
- Faster because it is directly connected to the processor.

### *2️⃣ Expansion Bus (External Bus)*
- Connects external devices (USB, PCI, etc.).
- Allows the CPU to communicate with peripheral devices.
- *Examples:* PCI, PCIe, USB, SATA.

---

## *🚀 Summary Table*
| *Bus Type*  | *Purpose*                 | *Direction* | *Examples* |
|--------------|----------------------------|-------------|------------|
| *Address Bus*  | Sends memory/I/O addresses | Unidirectional (→) | 32-bit, 64-bit |
| *Data Bus*     | Transfers actual data      | Bidirectional (⇄) | 8-bit, 16-bit, 64-bit |
| *Control Bus*  | Sends control signals     | Uni/Bidirectional | Read, Write, Interrupt |

---

## *🔥 Final Thoughts*
✅ *More address lines = More memory access*.  
✅ *More data lines = Faster processing*.  
✅ *Control Bus ensures smooth operation*.  

