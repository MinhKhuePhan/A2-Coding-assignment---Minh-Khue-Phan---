# Assignment 2: Code Prototype Project 
# Recreating Vietnam's National Anthem in TunePad
> This project uses musical coding to recreate Vietnam's national anthem, Tiến Quân Ca, on TunePad. Designed to help Vietnamese students in Australia reconnect with their homeland, this project combines technical precision and cultural pride.


## Table of Contents
* [Background and Purpose](#background-and-purpose)
* [Features and Functions](#features-and-functions)
* [Usage Instructions](#usage-instructions)
* [Code Explanation and Comments](#code-explaination-and-comments)
* [Challenges and Solutions](#challenges-and-solutions)
* [Future Improvements](#future-improvements)
* [References](#references)
* [Contact](#contact)



## Background and Purpose
Raising the flag and singing the national anthem is a meaningful ritual and a cherished cultural tradition observed in Vietnam's institutions, organizations, schools, and armed forces. It embodies a profound love for the homeland, a deep sense of pride, and national dignity. This practice serves as a reminder for all to remain committed to personal growth, to strive to fulfill their duties, and to uphold traditional cultural values and professionalism in the workplace.

However, as international students, we cannot maintain this routine while studying abroad, which inspired me to create this project. By coding the Vietnamese national anthem, I hope to bring a piece of this tradition to life digitally, allowing us to reconnect with our culture and remember the values it instills, even when we are far from home.


## Features and Functions
In this project, I used several key functions in TunePad to bring each part of the Vietnamese national anthem to life. Here’s how each function contributes to the composition:

PlayNote: This function is used to play individual notes, forming the core melody of the anthem. By specifying different notes, I was able to recreate the anthem’s main theme on the piano, ensuring it resonates with the familiar tune that Vietnamese students remember.

Rest: The Rest function introduces pauses between notes, allowing for natural breaks in the melody. This is essential to accurately reflect the rhythm of the anthem, adding emphasis where needed and making the piece feel more authentic.

Beats: The beats parameter determines the duration of each note, allowing me to control how long each note is held. This parameter is crucial for aligning with the tempo and rhythm of the anthem, ensuring the melody flows smoothly from one note to the next.

Chord: Some parts of the anthem require multiple notes to be played simultaneously. The Chord function allows for this by enabling me to define chords (collections of notes) and play them together, adding depth to the piece and enriching the overall harmony.

Velocity: The velocity parameter controls the intensity or volume of each note, allowing me to add emotional emphasis at certain points. For example, I increased the velocity at the end of each verse to capture the anthem's powerful and patriotic tone, making the music feel more impactful.

Combining these functions, I structured the anthem with a melody line on the piano and accompaniment parts played by additional instruments (bass and guitar) to create a fuller sound. This setup in TunePad allowed me to balance technical accuracy with cultural authenticity, resulting in a familiar and emotionally resonant rendition.


## Usage Instructions
To experience the recreated Vietnamese national anthem in TunePad, you can view the project using the link below:

[View Project on TunePad](https://tunepad.com/project/90374)


This link provides a read-only view, allowing you to listen to the anthem and explore the code without the ability to make changes. Simply follow these steps:

Open the Link: Click on the [project link](https://tunepad.com/project/90374) to open the TunePad project page.

Explore the Code: On the project page, you can view the code I used to recreate the anthem, including the functions PlayNote, Rest, Beats, Chord, and Velocity.


Play the Music: Use the play button in TunePad to listen to the coded rendition of the anthem. This will show you how the melody and accompaniment come together. 

First, on the top right, you will see 2 buttons, triangle and square. 

<img width="514" alt="Ảnh chụp Màn hình 2024-11-05 lúc 3 25 07 CH" src="https://github.com/user-attachments/assets/cb08e09a-805b-46bd-bd83-fc006ea7295b">

Step 1: Press the square button to restart every cell. 

Step 2: To start playing the music, press the triangle button. 


## Code Explanation and Comments
This is the music sheet 

<img width="811" alt="Ảnh chụp Màn hình 2024-11-04 lúc 12 22 56 CH" src="https://github.com/user-attachments/assets/1e1c9822-96df-4475-9d1f-d20b38702107">


You will see the music sheet set, with the BPM being 120 and 4/4. That is why, on top of the TunePad, you will see the reason why I set the BPM and time like this: 

<img width="382" alt="Ảnh chụp Màn hình 2024-11-05 lúc 3 35 25 CH" src="https://github.com/user-attachments/assets/4f758c55-97fd-44ea-b672-e73d7571cbc4">

On the right-hand side, in the cell sections, I have 1 cell for melody playing on the piano and 3 other cells for accompaniment playing on the piano, bass, and guitar. 

<img width="226" alt="Ảnh chụp Màn hình 2024-11-05 lúc 3 39 59 CH" src="https://github.com/user-attachments/assets/f84eb9df-c055-4314-bbfd-2757493bc8ce">

 4 most prominent codes that you will see in my TunePad are:

- playNote(0, beats=0): Plays a musical note based on its MIDI number (0-127), where each number corresponds to a specific pitch. With a Tempo di Marcia set at 120 BPM, each beat lasts 0.5 seconds. So, if you write beats = 1, the note will last for 0.5 seconds. 

- playNote(0, beats = 0, velocity = 0): I only use velocity for some notes at the end of each verse to set how hard/loud the note sounds. 

- rest(beats = 0): Add a pause between notes. The length of the pause can be set using the optional beats parameter.

- chord = [36,48,60,64,67]: Some notes must be played simultaneously. I used the chord function to combine notes, allowing multiple pitches to sound simultaneously, such as MIDI numbers 36,48,60,64, and 67.

<img width="173" alt="Ảnh chụp Màn hình 2024-11-05 lúc 4 30 26 CH" src="https://github.com/user-attachments/assets/6c087e2b-4dd6-4c96-a747-02b4231fb0b7">

## Challenges and Solutions
I encountered several challenges while coding this song.

Setting the Beats: One of the main issues was determining the duration for each note, as the music sheet didn’t specify this. To solve this, I watched performances of the anthem on piano [like this one on YouTube](https://www.youtube.com/watch?v=JBDmWrH3OGI) and gradually figured out the appropriate beats for each note.

Playing Multiple Notes Simultaneously: Initially, I was unsure how to play multiple notes at the same time. To address this, I researched examples on TunePad and learned how to use the chord function to play notes together, allowing me to add depth and harmony to the piece.


## Future Improvements
How does one go about using it?
Provide various use cases and code examples here.

`write-your-code-here`


## References
Project is: _in progress_ / _complete_ / _no longer being worked on_. If you are no longer working on it, provide reasons why.


## Contact
Created by [@flynerdpl](https://www.flynerd.pl/) - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->

