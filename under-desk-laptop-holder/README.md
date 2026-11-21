# Under-desk laptop holder for the Dell Latitude 5531

This folder contains a pair of 3D printed arms for keeping a closed laptop under a desk.
The arms fit the Dell Latitude 15 5531.
The laptop slides in from the front and sits on a shelf along each side.
Each arm prints in one piece on a 180 mm print bed, such as the Bambu Lab A1 mini.

The side walls of the arms are open alongside the laptop's ports.
You can plug in network, USB, HDMI, and Thunderbolt cables while the laptop is in the holder.
In front of the ports, the walls have a honeycomb of hexagonal holes for extra support.

## Inspiration

This design was inspired by [Under Desk Laptop Holder](https://makerworld.com/en/models/127452-under-desk-laptop-holder) by [@KG3Dee](https://makerworld.com/en/@KG3Dee) on MakerWorld.
That model's side supports block the ports on the right side of the laptop.
This is a new design, drawn from scratch from the laptop's published dimensions.
It does not use any geometry from the original model.

## Files in this folder

| File | What it contains |
|---|---|
| `right-arm.stl` | The arm for the right side of the laptop, ready to print |
| `left-arm.stl` | The arm for the left side of the laptop, ready to print |
| `under-desk-laptop-holder.sc` | The editable SolidCraft design of both arms |

## How the arms are shaped

Seen from the front, each arm is shaped like the letter C.

- The top plate screws to the underside of the desk.
- The shelf at the bottom holds the laptop.
- The outer wall joins the top plate to the shelf.
  The wall is open from 12 mm to 145 mm from the laptop's back edge, where the ports are.
  In front of that opening, the wall has 3 hexagonal holes in 2 staggered rows: 2 below and 1 above.
  The plastic between the holes supports the front of the arm.
- A small stop at the rear end of the shelf stops the laptop sliding out the back.
- A shallow notch in the shelf near the rear leaves room for the network port.
  The network port has a jaw that flips down below the bottom of the laptop when you plug in a cable.

The left arm is a mirror image of the right arm, so it has the notch too.

## Sizes

These sizes come from Dell's specifications for the Latitude 5531:
357.8 mm wide, 233.3 mm deep, and 24.05 mm thick at the rear.

| Size | Value |
|---|---|
| Arm length | 172 mm, or 176 mm with the rear stop |
| Laptop past the front of the arms | about 61 mm, to grab |
| Gap between shelf and top plate | 40.05 mm, 16 mm more than the laptop's thickness |
| Shelf depth under the laptop | 24 mm |
| Overall height under the desk | 54 mm |
| Weight of each arm | about 106 g |

To fit a different laptop, change these parameters in the SolidCraft design:

- `lap_w`, `lap_d`, and `lap_h` set the laptop's width, depth, and thickness.
- `L` sets the arm length. Keep `L` plus 4 mm for the rear stop shorter than your print bed.
- The parameters that start with `rj_` set the position of the network port notch.
- `port_end` sets where the port opening ends, measured from the laptop's back edge.
- The parameters that start with `hex_` set the size, spacing, and number of the hexagonal holes.

If you make the port opening longer, use fewer hexagonal holes, so the holes do not run into the opening.

## Print the arms

1. Print each arm lying on its outer wall.
   The STL files are already turned this way, so the arms print without supports.
2. Each arm needs a print bed at least 176 mm long.
   It fits the 180 mm square bed of the Bambu Lab A1 mini.
3. PETG suits this part, because PETG bends less than PLA under a steady load over time.

## Fit the arms to the desk

The arms screw to the desk with 3 wood screws each.
The screws are 4 mm wide, with a head no wider than 9 mm.
Each screw passes through 3 mm of plastic under its head, then into the desk.
Choose screws at least 5 mm shorter than the thickness of the desk, so they don't come through the top of the desk.
For example, use 16 mm screws for a 25 mm desk.

1. Hold the right arm under the desk, with the open side of the C facing the laptop.
   The rear stop goes at the back.
2. Screw the right arm to the desk.
3. Put the inner faces of the two walls 359.8 mm apart.
   This leaves a gap of 1 mm on each side of the laptop.
4. Screw the left arm to the desk.
   The screw slots let you move each arm 4 mm sideways each way before you tighten the screws.
5. Slide the closed laptop in from the front, until it touches the rear stops.

## The network port notch

The notch runs from 20 mm to 65 mm from the back edge of the laptop.
This position was checked on a real Latitude 5531.

On that laptop, the ports on the right side run from 26.5 mm to 137 mm from the back edge.
These measurements leave out the lock slot.
The network port is the port nearest the back edge, so it starts 26.5 mm from the back edge.
That is 6.5 mm inside the notch.

All the ports are inside the open part of the wall.
The opening ends 145 mm from the back edge.
That leaves 8 mm in front of the SD card slot for your finger.

If you change the design for a different laptop, measure from its back edge to its network port.
If the port is not between 20 mm and 65 mm from the back edge, change `rj_from_rear` in the design.
