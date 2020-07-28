# Deep Fake Audio VIdeo with colab

**Contents:**

There are three process 

- [Video Generation](#Video-Generation) - A single image is enough
- [Audio Generation](#Audio-Generation) - A single audio is enough you can make any words with it 
- [Combine Audio and video](#Combine-Audio-and-video)

Will covert all manual process to code soon

Entire process of audio and video generation is in colab so no need to install any thing in local . if you are in linux machine you can use "ffmeg command" to do all preprocessing and post processing below.


## Video Generation 


1. have a png file (target person)

2. have a video file (specimen person)

Execute the colab file for video

3. Use increasefps.py file to increase FPS and make your video better

**How to generate good deep fake video**

Use a 256x256 file and choose one png file in which it is till neck example see this drive (https://drive.google.com/drive/folders/1kZ1gCnpfU0BnpdU47pLM_TQ6RypDDqgw)


<img align="left" width="100" height="100" src="09.png">
<img width="100" height="100" src="got-05.png">
<img  width="100" height="100" src="02.png">









## Audio Generation 

Note it works for both male and female

**Instructions in colab for good audio**

please add within 12 words .. and if u want to generate more paragraph save the generated audio in another name and then generate another audio

Dont use any punctuations it will produce some noise . Use only one space between words


Have the any audio(.wav) file of the person who is the target and read the instruction below and then go to colab 



if u dont have (.wav) follow below steps to generate quickly 

**Convert video to audio**

1. find a youtube video where the target person is speaking(only the person should speak no background audio or else no other persons voice) and convert to mp3 use this site for converting https://ytmp3.cc/en13/  and download the video 

**Convert mp3 to wav**

In linux - Using ffmpeg 

```
ffmpeg -i input.mp3 output.wav 
```

or else follow 2 and 3 points

2. Open this site https://online-audio-converter.com/ and Upload the mp3 file and give a DVD resolution and click convert . Now hover over the "Download" button and copy the link . go to google colab and use 
    below command to copy it to google colab
    
```!wget <link>```

3.Rename the file name to audio.wav

```!mv <filename.wav> audio.wav ```


**Audio merger :**
https://clideo.com/merge-wav


**Sample audios that i used**

(In the entire audio only the targeted person will be speaking )

- Steve jobs - https://www.youtube.com/watch?v=65_PmYipnpk
- Rohan Shravan - https://www.youtube.com/watch?v=PstVDlK2lGA
- Ritika sighn - https://www.youtube.com/watch?v=QQI7foZMPtE



## Combine Audio and video

if you are in linux you can use below command 

```ffmpeg -i "mres/g_wonder.mp4.mp4" -i "properaudio/c_wonderwoman.wav" -shortest g_wonder.mp4```

or else you can use below website which generates without water mark
 
 
 Use this website - https://www.kapwing.com/tools/add-music-to-video
 


### Will upgrade the code and process in manner and quality of audio and video asap


**Credits :**

Video - https://towardsdatascience.com/how-to-produce-a-deepfake-video-in-5-minutes-513984fd24b6 

Video - https://www.youtube.com/watch?v=peOKeRBU_uQ

Audio - https://github.com/CorentinJ/Real-Time-Voice-Cloning.git

