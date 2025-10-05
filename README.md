# concertc: the music compiler

concertc is a program that converts a new kind of music file to a lilypond file (can be converted to sheet music).

## usage

`concertc src.concert dest.ly (C|Bb|Eb|F) {pitch offset} (treble|bass)`

 - src.concert: name of source file
 - dest.ly: name of destination file
 - (C|Bb|Eb|F): type of instrument
 - {pitch offset}: start at 0, and tweak as needed for instrument
 - (treble|bass): type of clef

## example

For Bb clarinet:

`concertc happy-birthday.concert hb.ly Bb 1 treble`
