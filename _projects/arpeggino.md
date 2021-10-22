---
layout: project
title: Arpeggino
description: Arduino based MIDI arpeggiator, sequencer, recorder and looper
permalink: /projects/arpeggino
time: Sep 2019 - Aug 2020
logo: arpeggino.png
---

Arpeggino is an Arduino based MIDI arpeggiator, sequencer, recorder and looper.

A detailed step-by-step tutorial on how to build it is available on [GitHub](https://github.com/razrotenberg/Arpeggino#tutorial) and on [Arduino Project Hub](https://create.arduino.cc/projecthub/razrotenberg/arpeggino-midi-arpeggiator-sequencer-recorder-and-looper-5aeb7b).

<span class="highlight">[Check out the tutorial](https://create.arduino.cc/projecthub/razrotenberg/arpeggino-midi-arpeggiator-sequencer-recorder-and-looper-5aeb7b){:target="_blank"}</span>

Having studied Computer Science, I wanted to experiment with technology other than software.
I love music, and I was intrigued to know how it is represented digitally.
This led me to learn [DSP](https://www.coursera.org/learn/dsp1){:target="_blank"},
and after a few weeks of studying, I started to look for a project idea that would involve both music and technology.

I ran into [this](https://create.arduino.cc/projecthub/dra/arduino-midi-arpeggiator-3bd731){:target="_blank"} Arduino project and even though MIDI is not proper DSP,
it was immediately clear to me that I want to build a MIDI sequencer myself.

Back then I knew nothing about Arduino or electronics.
I did not know how to begin the project, and I was certain that I would not get to the level of the project I took inspiration from.
I started by playing a single note via MIDI, then chords, scales, and arpeggios.
By the time more and more ideas came to me, such as having an LCD, supporting dynamic configuration, recording and looping, etc.

During the development of Arpeggino, I learned a lot about Arduino and electronics, MIDI, and music theory,
and I was fascinated by how code and music theory seamlessly integrate.

Arpeggino consists of three sub-projects:
* [Controlino](https://github.com/razrotenberg/Controlino){:target="_blank"} - An Arduino library for using complex gestures of input controls behind a multiplexer.
* [Midier](https://github.com/razrotenberg/Midier){:target="_blank"} - An Arduino library for playing, recording, looping and programming MIDI notes, arpeggios and sequences. This is the engine behind Arpggino, that lets it do all the musical and rhythmical stuff.
* [Arpeggino](https://github.com/razrotenberg/Arpeggino){:target="_blank"} - An Arduino sketch responsible for the I/O controls, LCD, serial connection, etc.

<div class="youtube-container">
    <iframe src="https://www.youtube.com/embed/HbMf0oO-zfE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
