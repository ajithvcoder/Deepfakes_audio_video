# Deep Fake Audio VIdeo

**Contents:**

There are three process 

- [Video Generation](#Video-Generation)
- [Audio Generation](#Audio-Generation)
- [Combine Audio and video](#Combine-Audio-and-video)

Will covert all manual process to code soon



## Video Generation 


1. have a png file (target person)

2. have a video file (specimen person)

Execute the colab file for video


**How to generate good deep fake video**

    "Will update it soon"



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

2. Open this site https://online-audio-converter.com/ and Upload the mp3 file and give a DVD resolution and click convert . Now hover over the "Download" button and copy the link . go to google colab and use 
    below command to copy it to google colab
    
```!wget <link>```

3.Rename the file name to audio.wav

```!mv <filename.wav> audio.wav ```



**Sample audios that i used**

(In the entire audio only the targeted person will be speaking )

- Steve jobs - https://www.youtube.com/watch?v=65_PmYipnpk
- Rohan Shravan - https://www.youtube.com/watch?v=PstVDlK2lGA
- Ritika sighn - https://www.youtube.com/watch?v=QQI7foZMPtE


## Combine Audio and video

 Use this website - https://www.kapwing.com/tools/add-music-to-video


### Will upgrade the code and process in manner and quality of audio and video asap


**Credits :**

Video - https://towardsdatascience.com/how-to-produce-a-deepfake-video-in-5-minutes-513984fd24b6 

Audio - https://github.com/CorentinJ/Real-Time-Voice-Cloning.git

