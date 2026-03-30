# SUAV-Avionics

As one of the Avionics Co-Leads for the Schulich Unmanned Aerial Vehicles design team, there are a good number of projects I've worked on directly and indirectly. With the team having cycles of development; making a new plane every few years or every other year, there is a constant influx of new projects.

## Mako Avionics Integration
This is an ongoing proceess, we'll see how it goes!

## Power Distribution Board v2
Since the failure of the last power distribution board, this one took the lessons learned. Rather than overcomplicating and letting scope creep get the better of us, we kept things simple and aimed for reliability. This time we added multiple current sensors, a COTS DC-DC converter, a fuse, and specific connectors for the various avionics (flight controller, Raspberry Pi, etc.).

<div align="center">
  <img src="https://github.com/user-attachments/assets/0b1892b1-54a3-4433-a2d6-3fe30746be34" width="300" alt="Assembled Optipong">
  <p>Testing the power test board</p>
</div>

From testing, the new PDB accomplishes it's intended role, it is currently in the proceses of being integrated with the new plane, Mako.

## Orca Avionics Integration
With no time to continue making the power distribution boards, focus was all in on integrating the avionics to get Orca ready for competition. This involved wiring and testing flight controllers, pitot tubes, radios, pitot tubes, GPSes, batteries, and servos, sometimes on the tarmac when things went very wrong. In the peak of crunch time, I would work my 8 hour internship, then pull up to school for another 8 hour shift troubleshooting and fixing things.

<div align="center">
  <img src="https://github.com/user-attachments/assets/bab6b80d-0eab-4327-a3de-47029ce30558" width="300" alt="Assembled Optipong">
  <p>Orca after the first crash</p>
</div>

This was definitely a move fast break things operation, as with the looming deadlines we had to work quickly. 

<div align="center">
  <img src="https://github.com/user-attachments/assets/fd3685f5-096a-4c9b-858d-79a45f5ee3fc" width="300" alt="Assembled Optipong">
  <p>More finalized and majestic Orca</p>
</div>

Ultimately competition didn't end well as we had motor burnout issues with the heat, but we learned a ton along the way.

## Power Distribution Board v1
This was designed to replace all the separate BECs while also providing software control and power telemetry to the ground. This was an overly ambitious board that eventually ran out of time. Thus it stays as just a design.

## Power Test Board
When I first joined the team, we had a mess of batteries, wiring, and battery eliminator circuits powering everything. Thus we wanted to make a custom power board to optimize our systems, and to clean up our wiring. We wanted a board that could also be software controlled, so we wanted to use a FET as a main connector/disconnector. Since ESCs eat up high currents, our board and components would need to be rated for those high powers. Thus we made a test board to see how capable our components were.

<div align="center">
  <img src="https://github.com/user-attachments/assets/539733d8-84b1-4f6b-bd4d-6314530b3475" width="300" alt="Assembled Optipong">
  <p>Testing the power test board</p>
</div>

Unfortunately, an issue we only realized once the board had been manufactured and shipped was that the footprint of the FETs we chose was wrong. We blindly trusted the built in Altium library part, so we found the components did not fit the footprint at all. We had to flywire the high power FET, which obviously would lead to poor thermal performance. From this experience, we have made sure to always double check footprints for components before ordering.

## Other Things

<div align="center">
  <img src="https://github.com/user-attachments/assets/510757ae-00a4-4059-8dd9-6618afd523d6" width="300" alt="Assembled Optipong">
  <p>Troubleshooting a dead Li+ battery charger</p>
</div>

<div align="center">
  <img src="https://github.com/user-attachments/assets/43ae3f17-72f3-498c-80d5-b53b204efc7f" width="300" alt="Assembled Optipong">
  <p>Motor test rig</p>
</div>

<div align="center">
  <img src="https://github.com/user-attachments/assets/9ce96a42-8163-45d2-9fd1-d67acb1dd2f7" width="300" alt="Assembled Optipong">
  <p>Last minute surgery to replace the antenna on our controller</p>
</div>



