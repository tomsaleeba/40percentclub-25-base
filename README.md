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
- `baseplate.dxf` the baseplate

![licence logo](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)
