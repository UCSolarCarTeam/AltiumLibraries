# AltiumLibraries
Libraries used in development of PCBs for the University of Calgary Solar Car Team

**Note:** These libraries are under active development. We are in the process of consolidating legacy components to our newer format.
If there is legacy content that you think should be updated to reflect the new format, please create an issue.


## Conventions
### Schematic Libraries
#### Part Naming Convention:
A custom part numbering system is being implemented. Currently, it is primarily used for generic resistors and capacitors.

There are three fields:   `AAAA-BBBBB-CC`

The theory behind the part numbering system is hierarchical; `A` values are the most common similarities, followed by `B` unique attributes, followed by `C` variants.


**Example** -  naming a 120 Ohm, 0603 resistor with 5% tolerance and a 63mW power rating:
- Field A:
  - Used for **component type and package**. Our example resistor will fall under the same 'A' field as all other 0603 resistors. The 'A' field is: `R060`
- Field B:
  - Used for **unique component features**. This field separates our example resistor from all other resistors with the parent field of `R060`. The 'B' field is: `00121`. `121` means `12 * 10^1 Ohms`. Note that in this instance, the leading `00` does not have any meaning. It is used as filler. Also notice that the power rating is not considered. This will usually not vary substantially for a resistor of a set resistance and package, so we don't give it a unique part number based on power rating.
- Field C:
  - Used for **component variants**. Our example resistor now has an identifying part number to show that it is a 120 Ohm 0603 resistor: `R060-00121-xx`. The variant field is now used to specify the tolerance. In this case, 5%: `-05`.
  
Our full part number is now: `R060-00121-05`.

### PCB Libraries
< Need content here >
