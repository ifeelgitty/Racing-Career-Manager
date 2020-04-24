# Racing-Career-Manager (v0.2)

**Warning: v0.2 not compatible with previous files or savegames**

As someone who has been playing racing simulators for nearly a decade now, something has always been missing: (A girlfriend?) A long-term motivation like it was found in the early Gran Turismo games, the feeling of **buying and owning cars, racing for a reason, climbing through the stages of motorsport, earning licenses etc.** While most modern racing simulator-creators will spend loads of money and months on getting the air pressure simulation of the tyres right, none of them really seemed to care about this part of the experience. This ends now(a bit)! Because I'm working on a free and simple(and ugly) software which simulates this career, **embedding any simulator to buy cars, race championships and ultimately work yourself through the ranks of racing**. 

## Current State of the Software

This is a very early beta. You can already see how it works, most thingy actually do work, but there are bugs and missing functions everywhere(from starting a second season to, well, viewing your garage!). Also, in the process of adding new features I will overhaul old ones, so expect lots of changes and don't expect "savegames" to work. The App is certainly not self-explanatory, so I will at some point add appropriate tutorials/info screens in-app. This is also true for modding: I will create a manual that fully explains how to deal with the CSV-files, but that will be done when Im far enough to feel comfortable that the way I structure the CSV-files doesn't change much anymore(should be quite soon).

**The vehicle list and race series included is not up to date and far from complete. It is mostly for demonstration and development purposes. Mod them as much as you like!**

In the long term, lots of functionality will be added, from Sponsorships to random events and whatever else I can come up with. I will probably release a proper list of that at some point soon. Don't expect major upgrades to the User Interface soon, it will probably stay quite simple, as I find it a lot more fun to implement functionality codewise than having to deal with UI-stuff, which I find annoying.

**I'm happy to get feedback in any way, suggestions for features, improvements, problems you ran into, bugs etc.**

## How to Download and Start

- I doubt this software will work on anything that isn't a Windows computer, but feel free to try.

- Click "Clone or Download" and then "Download Zip" (if you don't know GitHub, else you will know alternatives)
- Extract content of downloaded Zip in a Folder
- Make sure you have the Java Runtime Environment installed.
- Open the App by clicking "RCM.jar", if that does not work, open the "RCM.bat".

# Beginning of App-Documentation

## A Disclaimer

This software has been created to help you keep track of your career, allowing for any simulator and any combination of different simulators to be used in context of a racing career. What it does not do though is: Read out results from your game or save championship standings with points etc. **You actually have to keep track of the championship standings inside the game(AMS, AC, RRR) or with additional software(rf2) and then type in the position you scored in as well as the damage your car had into the software, so it can calculate all the relevant measures.** As this is a one-person project and the world of racing simulators moves fast, too many resources would have to go into developing plugins, which probably are out of date easily anyway.

I feel the need to add that the money in game is virtual, you will neither pay nor receive actual money in any way.

## What it offers

Racing yourself through the career ladder, signing up for different racing series, going through cycles of seasons. And the best thing: Everything is **moddable**. The car list as well as the different racing series are saved as **csv files, so as tables, which means that you can add your favorite cars and racing series and combine different games**. You're not set to just one simulator. So, if you prefer the F1 cars in Assetto Corsa over the ones in Automobilista, just use them! 

## Buying Cars

*The Car store, where you have a list with all vehicles to buy*

<img src="https://raw.githubusercontent.com/ifeelgitty/Racing-Career-Manager/master/tut-img/CarStore.PNG"  title="Carstore" width=600>

Buying cars is quite straightforward: **If you have the money, you can buy them**. All relevant attributes are shown, including their type, class and prize. Whether you can sign up for racing series that use this car, however, depends on the requirements for that series, which might be linked to you holding the required license. **In a future iteration, the store will also show which games include these vehicles, so you have an impression of which car makes most sense for you**.

There also is a **garage** in which you can see the cars you own and **sell them at heavy discounts**, if you need to!

Additionally, there will be a **used car store**. This holds cars that are not available in the normal shop, probably rather old cars. A couple of times per year, the list of cars will be refreshed, with **each car having an individual likeliness of popping up**. Therefore, you might want to hold your money together, in case that very rare car you always wanted is finally available for purchase. Not only this however, but the **prize for the vehicle will vary**, so maybe, maybe, the offer you're seeing there is completely overpriced and it might make sense to wait another year... maybe...

## Racing Seasons

*CSV-File with all (possible) tracks assigned to the Formula 1 series. Per Season, the tracks are drawn from this list*

<img src="https://raw.githubusercontent.com/ifeelgitty/Racing-Career-Manager/master/tut-img/F1Races.PNG"  title="CSV List of all available F1 Races" width=412>

*Example for one Formula 1 season in-App, based on the available tracks above*

<img src="https://github.com/ifeelgitty/Racing-Career-Manager/blob/master/tut-img/F1ActualRaces.PNG?raw=true"  title="Example of F1 Season" width=412>

*The Season Sign Up-Tab allows you to sign up for, well, seasons of different racing series. That is, if you have a suitable car, license and money*

<img src="https://github.com/ifeelgitty/Racing-Career-Manager/blob/master/tut-img/SeasonSignUp.PNG?raw=true"  title="Season Signup window" width=550>

One thing I’ve been annoyed with in many Racing Games is the static season setup. Where is the re-play value when every season is set up in the exact same way with the same tracks? Therefore, **every season in this software will look differently, with a newly generated calendar every season!** Every series has a list of tracks with some being “mandatory” and some optional. For example, a Formula 1 season will always have Barcelona at some point during the season, while Nurburgring is an optional race, which might or might not be included in a season. This can even go further, with a race like Melbourne being set to “Spot 1”, always being the first race of the season. Thereby, you will have some stability and some variety in-between seasons, keeping it fresh but also not totally random.

Now, while for most races you will have to be signed up for the series to be able to sign up for the race, there are exceptions. We’ve all seen how race drivers try their hands on the Le Mans 24h or the Indy 500. Therefore, **some races you can attend without signing up for the whole season**. However, while you will get prize money for the race, you won’t get any season prize money for your final championship position(because you are not signed up for the championship).

Some racing series are just **support categories for bigger championships**. Formula 2 and 3 race at a selected group of F1 races, or the Australian Formula 4 supports the larger (V8) Supercars category. Therefore, calendars can be “inherited”. Randomly, the support championships take part at some of the races of the main championship.

## Setting Up a Season

*First screen of setting up a new season: Choose the games you want to include and the sorting mechanism, in case some series are included for multiple games.*

<img src="https://raw.githubusercontent.com/ifeelgitty/Racing-Career-Manager/master/tut-img/SeasonSetUp1.PNG"  title="The Stages!" width=712>

*On the second screen you can then change the automatic selection, in case you want to. Here for example you can see that three series are both implemented in AMS and AC, so you can pick and choose!*

<img src="https://github.com/ifeelgitty/Racing-Career-Manager/blob/master/tut-img/SeasonSetUp2.PNG"  title="The Stages!" width=712>

Before every season you can set up the games you want to include. In case one series like formula 1 is implemented in multiple games, you can pick which one to include for the season. For the examples above, the ordering is AMS -> RF2 -> AC, which means that the automatic selection prefers the AMS-implementations. However, you can change this in the second screen for each of the series if you like!

## Managing your Finances 

This also brings us to another aspect: Finances! You will have **costs and a revenue stream** that needs to be balanced to not break the bank. You will purchase cars, sign up for testing, sign up for racing series and sign up for races. You will also have to **pay for damages** to your car in any of those sessions. Income is provided by **prize money** that you can win both by finishing well in races and the overall championship. By finishing rather high in the standings, you will gain enough profit to finance taking part in a higher-staged championship in the following season. But even if you’re in the lower part of the field, you are still well-capable to support another season in the same category. This corrects something I have never been fond of in some racing games: **It is not at all expected of you to always win championships to advance in your career, it should rather be the exception**. Also: As long as you’re somehow competitive, even if just occasionally getting into the top 10, this is typically enough to stay in the same category.

## Making it through the Stages of Racing

*Table of all stages, their typical total season cost, the number of races you will on average expect on this stage, the typical license required to attend a series like this and examples of suitable championships to run on this stage.*

<img src="https://github.com/ifeelgitty/Racing-Career-Manager/blob/Readme/tut-img/StageTable.png?raw=true"  title="The Stages!" width=712>

When setting up your profile, you can choose whatever amount of credits you want to start with, also dictating which stage you are able to start on. Generally, you work your way up, trying to make enough money to finance seasons in higher stages, while winning the required license to be able to attend. Licenses are obtained by scoring a certain position in a championship, while the stage technically does not represent anything else than the total amount of money you will spend per year on the season, races and the vehicle.

Race Length | Race Multiplier | 
--- | --- 
Short | 1
Medium | 1
Long | 1
Endurance | 2
12 Hours | 3
24 Hours | 4

While the number of races per stage is just an indicator, there is a second factor to keep in mind: The Race Length. **It wouldn't be fair to get the same prize money for winning a sprint race than for winning the 24 hours of Le Mans.** Therefore, from a predefined list of race lengths seen above, **some count as "multiple" races**. This means that a **racing series like the WEC has effectively less races per season than Formula one, as the average race is simply longer. It also has an effect in that it multiplies the cost for signing up and the race prize money by the same factor.**

It is up to you to interpret the "real" lengths you want to race lengths to equate to. I, for example, generally halve the lengths of all races, regardless of whether its short or long, compared to their real counterparts. 


## The Calendar

*Example Screenshot of the Calendar. Obviously, February is not the most active month yet, so expect more races later in the year.*

<img src="https://github.com/ifeelgitty/Racing-Career-Manager/blob/Readme/tut-img/Calendar.PNG?raw=true"  title="Example of F1 Season" width=712>

Like Julius Caesar, I feel entitled to slightly modify the workings of our calendar. **Every month is simply split into 4 weeks**, without specific days or anything. This is totally not done because I’m too lazy to properly implement a calendar (Yes, it is), but because it simplifies the process (same thing). It has another positive effect: As this calendar has 48 instead of 52 weeks, it densens the calendar a bit, compensating for the lower number of races per championship compared to real life.

Besides structuring the year, the calendar has one main effect: **You are only able to sign up for races at one location per week.** Therefore, you can for example sign up for all races at Adelaide at the same weekend(if youre eligible to participate in the respective series, of course), but not attend both a race in Adelaide and Gioania. So, **if two events at different locations overlap, choose which race is more important to you (or you might lose your championship title) and choose wisely**. Also feel free to check whether there are overlaps between multiple championships before signing up for them, so you know in advance what to expect. Of course, each series has a different start and end point of the season, based on the span in real life, so Australian Supercar races start already in February, while Formula one does not start before March.

## Damage!

*Window of a test day, showing the damage-intake. Here you insert the number of damaged and destroyed parts over the whole session, for which you will have to pay!*

<img src="https://github.com/ifeelgitty/Racing-Career-Manager/blob/Readme/tut-img/TestDay.PNG?raw=true"  title="Test Day incl. Damages" width=712>

When this software was started, the "new generation" of Racing Sims wasnt really there yet. For both Automobilista and rFactor 2, the damage is well-shown in two steps, which I call **"damaged" and "destroyed"**. Based on this, the damage system was created. You will have to straightforwardly put in the damage obtained in your session here. In the case of Assetto Corsa, it works by interpreting any damage to a part as "damaged", and full, red damage as "destroyed". For other racing sims, I will try to create other ways to input the damage at a later point in time. 

If you're wondering why damage input is even relevant: In simming, crashing your car obviously does not have any consequences, so drivers are less attentive and less careful than they would be on a real track. '**By adding paying for your damages, an incentive is added to drive more responsibly, as a real driver would.** Crashing once in a while will not break your bank, but crashing 10 times per session will! 

## The Racing Weekend

### Testing Sessions

Per week, you can **sign up for one testing session**, independent of your racing weekend plans. This can be one, two or three hours long. Depending on the length and the vehicle you use, the session will cost you some credits. Quite straightforward.

### The actual Racing Weekend

*Raceweekend Window, to decide which sessions to attend. Example taken from the first Formula Ford Australia round at Adelaide.*

<img src="https://github.com/ifeelgitty/Racing-Career-Manager/blob/Readme/tut-img/Raceweekend.PNG?raw=true"  title="Raceweekend" width=712>

As already mentioned, you're able to sign up for any amount of races at exactly one track per racing weekend. When you've signed up and the weekend finally starts, you have to **choose which sessions to include, Practice 1, 2, Qualifying and Warmup**. The race itself will obviously always be part of it. Here, we have selected Practice 1 and Qualifying.

### Practice and Qualifying Sessions

*Example from the Qualifying Window. However, the practice and warmup windows are identical. Please ignore the error regarding the race number, will be fixed ;)*

<img src="https://github.com/ifeelgitty/Racing-Career-Manager/blob/Readme/tut-img/Qualifying.PNG?raw=true"  title="Qualifying" width=712>

For each session, you will see the above window. At the end of the actual session, you have to **type in the damage and your final position here**. In this case, we've damaged one front wing, costing us a mere 450$ to fix(funny, because the formula ford doesnt really have a front wing), which will of course differ depending on the car. The position is only relevant for future statistics and does not influence your income or anything.

### The Race Session

*Example of the Race Session Window*

<img src="https://github.com/ifeelgitty/Racing-Career-Manager/blob/Readme/tut-img/RaceView.PNG?raw=true"  title="Race" width=712>

As for the practice views, the race view includes a **section for damage** obtained during the race and the **Final Position**. Additionally, you can indicate your **final state, whether you've finished or not**. Only if you qualy as a finisher, you will receive Prize Money. You also have to **indicate your championship position after the race**. This is for statistical purposes, but the championship position after the final race counts as your final championship position, based on which the season prize money will be calculated.

In the example above, we've finished second, which, as this is the first race, also means that we're currently second in the championship. Deducting the costs for the weekend damages, adding up to 1,125$, we end up with a total weekend gain of about 31,000$(excluding the cost for signing up for the race).

And the end of the race weekend, a summary of the weekend will be shown. The same is true for the end of the season. Both are so far in a quite early state, and I am expecting to implement quite nice stats and other feature that make this more alluring.
