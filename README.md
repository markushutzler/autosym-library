Symbol Definitions
==================

Schematic symbol descriptions are used to simplify the creation of schematic symbols. It also gives the opportunity to generate symbols for different schematic design applications.

Each file contains 'description' , 'options', 'footprints', 'variants' and mapping.

Description
-----------

The description section defies the basic properties of the device. Use key=value format.

 - `fileversion`: The definition file version. We suggest to set it to 1.
 - `refdes`: The default refdes value.
 - `device`: The name of the created files.
 - `description`: Will be added into the sym file.
 - `documentation`: Will be added into the sym file.
 - `symversion`: Will be added into the sym file.
 - `author`: Will be added into the sym file.
 - `dist-license`: Will be added into the sym file.
 - `use-license`: Will be added into the sym file.
 - `category`: Will be used to organise the symbols in folders.

Options
-------

The options section defies the rendering properties of the device. Use key=value format.

 - `pin_length`: Defines a custom pin length. (default=300)
 - `pin_grid`: Defines a custom pin grit. (default=200)
 - `symbol_width`: Defines a custom symbol minimum width. (default=1000)

Variants
--------

Variants are used to define different pin mapping options. Components distributed in different packages may have a different pin number mapped to different functions. Define one variant for each mapping.

The filename of the created symbol  will be: "`device` + `variant` + .sym". 
The first column defines the add-on to the generated file name. The second 
column is added to the `description` parameter.

footprints
----------

Mapping
-------

The mapping is used to map pins of the symbol. Each newline adds a new row. The pin number is set in the first column. Each package variant needs a pin number. Use a '-' if a pin is not used. The second column defines the name. You can use a "!" to add a line over the name. The third column defines the pin function.
