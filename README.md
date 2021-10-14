# setupEnvironment
In this repo i upload my setup instructions.....

## VGA_Monitor.sh :-

Step 1 :- This to Check The Resolution Setting

    gtf 1920 1080 60

Step 2 :- This is For Adding New Mode using Xrandr

    xrandr --newmode "1920x1080_60.00"  172.80  1920 2040 2248 2576  1080 1081 1084 1118  -HSync +Vsync

Step 3 :- This For configure the Setting to your desktop environment
    
     xrandr --addmode VGA-1 "1920x1080_60.00"

Step 4 :- This is to Forcefully Generate the output
    
    xrandr --output VGA-1 --mode "1920x1080_60.00"