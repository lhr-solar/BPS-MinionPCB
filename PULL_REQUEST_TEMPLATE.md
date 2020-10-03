# Quality Assurance Checklist
To make reviews more efficient, please make sure the board meets the following standards and check everything off once the board meets the quality check. Once everything has been checked, the assigned reviewers will begin the review process. _Edit this description to check off the list._

There are exceptions with all guidelines. As long as your decisions are justified, then you are good! Contact the reviewers or the leads about any exceptions.

### Minimum Prerequisites
- [X] Pushed changes to branch.
- [ ] The board passes ERC and DRC.
    - Note some ERC warnings are acceptable.
- [ ] All traces are routed.
- [ ] Units are in metric.

### 2D Spacing
- [ ] The components are spaced out at an optimal distance.
    - All components can be easily hand-soldered.
    - IPC-SM-782A Standard requires a minimum distance of 1.0mm from edge to edge.
- [ ] Components that are in parallel with each other are spaced out at an equal distance when possible.
- [ ] The components are aligned with each other when possible.
- [ ] Components are grouped based off of functionality.
    - E.g. all components for CAN should be grouped.
- [ ] Bypass capacitors are less than 1cm away from their respective IC's power pins.

### 3D Spacing
- [ ] Layout of components have been placed with mounting location and usage of the board in mind.
    - Are PCBs going to be stacked on above/below this board? Are tall components placed accordingly?
    - Are buttons and lights easily accessible and viewable?
    - When mounted into the car, are the heights of the components and connectors accounted for?
- [ ] Location of connectors and wires going out of the board will prevent messy wiring.
    - Are all the wires that are going in the same direction placed on the same edge of the board?

### Components
- [ ] Custom footprints have been double checked with the datasheet.
- [ ] Pin 1 of the footprint is labeled in some way.

### Copper Layer
- [ ] The trace widths and trace clearances are greater than JLCPCB's minimum requirements.
- [ ] The trace lengths are as short as possible.
    - Can there be a more optimal route if you go to another layer?
- [ ] Each trace's width is capable of handling the expected current flow.
    - Use PCB width calculator to calculate trace width.
- [ ] *No sharp corners. No trace angles equal to or less than 90 degrees.
- [ ] Traces are in parallel with each other when possible.
    - E.g. traces connected between an IC and MCU can be placed in parallel with each other.
- [ ] There are no random trace appendages.
- [ ] Vias placed in copper pads are fully encompassed in the copper pads.
- [ ] Through-hole components do not have extraneous vias.

*Not really a problem for modern manufacturing techniques but good practice and important for high speed signal integrity.

### Silkscreen Layer
- [ ] Visible text sizes are greater than JLCPCB's minimum requirements.
- [ ] All visible text is on the silkscreen layer.
- [ ] All reference labels of each component are not overlapping a copper pad or another component.
- [ ] All connector pins are labeled with a meaningful and helpful name.
- [ ] All LEDs are labeled with a meaningful and helpful name.

### Edge Cut Layer
- [ ] The dimensions of the board and the mounting holes are nice values in metric i.e. no long decimals.
- [ ] The physical outline of the board is on the edge cut layer.
- [ ] Edge cuts are straight and parallel with opposite edge of the board.
- [ ] Mounting holes are aligned.
- [ ] Corners are curved and contoured to mounting holes.

### IMPORTANT NOTICE
- [ ] I am confident that this board will be safe to use in a safety critical environment.
- [ ] I had fun :)

## Other Comments
_Write any comments about the board that would help the reviewers here._