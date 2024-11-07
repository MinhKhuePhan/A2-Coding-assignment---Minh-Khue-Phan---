# Assignment 2: Code Prototype Project 
# Recreating Vietnam's National Anthem in TunePad
> This project uses musical coding to recreate Vietnam's national anthem, Tiến Quân Ca, on TunePad. Designed to help Vietnamese students in Australia reconnect with their homeland, this project combines technical precision and cultural pride.


## Table of Contents

- [Background and Purpose](#background-and-purpose)
- [Features and Functions](#features-and-functions)
- [Usage Instructions](#usage-instructions)
- [Code Explanation and Comments](#code-explanation-and-comments)
- [Challenges and Solutions](#challenges-and-solutions)
- [Future Improvements](#future-improvements)
- [References](#references)
- [Contact](#contact)



## Background and Purpose
Raising the flag and singing the national anthem is a meaningful ritual and a cherished cultural tradition observed in Vietnam's institutions, organizations, schools, and armed forces. It embodies a profound love for the homeland, a deep sense of pride, and national dignity. This practice serves as a reminder for all to remain committed to personal growth, to strive to fulfill their duties, and to uphold traditional cultural values and professionalism in the workplace.

However, as international students, we cannot maintain this routine while studying abroad, which inspired me to create this project. By coding the Vietnamese national anthem, I hope to bring a piece of this tradition to life digitally, allowing us to reconnect with our culture and remember the values it instills, even when we are far from home.


## Features and Functions
In this project, I used several key functions in TunePad to bring each part of the Vietnamese national anthem to life. Here’s how each function contributes to the composition:


**PlayNote**: This function plays individual notes based on their MIDI number.
- Example of using playNote
playNote(60, beats=1) 

Here, playNote(60, beats=1) plays the note with MIDI number 60 (Middle C) for 1 beat.


**Rest**: The Rest function introduces pauses between notes.
- Example of a Rest
Rest(beats=0.5) 

This half-beat rest creates a break in the melody, giving it rhythm and emphasis.


**Beats**: This parameter specifies how long a note or rest should last.
- Example of beats in playNote
playNote(62, beats=2) 

Setting beats=2 makes the note last longer, aligning with the anthem’s tempo and flow.


**Chord**: This function allows multiple notes to play simultaneously.
- Example of a chord
chord = [60, 64, 67]  # Define a C major chord (C, E, G)
playNote(chord, beats=1.5)

In this example, playNote(chord, beats=1.5) plays a C major chord, adding harmonic depth.


**Velocity**: This parameter adjusts the volume or intensity of a note.
- Example with velocity
playNote(60, beats=1, velocity=100)  # Plays Middle C loudly

Setting velocity=100 makes the note louder, emphasizing strong parts of the anthem.


Combining these functions, I structured the anthem with a melody line on the piano and accompaniment parts played by additional instruments (bass and guitar) to create a fuller sound. This setup in TunePad allowed me to balance technical accuracy with cultural authenticity, resulting in a familiar and emotionally resonant rendition.


## Usage Instructions
To experience the recreated Vietnamese national anthem in TunePad, you can view the project using the link below:

[View Project on TunePad](https://tunepad.com/project/90374)


This link provides a read-only view, allowing you to listen to the anthem and explore the code without the ability to make changes. Simply follow these steps:

Open the Link: Click on the [project link](https://tunepad.com/project/90374) to open the TunePad project page.

Explore the Code: On the project page, you can view the code I used to recreate the anthem, including the functions PlayNote, Rest, Beats, Chord, and Velocity.

The project is organized into different cells:

- Melody on Piano: The main melody line of the anthem.
  
- Piano Accompaniment: Chord progressions to support the melody.
  
- Bass Accompaniment: Adds depth with bass notes.
  
- Guitar Accompaniment: Complements the melody with additional harmony.


Play the Music: Use the play button in TunePad to listen to the coded rendition of the anthem. This will show you how the melody and accompaniment come together. 

First, on the top right, you will see 2 buttons, triangle and square. 

<img width="514" alt="Ảnh chụp Màn hình 2024-11-05 lúc 3 25 07 CH" src="https://github.com/user-attachments/assets/cb08e09a-805b-46bd-bd83-fc006ea7295b">

Step 1: Press the square button to restart every cell. 

Step 2: To start playing the music, press the triangle button. 

### How to Upload a JSON File to TunePad
- Access the JSON File: Locate the JSON file on top of the README file.  

- Download the Raw File: Click to download the raw file. It may download with the name "JSON file.txt".

- Rename the File: Change the file extension from "JSON file.txt" to "JSON file.JSON". Confirm and save the changes.

- Upload to TunePad:Open TunePad. Go to Project > Import. Select the renamed file "JSON file.JSON" and upload it.

You should now have the project imported into TunePad and ready for use.


## Code Explanation and Comments
This is the music sheet 

<img width="811" alt="Ảnh chụp Màn hình 2024-11-04 lúc 12 22 56 CH" src="https://github.com/user-attachments/assets/1e1c9822-96df-4475-9d1f-d20b38702107">


You will see the music sheet set, with the BPM being 120 and 4/4. That is why, on top of the TunePad, you will see the reason why I set the BPM and time like this: 

<img width="382" alt="Ảnh chụp Màn hình 2024-11-05 lúc 3 35 25 CH" src="https://github.com/user-attachments/assets/4f758c55-97fd-44ea-b672-e73d7571cbc4">

On the right-hand side, in the cell sections, I have 1 cell for melody playing on the piano and 3 other cells for accompaniment playing on the piano, bass, and guitar. 

<img width="226" alt="Ảnh chụp Màn hình 2024-11-05 lúc 3 39 59 CH" src="https://github.com/user-attachments/assets/f84eb9df-c055-4314-bbfd-2757493bc8ce">

 The four prominent codes that you will see in my TunePad are:

- playNote(0, beats=0): Plays a musical note based on its MIDI number (0-127), where each number corresponds to a specific pitch. With a Tempo di Marcia set at 120 BPM, each beat lasts 0.5 seconds. So, if you write beats = 1, the note will last for 0.5 seconds. 

- playNote(0, beats = 0, velocity = 0): I only use velocity for some notes at the end of each verse to set how hard/loud the note sounds. 

- rest(beats = 0): Add a pause between notes. The length of the pause can be set using the optional beats parameter.

- chord = [36,48,60,64,67]: Some notes must be played simultaneously. I used the chord function to combine notes, allowing multiple pitches to sound simultaneously, such as MIDI numbers 36,48,60,64, and 67.

<img width="173" alt="Ảnh chụp Màn hình 2024-11-05 lúc 4 30 26 CH" src="https://github.com/user-attachments/assets/6c087e2b-4dd6-4c96-a747-02b4231fb0b7">

## Challenges and Solutions
I encountered several challenges while coding this song.

- Setting the Beats: One of the main issues was determining the duration for each note, as the music sheet didn’t specify this. To solve this, I watched performances of the anthem on piano [like this one on YouTube](https://www.youtube.com/watch?v=JBDmWrH3OGI) and gradually figured out the appropriate beats for each note.

- Playing Multiple Notes Simultaneously: Initially, I was unsure how to play multiple notes at the same time. To address this, I researched examples on TunePad and learned how to use the chord function to play notes together, allowing me to add depth and harmony to the piece.


## Future Improvements
In the future, I would like to expand the project by including additional verses of the anthem, as I currently focus only on the main verse commonly sung by students. Given more time, I plan to code the other verse to render the anthem completely.

Additionally, I feel something may be missing in the current version, perhaps due to the coding limitations or playback speed in TunePad. I’ve noticed that this version feels a bit slower than expected. To address this, I’ll experiment with tempo adjustments and playback features to capture the anthem’s full energy and pace.

Moreover, I aim to make the coding more dynamic and expressive by incorporating more advanced functions beyond the basic four I used initially. By adding varied techniques and code functions, I hope to make the project more vibrant and musically rich, capturing the full spirit of the anthem.


## References

Grigsby, C. (2023). Python for students [LinkedIn Learning course]. LinkedIn. https://www.linkedin.com/learning/python-for-students-2023

LANDR. (2020, February 8). Music scales explained in 6 minutes [Video]. YouTube. https://www.youtube.com/watch?v=PG_u4NDJtwU

National Assembly of Vietnam. (n.d.). Tiến quân ca [PDF file]. Retrieved from https://quochoi.vn/content/tintuc/Lists/News/Attachments/30645/1.Ti%E1%BA%BFn%20qu%C3%A2n%20ca.pdf

TunePad. (n.d.). TunePad documentation. TunePad. https://learn.tunepad.com/docs/

TunePad. (2024). TunePad piano. Learn TunePad. https://learn.tunepad.com/interactives/piano/

Vietnamese Musician. (2017). Quốc ca Việt Nam - Tiến quân ca (Vietnamese National Anthem - Marching Song) [Video]. YouTube. https://www.youtube.com/watch?v=JBDmWrH3OGI




## Contact
Created by Minh Khue Phan. 
Email: Minh.K.Phan@student.uts.edu.au


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->

