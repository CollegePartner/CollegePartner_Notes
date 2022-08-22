# Input-Output Organization
## Peripheral Devices
The input-output subsystem of a computer, referred to as I/O , provides an
effldent mode of communication between the central system and the outside
environment. 

Programs and data must be entered into computer memory for
processing and results obtained from computations must be recorded or dis­played for the user. 

A computer serves no useful purpose without the ability to receive information from an outside souroe and to transltUt results in a
meaningful form.

The most familiar means of entering information into a computer is
through a **typewrite** like **keyboard** that allows a person to enter alphanumeric information directly.

Every time a key is depressed, the terminal sends a binary
coded character to the computer.The fastest possible speed for entering
information this way depends on the person's typing speed.

On the other hand, the central processing unit is an extremely fast device capable of performing operations at very high speed. When input information is transferred to the processor via a slow keyboard, the processor will be idle most of the time while waiting for the information to arrive.

To use a computer efficiently, a large amount of programs and data must be prepared in advance and transmitted into a storage medium such as magnetic tapes or disks .

The information in the disk is then transferred into computer memory at a rapid rate.

Results of programs are also transferred into a high-speed storage, such as disks, from which they can be transferred later into a printer to provide a printed output of results.

----
Devices that are under the direct control of the computer are said to be
connected on-line.

These devices are designed to read information into or out of the memory unit upon command from the CPU and are considered to be part of the total computer system.

*Input or output devices attached to the computer are also called **peripherals** .*

Among the most common **peripherals** are **keyboards**, **display units**, and **printers**.

**Peripherals** that provide auxiliary storage for the system are **magnetic disks and tapes**. Peripherals are electromechanical and electromagnetic devices of some complexity.

---
### **MAGNETIC TAPES.**
Magnetic tapes are used mostly for storing files of data: *for example*, a
company's payroll record. Access is sequential and consists of records that can be accessed one after another as the tape moves along a stationary read-write mechanism. It is one of the cheapest and slowest methods for storage and has the advantage that tapes can be removed when not in use.

### **MAGNETIC DISK.**
Magnetic disks have high-speed rotational surfaces coated with magnetic material. Access is achieved by moving a read-write mechanism to a track in the magnetized surface. Disks are used mostly for bulk storage of programs and data.

---
Other input and output devices encountered in computer systems are
digital incremental plotters, optical and magnetic character readers, analog-todigital converters, and various data acquisition equipment.

Not all input comes from people, and not all output is intended for people. Computers are used to control various processes in real time, such as machine tooling, assembly line procedures, and chemical and industrial processes. For such applications, a method must be provided for sensing status conditions in the process and sending control signals to the process being controlled.



****

# Input-Output Interface
Input-output interface provides a method for transferring information between internal storage and external I/0 devices. Peripherals connected to a computer need special communication links for interfacing them with the
central processing unit. The purpose of the communication link is to resolve
the differences that exist between the central computer and each peripheral.
The major differences are:
1. Peripherals are electromechanical and electromagnetic devices and their manner of operation is different from the operation of the CPU and
memory, which are electronic devices. Therefore, a conversion of signal
values may be required.

2. The data transfer rate of peripherals is usually slower than the transfer
rate of the CPU, and consequently, a synchronization mechariism may
be needed.

3. Data codes and formats in peripherals differ from the word format in
the CPU and memory.

4. The operating modes of peripherals are different from each other and
each must be controlled so as not to disturb the operation of other
peripherals connected to the CPU.

To resolve these differences, computer systems include special hardware
components between the CPU and peripherals to supervise and synchronize
all input and output transfers. These components are called **interface units** because they interface between the *processor bus and the peripheral device.* 

In addition, each device may have its own controller that supervises the operations of the particular mechanism in the peripheral.



# to be continued.......

---
# Modes of Transfer
Binary information received from an external device is usually stored in memory for later processing. Information transferred from the central computer into an external device originates in the memory unit. The CPU merely executes the 110 instructions and may accept the data temporarily, but the ultimate source or destination is the memory unit. Data transfer between the central computer and 110 devices may be handled in a variety of modes. Some modes use the CPU as an intermediate path; others transfer the data directly to and from the memory unit. Data transfer to and from peripherals may be handled in one of three possible modes:

1. Programmed 110
2. Interrupt-initiated 110
3. Direct memory access (DMA)

## Programmed I/O
Programmed I/O operations are the result of 110 instructions written in
the computer program. 

Each data item transfer is initiated by an instruction
in the program. Usually, the transfer is to and from a CPU register and
peripheral. 

Other instructions are needed to transfer the data to and from CPU
and memory. 

Transferring data under program control requires constant monitoring
of the peripheral by the CPU. Once a data transfer is initiated, the CPU
is required to monitor the interface to see when a transfer can again be made.

It is up to the programmed instructions executed in the CPU to keep close tabs on everything that is taking place in the interface unit and the I/O device.

In the programmed I/O method, the CPU stays in a program loop until
the 110 unit indicates that it is ready for data transfer. This is a time-consuming process since it keeps the processor busy needlessly.

This is a time-consuming process since it keeps the processor busy needlessly. It can be avoided by using an ***interrupt facility*** and special commands to inform the interface to issue an
***interrupt request*** signal when the data are available from the device. 

In the meantime the CPU can proceed to execute another program. 

The interface meanwhile keeps monitoring the device. When the interface determines that the device is ready for data transfer, it generates an ***interrupt request*** to the computer. 

Upon detecting the external ***interrupt signal***, the CPU momentarily
stops the task it is processing, branches to a service program to process the I/O transfer, and then returns to the task it was originally performing.


## DMA
Transfer of data under programmed I/O is between CPU and peripheral.

In ***direct memory access (DMA)***, the interface transfers data into and out of the memory unit through the memory bus. 

The CPU initiates the transfer by supplying the interface with the starting address and the number of words needed to be transferred and then proceeds to execute other tasks. 

When the transfer is made, the **DMA** requests memory cycles through the memory bus.

When the request is granted by the memory controller, the **DMA** transfers the data directly into memory. 

The CPU merely delays its memory access operation to allow the direct memory I/O transfer. 

Since peripheral speed is usually slower than processor speed, I/O-memory transfers are infrequent compared to processor access to memory.

## IOP
Many computers combine the interface logic with the requirements for
direct memory access into one unit and call it an ***I/O processor (IOP).*** 

The **IOP** can handle many peripherals through a **DMA** and **interrupt facility.**

In such a system, the computer is divided into three separate modules: the 
* Memory unit, 
* The CPU, and 
* The lOP.



















