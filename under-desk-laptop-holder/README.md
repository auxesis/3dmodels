# Under-desk laptop holder for the Dell Latitude 5531

This folder contains a pair of 3D printed arms that hold a closed laptop under a desk.
The arms fit the Dell Latitude 15 5531.
The laptop slides in from the front and rests on a shelf along each side.

The side walls of the arms are open between a post at each end.
You can plug in network, USB, HDMI and Thunderbolt cables while the laptop is in the holder.

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
  The wall is open between a post at the front and a post at the rear.
- A small stop at the rear end of the shelf stops the laptop sliding out the back.
- A shallow notch in the shelf near the rear leaves room for the network port.
  The network port has a jaw that flips down below the bottom of the laptop when you plug in a cable.

The left arm is a mirror image of the right arm, so it has the notch too.

## Sizes

These sizes come from Dell's specifications for the Latitude 5531:
357.8 mm wide, 233.3 mm deep, and 24.05 mm thick at the rear.

| Size | Value |
|---|---|
| Arm length | 230.3 mm, so the front of the laptop sticks out 3 mm to grab |
| Gap between shelf and top plate | 27.05 mm, 3 mm more than the laptop's thickness |
| Shelf depth under the laptop | 24 mm |
| Overall height under the desk | 41 mm |
| Weight of each arm | about 136 g |

To fit a different laptop, change the parameters in the SolidCraft design.
The parameters `lap_w`, `lap_d` and `lap_h` set the laptop's width, depth and thickness.
The parameters that start with `rj_` set the position of the network port notch.

## Print the arms

1. Print each arm lying on its outer wall.
   The STL files are already turned this way, so the arms print without supports.
2. Each arm needs a print bed at least 235 mm long.
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

## Check the network port notch first

The position of the network port notch is an estimate.
The notch starts 20 mm from the rear of the arm and is 45 mm long.
Dell doesn't publish where the ports are along the side of the laptop.

Before you print, measure from the back edge of the laptop to the network port.
If the port isn't between 20 mm and 65 mm from the back edge, change `rj_from_rear` in the design.
