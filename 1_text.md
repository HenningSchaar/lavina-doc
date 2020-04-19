# Introduction

Music generation is often times a process in which two or more entities interact and draw inspirations from the sounds created by other performers to inform their own behaviour. In the interaction between machine and performer, the machine can be seen as one such entity. 

Sound synthesisers are commonly understood as musical instruments, but with sound generating devices gaining complexity through technological advancement, they can also gain autonomy in their function as performing entities in the music generation process.

In musical improvisation this process happens while the music is being generated. However in experimental composition techniques, established through the work of composers of musique concrète, a composition is being informed by the material which is used to create it. The feedback to user input of music generation systems can act as such a material and can inform decisions about the composition in a workflow that could be understood as trial-and-error.

The nature of musical generation through interaction and feedback manifest themselves not only in the workflow with Lavina, but also in the interactions between the individual particles of the flocking system.

# Background

## Particle System

Particle systems are collections of large numbers of particles, each having its own behaviour. In models of flocking, there are three accelerating forces acting upon any given particle. [@craig_reynolds_flocks_1987]

1. Collision Avoidance: avoid collisions with nearby flockmates.
2. Velocity Matching: attempt to match velocity with nearby flockmates.
3. Flock Centering: attempt to stay close to nearby flockmates.

In the particle system Lavina uses, the finite sized birds are replaced by point objects and the velocity matching is omitted. Collision Avoidance is realised by giving the particles a charge. Similiar to charged particles in physics, there is a negative attractive force at close distances which allows the particles to avoid each other and objects in the environment. Flock Centering works via an attractive force to all other particles in the the perception radius of each particle, which scales with distance similar to gravity. [@t_m_blackwell_swarm_2002]

To allow for more chaotic behaviour and expand artistic expression the option to add random acceleration to the particles was added. A greater sense of space is achieved by the addition of the wind parameter, which allows to apply a directed acceleration to all particles.

## Experimental Composition

In the tradition of European classical music the creative process starts in the imagination of the composer. The idea is committed to notation and then performed by performers to reach its final auditory form. In the early days of electronic music in Germany, notably in the cologne studios for electronic music, this tradition of idea, notation and performance in this order was preserved. In France however, a new form of composition was being developed. The composers of *Musique Concrète* used recorded sound materials as their starting point, and tried to derive the musical essence of these materials by manipulating them, while being guided by their musical tastes and intuitions. [@brindle_new_1987 S. 108]

Working with partially autonomous sound generating systems can be seen as an extension of this french tradition. The Composer might start with an idea in mind, but the hard to predict audio engine, gives a reaction, that then requires the composer to react accordingly and find a way to adapt their composition based on their intuition and vision.

# Design

## Sonification

The sonification is based on sound objects which are choosen by the composer. They can be loaded into the software and are played back by each particle. Each particle has randomised adjustable sample offset, pitch randomisation and randomised filter curves to achieve differentiation between particles. The particles experience a simulated doppler-effect, meaning a velocity dependent pitch variation, as well as distance simulation via filter and gain adjustments that are dependant on the distance from the listening sweet spot to the particle.

The sound parameters and flocking behaviour variables can be real time adjusted, via MIDI CC input. This enables the composer to create automation curves which serve as the notation for their composition. This information is then fed to the software to create the sonification and visuals.

## Animation



# Composition

An example composition was created to help in developing and testing the tools, as well as to demonstrate them. Reaper was used to create MIDI CC output that controls the input variables of the software. The timeline consists of envelopes which are turned in to MIDI CC messages via the ReaMidiControl plugin. The audio performance is then recorded via *Soundflower* and the visualisation is recorded via a screen recorder in the Java Processing environment.

## Sound Material

The sound material for the composition was created by taking pieces of popular music that were transformed through granular synthesis with the Max/MSP project *DroneBox* [@ohland_jonasohlanddronebox-max_2019]

The pieces that were chosen for granular synthesis editing were:

1. *Guillotine* by *Death Grips*
2. *Daydreaming* by *Radiohead*
3. *Nathalie Neil* by Swans
4. *Ocean Song* by *Daughters*

The pieces were chosen based on their sonic characteristics of complexity of texture, musical consonance/dissonance and their timbre.

These pieces were used because popular music in particular has become an inescapable part of the artificial sonic environment. In this way it shapes the relationship audiences have to devices with sound generating capabilities. One of the objectives of Lavina is the exploration of musical human-machine interfaces on the side of the composer. Therefore a connection to the human-machine interface in the perception of the audience seemed fitting.

## Timeline



# Conclusion



# References



