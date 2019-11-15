> a custom base plate for the "25 by 40percentclub" keyboard that supports extra
> switches

Gerber files for keyboard available at: https://git.40percent.club/di0ib/Misc/src/branch/master/25

I converted the .GTL gerber file using [these instructions](https://electronics.stackexchange.com/a/391476/37121):
```bash
gerbv -x ps Gerber_drill.GTL
GS_OPTIONS=-dNOSAFER pstoedit -f dxf output.ps Gerber_drill.GTL.dxf
```

# Files
- `Gerber_drill.GTL.dxf` original top copper from Gerber converted to DXF as-is
- `baseplate-master.dxf` master design of the baseplate, that includes
    construction lines, etc
- `baseplate-readytocut.dxf` a "ready to cut" design that is generated from the
    master

# TODO
  - change sizes of holes to 2.1mm as the existing holes are from the copper
      layer so they include the keepout distance.
  - add extra switch holder parts

![licence logo](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)
