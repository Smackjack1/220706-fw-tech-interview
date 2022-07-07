# Firmware Engineering Tech Interview

> What are checksums and what are they useful for?

> Checksums are used to check for errors that may have occured during the transfer of a data packet.
	Depending on the size of data and algorithm used, the checksum can be a single bit or a larger number.
	The receiver of the packet caclulates and compares the checksum of the data received to the checksum 
	calculated by the sender. If these do not match, an error has occured.
	