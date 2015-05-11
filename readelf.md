# readelf

Get information stored inside executable files in a human readable way.

See all information:

    readelf -a a.out

TODO understand all the information, and therefore the entire elf format.

To show only specific informations:

## s

Symtable of elf, `.o` or `.so`.

## d

Show only dependencies of an executable (symbols and shared libraries).

- `NEEDED`: direct `.so` dependencies <http://stackoverflow.com/questions/6242761/how-do-i-find-the-direct-shared-object-dependencies-of-a-linux-elf-binary>. `.so` can also depend on other `.so`. To recursively list all dependencies, use `ldd`.