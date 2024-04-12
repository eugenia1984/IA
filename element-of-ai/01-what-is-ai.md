# <img width="34" height="34" src="https://img.icons8.com/nolan/34/artificial-intelligence.png" alt="artificial-intelligence"/> What is AI

##  <img width="34" height="34" src="https://img.icons8.com/nolan/34/artificial-intelligence.png" alt="artificial-intelligence"/> How should we define AI? 

In our very first section, we’ll become familiar with the concept of AI by looking into its definition and some examples.

As you have probably noticed, AI is currently a “hot topic”: media coverage and public discussion about AI is almost impossible to avoid. However, you may also have noticed that AI means different things to different people. For some, AI is about artificial life-forms that can surpass human intelligence, and for others, almost any data processing technology can be called AI.

To set the scene, so to speak, we’ll discuss what AI is, how it can be defined, and what other fields or technologies are closely related. Before we do so, however, we’ll highlight three applications of AI that illustrate different aspects of AI. We’ll return to each of them throughout the course to deepen our understanding.

## Application 1. Self-driving cars

Self-driving cars require a combination of AI techniques of many kinds: search and planning to find the most convenient route from A to B, computer vision to identify obstacles, and decision making under uncertainty to cope with the complex and dynamic environment. Each of these must work with almost flawless precision in order to avoid accidents.

The same technologies are also used in other autonomous systems such as delivery robots, flying drones, and autonomous ships.

**Implications**: road safety should eventually improve as the reliability of the systems surpasses human level. The efficiency of logistics chains when moving goods should improve. Humans move into a supervisory role, keeping an eye on what’s going on while machines take care of the driving. Since transportation is such a crucial element in our daily life, it is likely that there are also some implications that we haven’t even thought about yet.

### Application 2. Content recommendation
A lot of the information that we encounter in the course of a typical day is personalized. Examples include Facebook, Twitter, Instagram, and other social media content; online advertisements; music recommendations on Spotify; movie recommendations on Netflix, HBO, and other streaming services. Many online publishers such as newspapers’ and broadcasting companies’ websites as well as search engines such as Google also personalize the content they offer.

While the frontpage of the printed version of the New York Times or China Daily is the same for all readers, the frontpage of the online version is different for each user. The algorithms that determine the content that you see are based on AI.

**Implications**: while many companies don’t want to reveal the details of their algorithms, being aware of the basic principles helps you understand the potential implications: these involve so called filter bubbles, echo-chambers, troll factories, fake news, and new forms of propaganda.

### Application 3. Image and video processing
Face recognition is already a commodity used in many customer, business, and government applications such as organizing your photos according to people, automatic tagging on social media, and passport control. Similar techniques can be used to recognize other cars and obstacles around an autonomous car, or to estimate wildlife populations, just to name a few examples.

AI can also be used to generate or alter visual content. Examples already in use today include style transfer, by which you can adapt your personal photos to look like they were painted by Vincent van Gogh, and computer generated characters in motion pictures such as Avatar, the Lord of the Rings, and popular Pixar animations where the animated characters replicate gestures made by real human actors.

**Implications**: when such techniques advance and become more widely available, it will be easy to create natural looking fake videos of events that are impossible to distinguish from real footage. This challenges the notion that “seeing is believing”.

## What is, and what isn’t AI? Not an easy question!

The popularity of AI in the media is in part due to the fact that people have started using the term when they refer to things that used to be called by other names. You can see almost anything from statistics and business analytics to manually encoded if-then rules called AI. Why is this so? Why is the public perception of AI so nebulous? Let’s look at a few reasons.

### Reason 1: no officially agreed definition

Even AI researchers have no exact definition of AI. The field is rather being constantly redefined when some topics are classified as non-AI, and new topics emerge.

There’s an old (geeky) joke that AI is defined as “cool things that computers can’t do.” The irony is that under this definition, AI can never make any progress: as soon as we find a way to do something cool with a computer, it stops being an AI problem. However, there is an element of truth in this definition. Fifty years ago, for instance, automatic methods for search and planning were considered to belong to the domain of AI. Nowadays such methods are taught to every computer science student. Similarly, certain methods for processing uncertain information are becoming so well understood that they are likely to be moved from AI to statistics or probability very soon.

### Reason 2: the legacy of science fiction
The confusion about the meaning of AI is made worse by the visions of AI present in various literary and cinematic works of science fiction. Science fiction stories often feature friendly humanoid servants that provide overly-detailed factoids or witty dialogue, but can sometimes follow the steps of Pinocchio and start to wonder if they can become human. Another class of humanoid beings in sci-fi espouse sinister motives and turn against their masters in the vein of old tales of sorcerers’ apprentices, going back to the Golem of Prague and beyond.

Often the robothood of such creatures is only a thin veneer on top of a very humanlike agent, which is understandable as most fiction – even science fiction – needs to be relatable by human readers who would otherwise be alienated by intelligence that is too different and strange. Most science fiction is thus best read as metaphor for the current human condition, and robots could be seen as stand-ins for repressed sections of society, or perhaps our search for the meaning of life.

### Reason 3: what seems easy is actually hard...
Another source of difficulty in understanding AI is that it is hard to know which tasks are easy and which ones are hard. Look around and pick up an object in your hand, then think about what you did: you used your eyes to scan your surroundings, figured out where are some suitable objects for picking up, chose one of them and planned a trajectory for your hand to reach that one, then moved your hand by contracting various muscles in sequence and managed to squeeze the object with just the right amount of force to keep it between your fingers.

It can be hard to appreciate how complicated all this is, but sometimes it becomes visible when something goes wrong: the object you pick is much heavier or lighter than you expected, or someone else opens a door just as you are reaching for the handle, and then you can find yourself seriously out of balance. Usually these kinds of tasks feel effortless, but that feeling belies millions of years of evolution and several years of childhood practice.

While easy for you, grasping objects by a robot is extremely hard, and it is an area of active study. Recent examples include for example [Boston Dynamics robots](https://www.youtube.com/watch?v=-e1_QhJ1EhQ).


### ...and what seems hard is actually easy

By contrast, the tasks of playing chess and solving mathematical exercises can seem to be very difficult, requiring years of practice to master and involving our “higher faculties” and concentrated conscious thought. No wonder that some initial AI research concentrated on these kinds of tasks, and it may have seemed at the time that they encapsulate the essence of intelligence.

It has since turned out that playing chess is very well suited to computers, which can follow fairly simple rules and compute many alternative move sequences at a rate of billions of computations a second. Computers beat the reigning human world champion in chess in the famous Deep Blue vs Kasparov matches in 1997. Could you have imagined that the harder problem turned out to be grabbing the pieces and moving them on the board without knocking it over! We will study the techniques that are used in playing games like chess or tic-tac-toe in Chapter 2.

Similarly, while in-depth mastery of mathematics requires (what seems like) human intuition and ingenuity, many (but not all) exercises of a typical high-school or college course can be solved by applying a calculator and simple set of rules.

## So what would be a more useful definition?

An attempt at a definition more useful than the “what computers can’t do yet” joke would be to list properties that are characteristic to AI, in this case autonomy and adaptivity.

```
Key terminology
Autonomy:  The ability to perform tasks in complex environments without constant guidance by a user.

Adaptivity: The ability to improve performance by learning from experience.
```

### Words can be misleading

When defining and talking about AI we have to be cautious as many of the words that we use can be quite misleading. Common examples are learning, understanding, and intelligence.

You may well say, for example, that a system is intelligent, perhaps because it delivers accurate navigation instructions or detects signs of melanoma in photographs of skin lesions. When we hear something like this, the word “intelligent” easily suggests that the system is capable of performing any task an intelligent person is able to perform: going to the grocery store and cooking dinner, washing and folding laundry, and so on.

Likewise, when we say that a computer vision system understands images because it is able to segment an image into distinct objects such as other cars, pedestrians, buildings, the road, and so on, the word “understand” easily suggest that the system also understands that even if a person is wearing a t-shirt that has a photo of a road printed on it, it is not okay to drive on that road (and over the person).

In both of the above cases, we’d be wrong.

```
Note

Watch out for “suitcase words”

[Marvin Minsky](https://en.wikipedia.org/wiki/Marvin_Minsky), a cognitive scientist and one of the greatest pioneers in AI, coined the term suitcase word for terms that carry a whole bunch of different meanings that come along even if we intend only one of them. Using such terms increases the risk of misinterpretations such as the ones above.
```

---

##  <img width="34" height="34" src="https://img.icons8.com/nolan/34/artificial-intelligence.png" alt="artificial-intelligence"/>  Related fields 

---

##  <img width="34" height="34" src="https://img.icons8.com/nolan/34/artificial-intelligence.png" alt="artificial-intelligence"/>  Philosophy of AI

---
