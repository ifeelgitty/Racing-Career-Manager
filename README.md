# Racing-Career-Manager

As someone who has been playing racing simulators for nearly a decade now, something has always been missing: (A girlfriend?) A long-term motivation like it was found in the early Gran Turismo games, the feeling of **buying and owning cars, racing for a reason, climbing through the stages of motorsport, earning licenses etc.** While most modern racing simulator-creators will spend loads of money and months on getting the air pressure simulation of the tyres right, none of them really seemed to care about this part of the experience. This ends now(a bit)! Because I'm working on a free and simple(and ugly) software which simulates this career, **embedding any simulator to buy cars, race championships and ultimately work yourself through the ranks of racing**. 

## A Disclaimer

This software has been created to help you keep track of your career, allowing for any simulator and any combination of different simulators to be used in context of a racing career. What it does not do though is: Read out results from your game or save championship standings with points etc. **You actually have to keep track of the championship standings inside the game(AMS, AC, RRR) or with additional software(rf2) and then type in the position you scored in as well as the damage your car had into the software, so it can calculate all the relevant measures.** As this is a one-person project and the world of racing simulators moves fast, too many resources would have to go into developing plugins, which probably are out of date easily anyway.

## What it offers

Racing yourself through the career ladder, signing up for different racing series, going through cycles of seasons. And the best thing: Everything is **moddable**. The car list as well as the different racing series are saved as **csv files, so as tables, which means that you can add your favorite cars and racing series and combine different games**. You're not set to just one simulator. So, if you prefer the F1 cars in Assetto Corsa over the ones in Automobilista, just use them! 

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

## Managing your Finances 

This also brings us to another aspect: Finances! You will have **costs and a revenue stream** that needs to be balanced to not break the bank. You will purchase cars, sign up for testing, sign up for racing series and sign up for races. You will also have to **pay for damages** to your car in any of those sessions. Income is provided by **prize money** that you can win both by finishing well in races and the overall championship. By finishing rather high in the standings, you will gain enough profit to finance taking part in a higher-staged championship in the following season. But even if you’re in the lower part of the field, you are still well-capable to support another season in the same category. This corrects something I have never been fond of in some racing games: **It is not at all expected of you to always win championships to advance in your career, it should rather be the exception**. Also: As long as you’re somehow competitive, even if just occasionally getting into the top 10, this is typically enough to stay in the same category.

## The Calendar

*Example Screenshot of the Calendar. Obviously, February is not the most active month yet, so expect more races later in the year.*

<img src="https://github.com/ifeelgitty/Racing-Career-Manager/blob/Readme/tut-img/Calendar.PNG?raw=true"  title="Example of F1 Season" width=712>

Like Julius Caesar, I feel entitled to slightly modify the workings of our calendar. **Every month is simply split into 4 weeks**, without specific days or anything. This is totally not done because I’m too lazy to properly implement a calendar (Yes, it is), but because it simplifies the process (same thing). It has another positive effect: As this calendar has 48 instead of 52 weeks, it densens the calendar a bit, compensating for the lower number of races per championship compared to real life.

Besides structuring the year, the calendar has one main effect: **You are only able to sign up for races at one location per week.** Therefore, you can for example sign up for all races at Adelaide at the same weekend(if youre eligible to participate in the respective series, of course), but not attend both a race in Adelaide and Gioania. So, **if two events at different locations overlap, choose which race is more important to you (or you might lose your championship title) and choose wisely**. Also feel free to check whether there are overlaps between multiple championships before signing up for them, so you know in advance what to expect. Of course, each series has a different start and end point of the season, based on the span in real life, so Australian Supercar races start already in February, while Formula one does not start before March.

