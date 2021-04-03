# PacletServer

This hosts a few paclets I am maintaining:
- [Q3](quantum-mob/Q3App)
- [QuantumWorkbook](quantum-mob/QuantumWorkbook)


## Set-Up Guide

Copy the following code, and just evaluate it in your Mathematica(R) Notebook:

```Mathematica
Module[
  { ps },
  ps = PacletSiteRegister[
    "https://github.com/quantum-mob/PacletServer/raw/main",
    "Quamtum Mob Paclet Server"
   ];
  PacletSiteUpdate[ps]
 ]
```

## Quick Start

To install paclets, use this code:

```Mathematica
PacletIntall["Q3"]
```
Or you can replace "Q3" with other paclet you like to install.

To find available versions of the paclets, evaluate the follwoing statement:

```Mathematica
PacletFindRemote["Q3"]
PacletFindRemote["QuantumWorkbook"]
PacletFindRemote["WorkbookTools"]
```

If you do not want to use this server any longer, then evaluate the following statements:

```Mathematica
PacletSiteUnregister["https://github.com/quantum-mob/PacletServer/raw/main"]
PacletSiteUpdate @ PacletSites[]
```
