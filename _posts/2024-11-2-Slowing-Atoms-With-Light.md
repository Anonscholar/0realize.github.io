---
title: Slowing Atoms with Light
date: 2024-11-2 0:04:00 +0530
categories: [Journey, STEM]
author: 0realize
tags: [journey, physics]
pin: false
description: How Doppler Laser Cooling slows atoms with light physics.
math: true
toc: true
comments: true
---

Imagine trying to "catch" atoms zooming around in all directions, each moving
with random, often incredibly high, velocities. To tame them, physicists use
laser cooling — a method that literally cools down atoms by hitting them with
light! Specifically, Doppler cooling makes use of the Doppler effect (yep, that
same effect that makes an ambulance’s siren pitch change as it passes by) to
reduce the speed of atoms. In this post, we'll look at how Doppler cooling works
and how it was approached in the IPhO  2009 problem on Doppler laser cooling and
optical molasses.

## The Basics: Doppler Effect and Laser Cooling

Laser cooling relies on the idea that light can “push” atoms, but only when the
light's frequency matches the energy needed for the atoms to absorb it. This
frequency depends on the Doppler effect because the atoms are moving. When an
atom moves toward a laser, it experiences the laser light as a bit 'bluer'
(higher frequency), which nudges it closer to resonance. When the atom moves
away, the light shifts 'redder' (lower frequency), and it’s harder for the atom
to absorb it. This effect lets us selectively slow down atoms moving toward a
laser.

Mathematically, for an atom moving with speed $v$ towards a laser source with
frequency $\omega_{L}$, the frequency it "see" will be:

$$\omega^{\prime}=\omega_L\left(1+\frac vc\right)$$ where $c$ is the speed
of light.

When we tune the laser frequency $\omega_{L}$ just below the atomic transition
frequency $$\omega_0$$, only atoms moving toward the laser get close enough to
resonance to absorb photons. This interaction results in a "kick" that slows
down the atom.

## The "Kick" from photon absorption

Here's the fun part: when an atom absorbs a photon, it gains the photon's
momentum. For a photon with wavelength $\lambda$ and frequency $$\omega$$, the
momentum $p$ is given by: 
$$p=\hbar k=\frac h\lambda$$ 
$ \hbar $ being the reduced Planck's constant, and $k=\frac{2\pi}\lambda$ being the wavenumber.
This extra momentum adds to the atom’s own, and if the photon travels opposite
to the atom’s motion, it slows down the atom by exactly this amount.

So, if the atom’s original momentum is $ mv $, then after the absorption of the
photon, its momentum becomes $$p_{\mathrm{atom}}=mv-\hbar k$$

This process might not look like much at first, but remember, we’re dealing with
an atomic scale here, so small changes in momentum add up over thousands of
cycles.

## The Role of Spontaneous Emission

After absorbing a photon, the atom eventually releases this energy by emitting
another photon. But here’s the twist: the direction of emission is random. This
randomness is essential because, while the photon absorption always slows the
atom, emission doesn’t entirely undo it. Over many cycles of absorbing and
emitting, the atom’s net speed decreases, leading to cooling.

The combined force from this cycle is known as the radiation force, and it can
be expressed as: $$F=R\cdot\hbar k$$ with $ R $ being the photon absorption
rate. This force is what we rely on to slow down (or “cool”) the atoms.

## Cooling with Counter-Propagating Lasers: Optical Molasses

One laser beam would only slow atoms moving in one direction. But by using two
beams moving in opposite directions, we can capture atoms moving in both
directions, creating a viscous-like environment called optical molasses. This
setup makes atoms feel like they’re moving through “thick syrup,” where every
direction of movement encounters resistance. The effect creates a damping force
that can significantly reduce the atoms' speed.

For low velocities, this damping force (or frictional force) becomes
proportional to the atom’s velocity: $$F=-\alpha v$$ here $ \alpha $ depends
on factors like detuning, laser intensitiy, etc. This is why we call it optical
“molasses”—atoms are effectively slowed in all directions, like they’re stuck in
a sticky substance.

## Limits of Doppler Cooling: The Doppler Temperature

Now, there’s a limit to how cold we can get the atoms using Doppler cooling
alone, known as the Doppler limit. At this point, the cooling force from the
laser balances with the heating effect from the random emission directions. The
Doppler temperature $$T_D$$ is given by: $$T_D=\frac{\hbar\Gamma}{2k_B}$$
where $ \Gamma $ is the natural line-width of the atomic transition (basically,
a measure of how quickly the atom can absorb and re-emit photons), and $$k_B$$
is the Boltzmann constant. For common atoms like rubidium or cesium, this limit
is around a few microkelvins, which is impressively cold but still above
absolute zero.