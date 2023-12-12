I have constructed a predictive model for estimating a players FPL points aquired in the upcoming gameweek (xP). I formed this as a regression problem where averages of recent 
form and fixture data were used as features (credit to https://github.com/vaastav/Fantasy-Premier-League for the raw data). Wherever possible I used underlying data (xG, xA, ICT ...) 
as opposed to previous perfomance (goals, assists, points) to try and get a unique point of view.

Since many of the features were highly correlated (eg xA, Creativity, bps ...), I found Ridge linear regression gave the best results, since it handles this situation well. The classes I have
build can be experimented with and fine-tuned to produce more impressive results. 

I also imported this season's premier league fixtures data to allow for predictions for the upcoming gameweek to be made (since the original dataset contained no information on upcoming fixtures).
