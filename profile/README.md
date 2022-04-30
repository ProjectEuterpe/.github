<p align="center">
  <img src="https://github.com/ProjectEuterpe/.github/blob/main/profile/projecteuterpe.png" width=50% height=50%>
</p>

## Project Euterpe
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

### Introduction
- [Who is Euterpe anyway?](#who-is-euterpe-anyway)
- [What exactly we are doing?](#what-exactly-we-are-doing)
- [What we designed the architecture to be?](#what-we-designed-the-architecture-to-be)
- [How will users interact with the application?](#how-will-users-interact-with-the-application)

### Who is Euterpe anyway?
[Euterpe](https://en.wikipedia.org/wiki/Euterpe) is one of the Muses in Greek mythology, presiding over music. We hope our desktop player will play media files properly and smoothly, which could give users excellent experience when enjoying music and videos, as the goddess Euterpe has done to entertain the gods on Mount Olympus.

### What exactly we are doing?
Project Euterpe is our software engineering course project. This project requires to implement a desktop audio and video player which is capable to play media files in various formats, manage media library, etc. This project covers the common desktop technology stacks. Read [this document](https://bytedance.feishu.cn/docx/doxcnIFNVSangxAHqoUlRolZQ3e) for further understanding of what we should do in this project.

### What we designed the architecture to be?
The overall architecture of this project is as follows:

<p align="center">
  <img src="https://github.com/ProjectEuterpe/.github/blob/main/profile/arch.png" width=80% height=80%>
</p>

The basic design idea of the project is to separate front-end and back-end development, using Qt framework to implement UI, interaction, asynchronous control and connection to back-end database. The project is using MVC (Model-View-Controller) design pattern, with the playback engine as the model part, the media library and the playback component as the view part, and the signal-and-slot-based asynchronous calls as the controller part. Read our [Architecture Design Document](https://enedlzm696.feishu.cn/docs/doccnDZX0rMaPVhaMSsHY9caj3g) for further understanding of the architecture design.


### How will users interact with the application?
The application is designed to be able to display and control media playback volume, progress, status, playback mode, etc. Users can get metadata of media files easily. The application provides a media library (playlist) which allows users to import media files by drag-and-droping or clicking the `open` button. This application's controller UI is made up of these components:
1. volume controller: `mute` button and volume slider bar;
2. progress controller: playback progress slider, current playback progress and total playback duration of media file;
3. playback status controller: `prev`/`next` button, `play`/`pause` buttton;
4. play mode controller: the button which supports playmode changes in "list loop", "sequential", "shuffle" and "single loop";
5. screen mode controller: the button which could switch the screen mode between "normal", "full screen" and "floating".

Read our [Interaction Design Document](https://enedlzm696.feishu.cn/docs/doccnGP9zYPlY059A3I4s8UCCQb) for further understanding of the interaction design.
<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
