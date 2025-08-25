#artifact 

The intention is to solve the problem outlined by three core pillars required for a successful weightlifting planning app.

This is the initial idea I have. It would probably the most straightforward in terms of actual problems it is attempting to solve, and I also have a relatively clear idea of how to actually implement. This, however, might be the most time-consuming project - I would actually be worried about possibly not fitting into the 400 hour time-frame, to actually get it fully implemented in terms of the whole feature-set.

Main problem would likely be surrounding front end design. While I have worked with UI design on android before, I never really got to any of the custom parts of Jetpack Compose or Flutter. As such, a lot of the more complex visualizations I actually have no idea how to design, and last time I didn't find a solution. Alternatively I could do it natively, but then I have never actually worked directly with React.

# Statistical Planning

There is an opportunity in that, for weightlifting, there *is* a limited amount of actual relationships between statistics and actual practical working metrics, so it can possibly be modeled once, and then adjusted through weights.

This is the "Excel" breed of software. It's the ability to feed data back into planning. As example, base a working set on current 1 rm, current week in a cycle, level of perceived exertion, etc. But it somehow needs to accurately account for the "fuck it we ball" aspect too - sometimes you will overtrain because you had a coffee on a given day, or miss a day entirely, increasing your rest. But also that depends on person.  Some form of extra metric for creating weights for the specific user?

## Possible Statistical Features
- Calculating future working weight off of current cycle based on week + 1rm
- Calculation of user-specific baseline statistics, such as recovery speed (short term and long term), sleep needs, work capacity, muscle retention
- Deload prediction based on baseline statistics + current cycle
- Calculation of proximity to failure based on 1rm, volume, reps, number in the set
- Building around both linear AND undulating progression
- Hypertrophy, cutting, and maintenance modes based on baseline statistics + past performance
- Daily/Per session metrical and perceived performance tracking
- Support for movement pattern/muscle group, AND commonly used exercise based progression tracking.
- Adjacent information tracking, such as: sleep quality, daily non-fitness physical expenditure (for integrated approximate total energy expenditure tracking)
- Formation of returning-to-the-gym-after-long-pause plans based on previous data + exercise frequency

# Absolute Control Over Measurement Metrics
There is an issue in that there is often a lack of specific tracking metrics/patterns. Great example is HIIT, or rate of perceived exertion. In FitnessPlan, you're stuck using cardio metrics for HIIT, and pray to god you remember rate of exertion. 

## Possible Metric Features
Either attempt to account for all metrics, or give flexible metrics that can be created on the fly. First option gives easier connection to statistics, the other gives greater flexibility.
- Extended tracking options: HIIT bouts, Rate of Perceived Exertion, Weight based on 1rm, Muscle group volume contribution, HIIT vs Steady State metrics, Max Heart Rate, Range of Motion, modifiers and effects, possibly more
- Integration of all metrics into comprehensive tracking along exhaustive number of vectors that may be relevant for fitness
- Flexible and customizable per-set + per-workout information: someone might only do reps + weight, someone reps + 1rm percentage, someone weight + proximity to failure. Other statistics could either be ignored or inferred based on collected data
- Custom notes/direction for individual lifts
- Custom lift creation (obviously)
- Muscle group organization (cover ALL the muscles a lift covers, in users opinion)
- Visualization for all this shit
# Psychological Buy-In
This is less about being consistent in going to the gym - that is not an issue that needs to be resolved, as practically anyone who is consistent is insane about it. The issue that needs solving is buy-in for the *software*. In case where long-term automated planning needs user input over-time, there is a need to somehow create amount of user-usage that is consistent *enough* to get the necessary data in the first place. This requires some form of addictive retention method to actually make such usage consistent.

I am guessing classic balance is at play - reduce friction to a minimum, create sensory feedback. Look into duolingo, snapchat, dailies/weeklies in general.

Perhaps feature unlock not through payment, but through usage - borrow directly from gamification.

## Possible Gamification Features
- Flexible accountability options: Daily/Weekly/Monthly or undulating, something like 4 out of 7 days a week, or minimum + extra work rewards
- Reward for feeding statistical information the app
- Daily questionnaire of different levels of complexity/completeness
- Unlockable higher precision tracking through consistent usage
- Incentive to track days/weeks/months when you FAIL to go to the gym - to feed into comeback plans + baseline tracking
- Setting of goals
- Showing of strengths and weaknesses
- Showing progression towards goals
- Possible cosmetic customization
- Possible quests for parts of fitness that are lagging/under represented
# Inspirations
Inspirations are Duolingo, Kanji Academy, MyFitnessPlan.

