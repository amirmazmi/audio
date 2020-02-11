# audio
general audio processing or commands
<br><br>



### Package to play beeps
```sudo apt install sox```
<br>  

### Package to play all music format
```sudo apt install libsox-fmt-all```
<br>  

### Package to read test
```sudo apt install espeak```
<br><br>


## Examples
Command to play beeping songs
```
play -q -n -t alsa synth 0.5 sin 1000 vol 0.7
```
```
for i in {1..10}; do play -q -n -t alsa -v 0.1 synth 0.5 sin 1000; sleep 0.2; done
```
<br>

Command to read text
```
espeak -p 15 -g 4 -s 140 "I am now self aware"
```
<br><br>

List all input devices  
```pacmd list-sources```  

Commad to mute/unmute  
`pacmd set-source-mute <device index> <mute boolean>`  
```pacmd set-source-mute 1 0```



