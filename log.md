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

### Day 7: April 8th, 2019

**Today's Progress** Mentored @nblaida on the website she's building and at first I wasn't going to count it but no, that was definitely coding too!

### Day 8: April 9th, 2019

**Today's Progress**  Back to my own code and fixed a bug in my selectors that hid users with no email, phone, or home address

### Day 9: April 10th, 2019

**Today's Progress** Added age and all parents & children to ContactProfile so even step parents and step children are shown. However the Profile is not updated yet, because they share so much logic and will have to be refactored with some kind of selector, I'm not sure, but it might improve performance.

### Day 10: April 11th, 2019

**Today's Progress** Added siblings to the contact details and profile, a nice added calculation that I hope sets the stage for future relationship calculations

**Thoughts** In order to make it less of a headache to tinker with the logic to pull in all this relational data on a contact I had to create a selector factory, my first time doing so. It was super easy and makes the code super reusable.
