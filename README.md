# Seemita
## A new kind of women safety app, for both Android and iOS.

# Main Idea
Seemita will provide the user confidence by detecting a deviation from the user's designated route. Then, unless the user assured she's okay, a message would be sent automatically to chosen contacts. This message includes a custom text and the user's location.

# How does it work?

Because Seemita's goal is to inform that the user is in danger, without demanding her to take active actions, the app lets her submit every little detail in advance (the first two are mandatory, while the others have default values, even if not selecetd manually):

## Before going out

1.	Choose up to 3 **emergency contacts**, which will get a text message, containing her most recent location, and a text she chose herself.

 <p align="center">
 <img src="https://user-images.githubusercontent.com/71612739/108601795-24427580-73a7-11eb-84ee-c2b280ddd839.gif" />
</p>

2.	Select a **4-digit PIN code**, which in cases of a false positive (when the user deviated on purpose, or forgot the app was on), will give the user the option to **cancel the sending**.

 <p align="center">
 <img src="https://user-images.githubusercontent.com/71612739/108529951-b716dd80-72dd-11eb-9b89-fbbc8bf84288.gif" />
</p>

3.	Select the **time period between the detection of the deviation and the sending of the message**. This varies between 0 and 90 seconds, and every user can choose the right           amount, depending on the course she's about to take and her confidence in it.

<p align="center">
 <img src="https://user-images.githubusercontent.com/71612739/108531427-57213680-72df-11eb-9b14-3a064880e2d4.gif" />
</p>

4.	Write her **own text**, which will be the one her emergency contacts will get (of course, a link with the user's location is in the message, regardless of the text).

<p align="center">
 <img src="https://user-images.githubusercontent.com/71612739/108531762-bbdc9100-72df-11eb-8238-ef82fd376f79.gif" />
</p>

5.	**Choose her destination**, and getting the shortest route to it (from the user's current location), which will appear on the map, and deviations will be measured from. 
    There are 4 option for this feature, 2 for new destinations and 2 for ones the user chose before:

###  A. New Destinations:
  
   1. Using the **search box at the top of the screen**, the user can choose any address she wants to get to as her destination.

<p align="center">
 <img src="https://user-images.githubusercontent.com/71612739/108532857-fa268000-72e0-11eb-97f0-b7ed3f53a2f6.gif" />
</p>
    
   2. If there is no specific address, or if the user knows the location but not the exact address, she can tap on the **blue hand button** at the bottom of the screen, and             then **tap anywhere on the map** in order to get a route to this spot.

<p align="center">
 <img src="https://user-images.githubusercontent.com/71612739/108602405-6ae59f00-73aa-11eb-93e5-4a3ad0f74a06.gif" />
</p>

 ### B. Known Destinations:

  **Important to remember**: In order to make life easier for the user, destinations are saved, and not specific routes. This way, there is no need for many different cards for the same destination (work, gym, home, etc.), because once a card is selected, the route to it will be calculated from the user's current location.

   1. Using the **Routes History** option, which will contain all of the destination the user chose in the past (unless deleted). By choosing one of the cards in this list, the           shortest route from the user's location to this destination will appear as the designated route on the map.

<p align="center">
 <img src="https://user-images.githubusercontent.com/71612739/108602279-d7ac6980-73a9-11eb-82f1-6e3e283d33a7.gif" />
</p>

   2. Since the history might be loaded, the little heart icon lets the user the option to add chosen destinations to the **Favorites List**. Once in the favorites list, the flow is     similar to the one of the history.

<p align="center">
 <img src="https://user-images.githubusercontent.com/71612739/108537701-999a4180-72e6-11eb-80d0-191b51f6591c.gif" />
</p>

### Now, all the user has to do is press "Start" and go on her way.


## While walking the route

This is where the power of Seemita kicks in. The user will see her designated route to her destination, and with any devitation from it, Seemita will be triggered.

Of course, as mentioned, the user would have the option to cancel the sending, by pressing "I'm Okay" and submitting her PIN code before the timer goes off.

<p align="center">
 <img src="https://user-images.githubusercontent.com/71612739/108543244-7e7f0000-72ed-11eb-8080-7b828ac871bb.gif" />
</p>

If the user didn't actively cancel the sending, or if she pressed on the "Send SMS" button, in order to shorten the waiting time, everything the user subitted before she went out will be part of Seemita's sending process. All of the chosen contacts will get the chosen text message, and her current location.
Additionally, the SOS button will pop up on the screen, which a press on will lead to a call to the police. Of course, the call to the police is never done automatically.

<p align="center">
 <img src="https://user-images.githubusercontent.com/71612739/108543553-e6cde180-72ed-11eb-9cea-0341e2678549.gif" />
</p>

After pressing "End Route", or once the user got to her destination (the app will notify the user that her route is done), the user will get back to the Home Screen, and if the used destination was new, it is now added to the history.


# Technical Details

- Seemita's defintion of a deviation from a route is **30 meters from the marked side of the road on the map**.
- The app declares the route is done within **15 meters from the chosen destination**.


# Technologies

**Frontend:** React Native

**Backend:** Firebase

**Platform:** Expo

**APIs:** Twilio, Google Maps (Directions, Geocoding, Places), Turf.js

**SDKs:** Expo Contacts, Expo Google-Signin, Vibrate

**UI Framework:** Galio

**Cloud functions:** Google Cloud


### <a name="team-members"></a>Team Members
* Shai Liran <shailiran@gmail.com>
* Omri Lerer <golerer@gmail.com>
* Kfir Lev <kfirLev135@gmail.com>
* Chen Dahan <hendahan12@gmail.com>

