![Header](./images/header.png)

# DXC Hackathon - Biometric Analysis and Response

## General Statement -

Autism is a lifelong neurological condition which affects one in every hundred people in the UK. As a spectrum condition, it affects each individual differently. High functioning individuals may be acutely intelligent and at the top of their professions, those with more complex challenges and additional difficulties (such as learning difficulties) may need much more support. A common thread is that nearly three quarters of those on the spectrum experience sensory differences. They may be under- or over-sensitive to light, sound, touch, taste etc and may have trouble with balance and spatial awareness. Communication is a further key issue. Some individuals will have difficulty understanding speech, some may not understand what their voice is for, others will be selectively mute. Problems communicating can mean that emotions – such as rising anxiety related to a sensory overload - are expressed physically, with sudden meltdowns which can include violence towards themselves or others or running away.  

If technology, in the form of non-intrusive biometric wristbands, could provide staff with a way to monitor each individual, giving awareness of rising agitation and anxiety before any marked behavior changes, each person could be better understood and supported. If the data gathered by the biometric device can then be cross-referenced with further data gathered by sensors positioned throughout the living environment – such as a residential care home – carers would be able to understand even more: such as, whether light (for example, sunlight, strip lights), noise levels or heat were a likely cause of the rising agitation shown on the biometric device.

At this point the volume, variety and veracity of the data to be processed and responded to for even a single human is not achievable.


## Problem Statement -

Autism Together (the client) is trying to better understand and support individuals with complex and challenging autism. The current method of observation only is not sufficient to understand rising anxiety and the potential for an onset of aggression in individuals. To improve this, the client has collected data from two main sources: a) from biometric devices worm by residents at a care home, b) from sensors gathering environmental data from the home itself. The client would like to be able to analyse the data and produce an algorithm which cross references each source and triggers a response from the support team. The outcome would enable each individual to experience a better quality of life.

## Overview of Consider Solutions

Some consideration has been given to a possible solution, although these are ideas, teams have the option to develop a solution using any method they see fit.

[Reference User stories](./Data%20Story%20-%20Improve%20Care.md)

## Hack-athon scope

The Hackathon event will focus on the

#### In-Scope
    - Data Storage in the Cloud
    - Turn the static Datasets into a simulated live feed
    - Data Processing - Ability to apply a simple query through code
    - Simple Event Trigger based on correlation of data events
    - Event Response through AI (Alexa)

#### Out of scope
    - Connecting to live data streams from devices
    - Multiple AI interfaces
    - Complex analytics Analysis
    - Security

#### Overview

Teams will aim to provide a solution that triggers an Alexa event by the analysis of a set of data held in a cloud ecosystem. The event will be based on the correlation of certain biometric and environmental triggers. (Heart Rate + Room Temperature)

Following a successful pattern match, an Alexa response should be triggered with a

  <b>"Hello World, I believe you need some help"</b>

## Preparation

Work Autism Together is doing and why.

- [Information on Behaviour](https://www.autism.org.uk/about/behaviour/meltdowns.aspx)
- [BBC News clip](https://www.bbc.co.uk/news/av/health-44680214/the-watch-that-could-help-manage-severe-autism?SThisFB=)

- Make sure you have a Github Account on [Github Link](https://github.com)  
  - Please note we are using two github Repo's
    - 1: General Information Repo [LINK](https://github.com/ckinson/Autism-Project) (For reference Only / Data Sources)
    - 2: Your Team repo (detail below) - This is secure, all code, Data and information for your team is stored here.
- You are familiar with AWS Services
- Understand the Data you are looking at, data set links are available at the bottom of this doc.


## Teams and Tools

#### Team Members

- Please see the Link below to see your team allocation

  [Team Members](https://github.com/ckinson/Autism-Project/blob/master/docs/teamstructure.md)

  *Action* - Please Fork, Edit and Send a Pull Request back to update the Team Members sheet with your Github ID.

#### Team Spaces
  - Code will reside on  Github under the following team spaces, teams will have access thought their Github userid's
  
## TEAM SPACES NOW MADE PUBLIC

- [Team 1 Space](https://github.com/ckinson/DTC-Hackathon-Team1)
- [Team 2 Space](https://github.com/ckinson/DTC-Hackathon-Team2)
- [Team 3 Space](https://github.com/ckinson/DTC-Hackathon-Team3)
- [Team 4 Space](https://github.com/ckinson/DTC-Hackathon-Team4)
- [Team 5 Space](https://github.com/ckinson/DTC-Hackathon-Team5)
- [Team 6 Space](https://github.com/ckinson/DTC-Hackathon-Team6)
- [Team 7 Space](https://github.com/ckinson/DTC-Hackathon-Team7)
- [Team 8 Space](https://github.com/ckinson/DTC-Hackathon-Team8)

*Note*  - you will see the each repo has three folders

- <b>Code</b> - this is to store any code you create, including configuration files
- <b>Docs</b> - this is to store you documents you create, ensure you document you solution and learnings
- <b>Media</b> - If you take photos, or video recordings please store here (funny moments are welcome)


#### AWS Service Info

Any AWS service can be used -

  [AWS Service Catalogue Link](https://console.aws.amazon.com/console/home?region=us-east-1)

  ![AWS Service Cat](./images/awscat.png)

#### Alexa Skills Info

- Alexa will be the AI interface

    Alexa AI provides the ability to develop your own AI Skills, more information on this can be found here [LINK](https://developer.amazon.com/alexa-skills-kit)

## Data

These data sets are made up, based on nominal levels from various data sources.

Based on a 24hr monitoring session from a Biometrics Sensor, and two Environment covering Light and Temperature.

### Three Data sets are provided

- 1: Biometric from Off the self Personal Device (Fitbit or Other)
    - [Biometric Data](https://github.com/ckinson/Autism-Project/blob/master/Data/Biometrics-Data_Set-24Hrs.csv)

- 2: Light Levels
    - [Light Level Data](https://github.com/ckinson/Autism-Project/blob/master/Data/LightLUX-Data_Set-24Hrs.csv)

- 3: Location Temperature
    - [Location Data](https://github.com/ckinson/Autism-Project/blob/master/Data/RoomTemp-Data_Set-24Hrs.csv)

### Raw Data - (optional) some data manipulation may be required.

 Below is data sent in by Autism Together, collected from the actual devices over a 24hr period.

 I’ve attached some CSV files for the Hackathon. You have some sample data from the environmental system on one spreadsheet and then separate sheets with the E4 (Bio-metric) data, the data we are keen on is the EDA, ACC and heart rate. Please note the accelerometer (ACC) data should be in 3 planes, x,y and z.

 [Raw Data Info](https://github.com/ckinson/Autism-Project/blob/master/Data/Real_Data/info.md)

 [Raw Data Sets Folder](https://github.com/ckinson/Autism-Project/tree/master/Data/Real_Data)


## Additional Credit

If the teams find that they complete the task, they is options to improve, considerations include

- Create addition a Alexa response, targeting different personas
    - Consider
        - Patient - "Hi Carl, you need to move location"
        - Carers - "Carl is in trouble you need to contact him, it's his Body Temp "
        - Family - " Carl is fine, but could do with you calling him"
- Consider increase the Data set
    - Noise, Light (this will require creating a simple data set)
    - Noise (db) level measured during the time period
    - Light (Lux) Level measured during the time period
