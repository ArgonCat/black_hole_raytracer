# black_hole_raytracer

## What?
A beam-marching based renderer which can simulate gravitational lensing and a transparent accretion disc!

## Why?
To learn numpy broadcast semantics and make cool images.

## How?
Beam Marching... we simulate light as particles, taking steps scaled by the distance to the nearest object. This means we can define objects using only SDFs.
Using numpy for this project has some unique challenges - we can't do shadow/light rays, as there's no way to recurse/split the particle once our tensor is initialised. This isn't a practical way of making a raytracer but it was certainly fun! We also have no way of stopping a ray when we hit something - we instead have to perform calculations for particles even if they've hit an object.

Inspired by:
https://github.com/kavan010/black_hole
https://www.youtube.com/watch?v=Cp5WWtMoeKg

## Gallery
