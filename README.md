# Audio Intent Detection - Classification Problem

## Problem Description
Intent detection is a crucial task in the field of natural language processing (NLP) and speech recognition.
It involves identifying the underlying intention or purpose of a spoken or written statement. This task
is particularly important in the development of voice assistants and other audio-based applications, as it
allows the system to understand and respond appropriately to the user’s requests and commands.
In the context of audio intent detection, the system must be able to accurately interpret the user’s spo-
ken words and determine their intended meaning. This requires the system to have a deep understanding
of language and context, as well as the ability to recognize and differentiate between different intents or
purposes.
The importance of accurate audio intent detection cannot be overstated. It plays a vital role in the
usability and effectiveness of voice assistants and other audio-based applications, and can greatly impact
the user experience. A system that is unable to correctly interpret the user’s intentions will be frustrating
and difficult to use, leading to a poor user experience and potentially even causing the user to abandon
the application altogether. On the other hand, a system that is able to accurately detect and respond to
the user’s intentions will be much more user-friendly and effective, leading to a better overall experience
for the user.
In this project, given an input audio sample, the goal is to predict both the action requested and the object 
that is affected by the action.

## Dataset 
The dataset consists in a collection of audio file in a WAV format. Each record is characterized by several
attributes. The following is a short description for each of them.
* path: the path of the audio file.
* speakerId: the id of the speaker.
* action: the type of action required through the intent.
* object: the device involved by intent.
* Self-reported fluency level: the speaking fluency of the speaker.
* First Language spoken: the first language spoken by the speaker.
* Current language used for work/school: the main language spoken by the speaker during daily activities.
* gender: the gender of the speaker.
* ageRange: the age range of the speaker.
An intent is given by the combination of an action with an object, therefore the information in the two
respective columns must be combined to obtain the label to be used to address this task. The way this
information should be combined is a simple string concatenation (e.g., if the action is “increase” and the
object is “volume”, the corresponding intent will be “increasevolume”).

