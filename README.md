# STRNG4DS

## Project Summary:
Use a small radioactive sample to generate true random to seed /dev/random on linux dedicated servers.

# Arduino

### Compiling Arduino:
Use Arduino IDE with modifications for your board, this prototype used the mega however many other boards should work perfectly fine.
If you are using a different board you may need to change the `interruptPin` used by `attachInterrupt`.



# Linux

### Compiling linux source to binary:
`gcc strng4ds.c -o strng4ds.out -lm`

### Running binary
You will need to use the sudo command or run as root to use the binary as it requires root to modify `/dev/random`. For example: `sudo ./strng4ds.out`

# Prototype Device
Using a Fiestaware Plate, an Arduino and a Geiger Counter we can collect truely random entropy from the decay of uranium fission decay products.
![Fiestaware Plate, Arduino and Geiger Counter](prototype.png)
