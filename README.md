
# English #


## Overview ##
"TAP" stands for "Teksto al parolado", which means "Text to speech" in [Esperanto](http://en.wikipedia.org/wiki/Esperanto). The goal of pytap is to produce a convincing male and female Esperanto voice.

# How it works #
* pytab is given some text
* the text is parsed into words, syllables, and characters
* a [phoneme](http://en.wikipedia.org/wiki/Phoneme) is assigned to each character, which is influenced by the position of the character in a word and the type of surrounding punctuation
* this set of phonemes is synthesized into a sound with [mbrola](http://tcts.fpms.ac.be/synthesis/mbrola.html) to produce the voice

## Usage ##


```
#!python

>>> python pytap.py -h
Usage: pytap.py -t text | -f file | -p phoneme [-o output] [-v voice] [-l language]

Options:
  -h, --help            show this help message and exit
  -t TEXT, --text=TEXT  Specify text to render
  -f FILE, --file=FILE  Choose file to read
  -p PHONEME, --phoneme=PHONEME
                        Choose a pho file
  -o OUTPUT, --output=OUTPUT
                        Specify output file for sound
  -v VOICE, --voice=VOICE
                        Choose voice
  -l LANGUAGE, --language=LANGUAGE
                        Choose language
  --pitch=PITCH         Ratio applied to pitch of voice (default 1.0)
  --speed=SPEED         Ratio applied to speed of voice (default 1.0)
  --play                Play sound that was rendered
  --voices              Display a list of all available voices
  --languages           Display a list of all available languages
>>> pytap.py -t "Saluton, mia nomo estas Maria"
>>> echo "Saluton, mia nomo estas Mario" | pytap.py -v es1 -l eo --play --pitch=0.8 --speed=0.9
```


(Download [male voice](http://pytap.googlecode.com/files/mario.wav) and [female voice](http://pytap.googlecode.com/files/maria.wav).)

## History ##
Pytap is derived from the [xAtUm](http://sourceforge.net/projects/xatum/) project.

# Esperanto #

## Super rigardo ##
"TAP" signifas "Teksto al parolado". La celo de pytap estas produkti ambaŭ vira kaj virina voĉo por Esperanto. 

## Kiel funkcias ##

* teksto estas donita al pytap
* la teksto estas analizita en vortoj, silaboj, kaj karakteroj 
* [fonemo](http://eo.wikipedia.org/wiki/Fonemo) estas asignita al ĉiu karaktero, kiu estas influita de la pozicio de la karaktero en la vorto kaj la ĉirkaŭa interpunkcio
* la fonemaro estas sintezita en sono kun [http://tcts.fpms.ac.be/synthesis/mbrola.html mbrola] por produkti la voĉon

## Uzado ##

```
#!python

>>> python pytap.py -h
Usage: pytap.py -t text | -f file | -p phoneme [-o output] [-v voice] [-l language]

Options:
  -h, --help            show this help message and exit
  -t TEXT, --text=TEXT  Specify text to render
  -f FILE, --file=FILE  Choose file to read
  -p PHONEME, --phoneme=PHONEME
                        Choose a pho file
  -o OUTPUT, --output=OUTPUT
                        Specify output file for sound
  -v VOICE, --voice=VOICE
                        Choose voice
  -l LANGUAGE, --language=LANGUAGE
                        Choose language
  --pitch=PITCH         Ratio applied to pitch of voice (default 1.0)
  --speed=SPEED         Ratio applied to speed of voice (default 1.0)
  --play                Play sound that was rendered
  --voices              Display a list of all available voices
  --languages           Display a list of all available languages
>>> pytap.py -t "Saluton, mia nomo estas Maria"
>>> echo "Saluton, mia nomo estas Mario" | pytap.py -v es1 -l eo --play --pitch=0.8 --speed=0.9

```

(Deŝuti [vira voĉo](http://pytap.googlecode.com/files/mario.wav) kaj [virina voĉo](http://pytap.googlecode.com/files/maria.wav).)

## Historio ##
Pytap estas derivita de la [xAtUm](http://sourceforge.net/projects/xatum/) projekto. 
