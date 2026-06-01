### Fundamentals of LTE
	- free space path loss:
	  $$P_r = P_t \frac{\lambda^2 G_t G_r}{(4 \pi d)^2}$$
	- $P_r, P_t$: received and transmitted powers. $G_t$ and $G_r$ are gains from using directional antennas
	- Empirical path loss formula (used for simple calcs):
	  $$P_r = P_t P_o \left(\frac{d_o}{d}\right)^\alpha$$
	  where $\alpha$ is the path loss exponent and $P_o$ is the power at a reference distance $d_o$
	- Service area is divided into cells. To minimize cell interference, the transmit power of base stations is regulated down to be just enough to provide the required signal strength at the cell boundaries
	- **CCI**: Co-Channel interference is an issue, cause by other user in the same cell or other cells.
	- **OCI**: Other cell interference
	- ### Timing and synchronization
		- need to determine the timing offset of the symbol, and align with the specific carrier frequency
		- channel delay spread $T_m$: a measure of the difference between the time of arrival between the earliest multipath component and the last multipath component realize
		- the timing offset $\tau$ cannot be greater than the difference between the cyclic prefix and the channel delay spread:
		  $$\tau < T_g - T_m$$
		  importantly, SNR decreases quadratically with the timing offset
	- ### FDMA and TDMA
		- Users are given a block of OFDM subcarriers, allowing for multiple users at lower datarates. We can also allocate timing slots to users as well, combining FDMA and TDMA into one thing
	- ### OFDMA
		- allocate time-frequency slices to subscribers (LTE Resource grids). Consists of M subcarriers over some number of consecutive OFDM symbols (usually 7)
		-
		-
	- ### SC-FDMA
		- SC-FDMA is used in the uplink because it has a lower PAPR, allowing UE amplifiers to work more efficiently.
	-
-
- [LTE Receiver, Demel](https://www.cel.kit.edu/download/SDR-WInnComm-Europe-2013_DemelKoslowskiJondral.pdf)
-
- ### Definitions:
	- UE: User Equipment
	- OFDMA: OFDM Access
	- eNodeB: Evolved Node B. This is the network hardware/base station
	- GPP: General Purpose Processor
	- PLMN: Public Land Mobile Network
	- SINR: Signal to interference plus noise ratio
	- S/P: serial to parallel
	- CSI: Channel state information
	- AMC: adaptive modulation and coding
	-
-
- What is LTE (from Matlab website):
	- LTE was developed b the Third Generation Partnership Project (3GPP)
	- 2G is GSM and 3G is UMTS
	- LTE uses OFDMA, where the spectrum is divided into resource blocks
		- each block is composed of twelve 15 kHz subcarriers
		- supports up to 64-QAM and bandwidth allocation of up to 20MHz
	- LTE Radio access network is comprised of the following protocols:
		- Packet Data Convergence Protocol (PDCP)
		- Radio Link Control (RLC)
		- Mediam Access control (MAC)
		- The Physical Layer (PHY)
-
- LTE Procedure
	- when the UE first powers on, it tunes to the available