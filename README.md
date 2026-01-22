# My-Stuff
Lots of things.

Don't try to read the source code its a disaster lmao.

# Update 21/01/2025 ( DD/MM/YYYY )

I'm not actively maintaining this and haven't writen a Java project in a long time. I also don't have the time nor drive to play this game the way I used to, but when I did, I used this tool a lot. It bulk converts `.sm` files and applies a series of 'rates' to the files attaching in query tags to make filtering the files in-game a trivial thing. 

So you can type `MSD>20` to get files where the overall rating is above that value, you can exclude rates with `rate:n` my most common query was `rate:n msd>25 msd<31`. You could also filter by skillset using `Skill!` i.e., `JS!` and `CHJ!` for jumpstream oriented or chordjack oriented maps. My most used query became `STR!` I also believe that `!Skill` was used for the inversion which meant 'this skill is not the max for the map' so `!JS !HS !STAM !JA !CHJ !TECH` would be the same as `STR!` I never really used this feature but its still there. Same with sum debug artifacts like `offset:positive` which was used to debug audio offsets. Since for files where the delay was negative we needed to audio silence to the start of the audio file; positive numbers was a simple seek-forward into the audio file.

Here is an example tag generated:

`Tags:rate:y:1.15,offset:positive,diff:1,pack:no,!STR,!JS,!HS,!STAM,!JA,!CHJ,TECH!,MSD>?,MSD:30,STR:28,JS:21,HS:18,STAM:24,JA:22,CHJ:14,TECH:30,MSD>12,MSD>13,MSD>14,MSD>15,MSD>16,MSD>17,MSD>18,MSD>19,MSD>20,MSD>21,MSD>22,MSD>23,MSD>24,MSD>25,MSD>26,MSD>27,MSD>28,MSD>29,MSD>30,MSD<31,MSD<32,MSD<33,MSD<34,MSD<35,MSD<36,MSD<37,MSD<38,MSD<39,MSD<40`

You could also see in that list msd>? which was added as a 'this file is a convert' query. You can also see how the `rate:y` query differs slightly, this was used to select a specific rate so `rate:y:1.15` would be 1.15x

Here is the baserate tags for the same file:

`Tags:rate:no,offset:positive,diff:1,pack:no,!STR,!JS,!HS,!STAM,!JA,!CHJ,TECH!,MSD>?,MSD:27,STR:24,JS:19,HS:15,STAM:22,JA:19,CHJ:12,TECH:27,MSD>12,MSD>13,MSD>14,MSD>15,MSD>16,MSD>17,MSD>18,MSD>19,MSD>20,MSD>21,MSD>22,MSD>23,MSD>24,MSD>25,MSD>26,MSD>27,MSD<28,MSD<29,MSD<30,MSD<31,MSD<32,MSD<33,MSD<34,MSD<35,MSD<36,MSD<37,MSD<38,MSD<39,MSD<40`

Another thing in there is for multi-difficulty maps we encode a 1-based value as the difficulty number. In the game these files are shown in greek numerals

![screenshot5480](https://github.com/user-attachments/assets/bcbcfdc3-4d63-49b0-8686-c97359f77538)

The generated files did make a dent on your drive though, for a single file you could get nearly 10x the size
```
    Directory: G:\Games\osu!\Songs\Untitled Etterna Pack\666 (Tim)

Mode                 LastWriteTime         Length Name                                                                 
----                 -------------         ------ ----                                                                 
-a----        17/11/2022     21:39          60487 (α - 1.00) - ([22.71] - 666).osu                                     
-a----        17/11/2022     21:39          60356 (α - 1.05) - ([23.59] - 666).osu                                     
-a----        17/11/2022     21:39          60233 (α - 1.10) - ([24.81] - 666).osu                                     
-a----        17/11/2022     21:39          60100 (α - 1.15) - ([25.72] - 666).osu                                     
-a----        17/11/2022     21:39          60015 (α - 1.20) - ([26.54] - 666).osu                                     
-a----        17/11/2022     21:39          60006 (α - 1.25) - ([27.25] - 666).osu                                     
-a----        17/11/2022     21:39          59995 (α - 1.30) - ([28.28] - 666).osu                                     
-a----        17/11/2022     21:39          59983 (α - 1.35) - ([29.39] - 666).osu                                     
-a----        17/11/2022     21:39          59971 (α - 1.40) - ([30.49] - 666).osu                                     
-a----        17/11/2022     21:39        1939468 1.00-Audio.mp4                                                       
-a----        17/11/2022     21:39        1845416 1.05-Audio.mp4                                                       
-a----        17/11/2022     21:39        1760540 1.10-Audio.mp4                                                       
-a----        17/11/2022     21:39        1683318 1.15-Audio.mp4                                                       
-a----        17/11/2022     21:39        1613341 1.20-Audio.mp4                                                       
-a----        17/11/2022     21:39        1549795 1.25-Audio.mp4                                                       
-a----        17/11/2022     21:39        1489949 1.30-Audio.mp4                                                       
-a----        17/11/2022     21:39        1435304 1.35-Audio.mp4                                                       
-a----        17/11/2022     21:39        1383759 1.40-Audio.mp4                                                                                                      
-a----        17/11/2022     21:39         121230 BG.jpg                                                               
```

<img width="337" height="178" alt="image" src="https://github.com/user-attachments/assets/9fd2d408-5dc3-44f2-b2db-f8cf32aa9070" />

Anyway, all of this now is just me reminicsing on an old hobby, I started playing in 2016 or 2017 ~ nearly a decade ago, a lot has changed since then...

[still never managed to get 10th dan lmao, forever 8th dan](https://youtu.be/nPNJUVjHlZo); and yes I know the etterna players have a panic attack when you mention dans, never stopped being funny.
