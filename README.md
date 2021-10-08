<!-- This is the markdown template for the final project of the Building AI course, 
created by Reaktor Innovations and University of Helsinki. 
Copy the template, paste it to your GitHub README and edit! -->

# Home Camera Assistant

Final project for the Building AI course

## Summary

Raspberry Pi powered system, which uses image recognition to identify and assist family members when coming home or leaving it. It recognises individuals, what they have with them, and gives clothing advice based on weather forecast data and persons schedule. Possible to integrate more actions, such as door unlocking if keys are missing.

## Background

Which problems does your idea solve? How common or frequent is this problem? What is your personal motivation? Why is this topic important or interesting?

Some motivations:
* hands are often literally and figuratively full when going out. This way there's not so much need to reach for phone to check the weather or bus schedules.
* If keys are left home, door can be still opened with own face. This would be also useful for children, since they tend to forget the keys quite often.
* Image recognition is quite fun application and this would be good way to get continous testing for it and figure out what other functions could be handy.


## How is it used?

Describe the process of using the solution. In what kind situations is the solution needed (environment, time, etc.)? Who are the users, what kinds of needs should be taken into account?

The system would basically be in use all the time, although some functions could be dropped by schedule.  
Always on:
* door opening by image

Scheduled  
* speech response preferably not at night

To be consireded:
* What about greeting when there's lots of traffic. Would it be enough to put some timeout for the next info about schedules and weather.
* How to distinguish if person is just going to look outside, instead of leaving? Integration to calendar?

Images will make your README look nice!
Once you upload an image to your repository, you can link link to it like this (replace the URL with file path, if you've uploaded an image to Github.)
![Cat](https://upload.wikimedia.org/wikipedia/commons/5/5e/Sleeping_cat_on_her_back.jpg)

If you need to resize images, you have to use an HTML tag, like this:
<img src="https://upload.wikimedia.org/wikipedia/commons/5/5e/Sleeping_cat_on_her_back.jpg" width="300">



## Data sources and AI methods

Basic image recognition from pretrained YOLO CNN. 
Facial recognition needs it's own training, which again needs images of family members and other persons of interest.

Weather data from various weather API's
Bus schedules and estimated arrival times from HSL's API

## Challenges

Biggest challenges are privacy and security. For privacy, camera shouldn't store images, unless permitted. Door opening should rather have false negatives than false positives for security reasons. How to prevent using picture of a person to get in?
* light environment
* mechanical components


## What next?

How could your project grow and become something even more? What kind of skills, what kind of assistance would you  need to move on? 


## Acknowledgments

* list here the sources of inspiration 
* do not use code, images, data etc. from others without permission
* when you have permission to use other people's materials, always mention the original creator and the open source / Creative Commons licence they've used
  <br>For example: [Sleeping Cat on Her Back by Umberto Salvagnin](https://commons.wikimedia.org/wiki/File:Sleeping_cat_on_her_back.jpg#filelinks) / [CC BY 2.0](https://creativecommons.org/licenses/by/2.0)
* etc
