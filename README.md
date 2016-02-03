Symbol Definitions
==================


description
-----------

The description section defies the basic properties of the device.

 - `fileversion`: The definition file version. We suggest to set it to 1.
 - `refdes`: The default refdes value.
 - `device`: The name of the created files.
 - `description`: Will be added into the sym file.
 - `comment`: Will be added into the sym file.
 - `documentation`: Will be added into the sym file.
 - `symversion`: Will be added into the sym file.
 - `author`: Will be added into the sym file.
 - `dist-license`: Will be added into the sym file.
 - `use-license`: Will be added into the sym file.
 - `category`: Will be used to organise the symbols in folders.

options
-------

 - `pin_length`: Defines a custom pin length. (default=300)
 - `pin_grid`: Defines a custom pin grit. (default=200_
 - `min_widt`: Defines a custom symbol minimum width. (default=400)

variants
--------

Variants are used to create symbols for different packages. The filename will be: "`devicename` + `variant` + .sym"
The first column defines the add-on to the generated file name. The second column is added to the `description` parameter.

mapping
-------

The mapping is used to place pins in the symbol. Each newline adds a new row. The pin number is set in the first column. Each package variant needs a pin number. Use a '-' if a pin is not used.
The second column defines the name. You can use a "!" to add a line over the name.
The third column defines the pin function.
