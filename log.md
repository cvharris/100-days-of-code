# 100 Days Of Code - Log

### Day 1: April 2nd 2019

**Today's Progress**: Upgrade Rolo's React-Native from 0.57.1 to 0.59.3

**Thoughts** Holy crap I hope RN gets their act together on the upgrade process soon, it is painful! Manual file updates? Who wants to do that!

**Links to work** Private repo but you can see the number of commits in my profile

### Day 2: April 3rd, 2019

**Today's Progress**: Yesterday's upgrade broke something in the app. Kept getting a 'Malformed calls from JS: field sizes are different', turned out to be an issue with styling NativeBase's header with a calculation on the StatusBar which we don't use!?

**Thoughts** both yesterday and today took entirely too long to work through and debug. Very exhausted but hoping to actually get real work done tomorrow.

### Day 3: April 4th, 2019

**Today's Progress**: Fixed a bug my brother Will discovered where Rolo would crash if a user denied having Contacts read.

**Thoughts** Probably not handling this the best way and there are possible edge cases that are not taken care of, but not sure how often a user is going to do something like this. We will put more time and thought into it once we have more data.

### Day 4: April 5th, 2019

**Today's Progress**: Fixed an issue with not being able to update the address of a new contact

**Thoughts** The issue was ultimately due to a mispelled prop on the container using the component, which I guess is what Typescript is supposed to help with but I'm not about to start using that this late into the project.

### Day 5: April 6th, 2019

**Thoughts** Got to read up on transducers which offerred new ideas for how I transform a bunch of data around the app, hoping to find out if reselect already does most of this under the hood.

### Day 6: April 7th, 2019

**Today's Progress** Replaced NativeBase's DatePicker with a new component from React Native Modal DateTime Picker. Used my first hook in an app too with `useState`

**Thoughts** Now I see what all the talk is on hooks, they're really awesome. They afforded me the ability to be more declarative with my component's logic without rewriting it into a class. Also the user experience from the new Date picker is sooo much better than NativeBase's, and I can make it do whatever I want.
