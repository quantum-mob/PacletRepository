# PacletServer
This hosts a few paclets I am maintaining.

- Q3App
- QuantumWorkbook

## How to use this paclet server

On Mathematica(R), evaluate the following statements:

```Mathematica
PacletSiteRegister["https://github.com/quantum-mob/PacletServer/raw/main"]
PacletSiteUpdate[PacletSites[]]
```

To find available paclets, evaluate the follwoing statement:

```Mathematica
PacletFindRemote["Q3"]
PacletFindRemote["QuantumWorkbook"]
```

If you do not want to use this server any longer, then evaluate the following statements:

```Mathematica
PacletSiteUnregister["https://github.com/quantum-mob/PacletServer/raw/main"]
PacletSiteUpdate[PacletSites[]]
```
