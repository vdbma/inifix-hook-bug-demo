# inifix-hook-bug-demo

Behaviour :

```
$ git commit idefix.ini -m'Added ini file'
Format .ini files........................................................Failed
- hook id: inifix-format
- exit code: 1

Fixing idefix.ini
[Grid]

X1-grid                       1  0.01  64  l  0.62
X2-grid                       1  0.0  128  u  6.283185307179586
X3-grid                       1  -0.0125  1  u  0.0125


[Streamer]

# streamerCs                    .0755
# streamerDensity               1.
# streamerWidth                 .1
# streamerVelocity              0.0755


[Output]

vtk                           0.1
dmp                           100.0
log                           100.0
analysis                      0.01                                              # format de sortie personnel
sampleNumber                  10
```
Note that the output is properly formated but the actual `idefix.ini` file is not.
