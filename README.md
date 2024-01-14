# Quantum Mob's Woflram Language Paclet Repository

This hosts a few paclets we are maintaining:
- [Q3](https://github.com/quantum-mob/Q3App)
- [QuantumPlaybook](https://github.com/quantum-mob/QuantumPlaybook)
- WorkbookTools -- Some utilities and stylesheets for QuantumWorkbook


## Set-Up Guide

Copy the following code, and just evaluate it in your Mathematica(R) Notebook:

```Mathematica
Module[
  { ps },
  ps = PacletSiteRegister[
    "https://github.com/quantum-mob/PacletRepository/raw/main",
    "Quamtum Mob's Wolfram Language Paclet Repository"
   ];
  PacletSiteUpdate[ps]
 ]
```

## Quick Start

To install paclets, use this code:

```Mathematica
PacletInstall["Q3"]
```
Or you can replace "Q3" with other paclet you like to install.

To find available versions of the paclets, evaluate the follwoing statement:

```Mathematica
PacletFindRemote["Q3"]
PacletFindRemote["QuantumPlaybook"]
```

If you do not want to use this server any longer, then evaluate the following statements:

```Mathematica
PacletSiteUnregister["https://github.com/quantum-mob/PacletRepository/raw/main"]
PacletSiteUpdate @ PacletSites[]
```
