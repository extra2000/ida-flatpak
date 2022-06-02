# ida-flatpak

Hex Rays IDA Flatpak.


## Building

Build using the following command:
```
flatpak run org.flatpak.Builder --user --install --force-clean build-dir io.extra2000.hexrays.ida.yml
```

Put IDA installer into `~/.var/app/io.extra2000.hexrays.ida/data/`. Make sure to allow execution for example:
```
chmod a+x ~/.var/app/io.extra2000.hexrays.ida/data/idafree77_linux.run
```

Then install using the following command:
```
flatpak run --command=data/idafree77_linux.run io.extra2000.hexrays.ida
```

Set installation path to `~/data/idafree-7.7`.


## Running

Create a work directory for example `Documents`:
```
mkdir -pv ~/.var/app/io.extra2000.hexrays.ida/data/Documents
```

Copy any binary into `~/.var/app/io.extra2000.hexrays.ida/data/Documents/`.

```
flatpak run --command=data/idafree-7.7/ida64 io.extra2000.hexrays.ida
```
