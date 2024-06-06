# T0 The bare-bones test if RELAP5-3D will run

## Step 1 - Load the RELAP5-3D module
### On your machine
We don't know how you do this. Please contact the relevant people in your
organization.

### On INL High Performance Computing machines
Pick a folder where you want to put the tutorial files. Then load the
`relap53D` module using

```
module load relap53D/relap53D
```

## Step 2 - Clone the bare-bones test input

Execute
```
git clone https://github.com/RELAP5-3D-UserCommunity/Tutorial0.git
```
and after this command completes,
```
cd Tutorial0
```

## Step 3 - Execute the input
We have three arguments we want to pass
- `-i Filename`, specifies the input file to use
- `-O OutFilename`, specifies an **overwritable** output file name
- `-tpfdir FluidDirectoryName`, specifies where the fluid property directory is
located at

For this tutorial we are going to use
```
relap53D -i Tutorial0.i -O Tutorial0.o -tpfdir /opt/relap53D_fluids
```
