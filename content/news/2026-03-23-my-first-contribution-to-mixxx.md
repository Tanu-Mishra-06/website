---
Title: My First Contribution to Mixxx through WOC
Author: Tanu Kumari
Date: 2026-03-23
---

# My First Contribution to Mixxx through WOC

## 1. How I Ended Up Contributing to Mixxx

I have always been fascinated by programs like GSoC, but I honestly thought they were only for very experienced students. So when a message about Winter of Code (WOC) suddenly appeared in my college WhatsApp group, I opened it mostly out of curiosity. I just wanted to see what it was about , not because I thought I would actually get in.

But the moment I opened the form, reality hit me. It was asking for things like my GitHub profile, LinkedIn account, past projects, and previous open-source contributions. The problem? I was in my first semester. My “project experience” at that time was basically one thing , building an AI assistant called JARVIS for a college hackathon (which somehow even won first prize). That was great, but compared to students who had already been coding for years, I was completely sure my application was going to be rejected.

Still, I filled the form anyway, mostly thinking, “Let’s just try once and see what happens.” And then something unexpected happened , I actually got accepted into the program. I still remember how excited I was because getting this opportunity in the very first semester felt unreal

Of course, the excitement didn’t last peacefully for long. The next round required us to send detailed project proposals to three organizations of our choice. Not just a simple idea , a proper plan with timelines, technical explanation, and what exactly we were going to build. I spent hours writing and rewriting those proposals, constantly asking seniors in my college to review them and tell me what was wrong. I am pretty sure they were more confident about my proposal than I was.

One of the organizations I chose was Mixxx, and honestly, the reason was simple: the idea of working on software related to music sounded too interesting to ignore. Most student projects involve websites or small applications, but this was completely different. The thought that I could work on something that actually processes sound in real time made the project feel much more exciting.

And then came the part I still don’t fully believe , I actually got selected for Mixxx. At that point, I was still convinced that they would probably choose someone more experienced. But instead, they gave a first-year student a chance. Looking back now, I think that moment was when I truly realised how welcoming the open-source community can be.


## 2. My First Reaction After Opening the Codebase

I was honestly shocked.

I already knew C++ and I was comfortable writing programs in it, so I thought understanding the code would just take some time. But the moment I opened the Mixxx codebase, I realised this was something completely different. This was not a small college project where everything fits into a few files. This was a real, large-scale application with thousands of lines of code, and suddenly everything looked much more serious.

The first challenge was simply building Mixxx on my laptop. And just to make the situation more interesting, I was doing all of this on an i3 laptop. At the beginning, it felt like every time I tried to build the project, a new error would appear. Sometimes it was one error, sometimes it was many, and most of the time I had no idea what the error message even meant. It was frustrating, but at the same time it was also strangely exciting because I knew that if I could get through this part, I would learn a lot.

After trying again and again (and probably testing the patience of my laptop more than necessary), the build finally worked. It took almost a week, but when it finally succeeded, it felt like a huge achievement. That was the moment when I started feeling that I might actually be able to contribute to this project.

I had already joined the Zulip chat earlier when I was preparing my proposal, because at one point I had decided that even if my proposal was not accepted, I still wanted to try contributing to Mixxx. So after the proposal was accepted and the build was working, I started communicating more actively with my mentors. Their first suggestion was simple: take some time and go through the codebase slowly before making any changes.

That is exactly what I did. Instead of rushing into coding, I spent time reading the files, trying to understand how different parts were connected, and especially how the audio effects worked internally. At first it felt confusing, but after a few days it slowly started making sense. The mentors also made it clear that there was no pressure and that I could take as much time as I needed to understand the project properly.

Even though there was no pressure from their side, I knew that WOC had a timeline and I wanted to use the time properly. So I tried to stay consistent and keep learning something new every day. In the end, it took me around two to three weeks to feel comfortable with the structure of the codebase, and that process itself was one of the most valuable parts of this experience.


## 3. The Idea: Can We Combine Reverb with a Band-Pass Filter?

While preparing my proposal, we were asked to choose projects from the list provided by the organizations. I went through the Mixxx ideas very carefully because I didn’t want to choose something randomly. I wanted a project that would actually teach me something new and also feel interesting enough to work on for weeks.

That is when I saw the idea of combining a band-pass filter with the reverb effect. At first, I only understood the concept at a basic level: a band-pass filter allows only a specific range of frequencies to pass, while reverb adds depth and space to the sound. The idea of combining both of them meant that instead of applying reverb to the entire sound, it would only affect a selected frequency range. Even though I had never worked with audio processing before, the idea itself sounded very interesting and different from typical beginner projects.

After the proposal was accepted and I started working on the code, I slowly began understanding how the existing reverb effect in Mixxx was implemented. My main task was to experiment with adding a band-pass stage into the effect and see how it changed the sound. This involved going through the reverb source files, understanding how the audio signal flows through the effect, and then adding new parameters that could control the band-pass filter, such as the frequency range and the Q value.

One of the most interesting parts of the project was testing how small changes in these parameters affected the sound. Sometimes the difference was very subtle, and sometimes it completely changed how the effect sounded. This made the process much more practical than just writing code, because I had to actually listen carefully and understand what the code was doing to the audio signal.

I also learned how audio effects are not only about writing new code but also about integrating it properly into an existing system. That included making sure the effect builds correctly, making sure the parameters appear properly, and testing whether the behaviour is consistent. Even though the idea looked simple at first, working on it helped me understand how complex real audio processing can be.

Looking back, this part of the project was where I learned the most technical things. It helped me understand how a real audio effect is structured, how parameters control the sound, and how experimenting step by step can turn a simple idea into something that actually works inside a real application like Mixxx.


## 4. The Moment I Realised Open Source Is Not Just Coding

When I first started working on the project, I thought the hardest part would be writing the code. I assumed that if the code builds successfully and the effect works, then the task is basically done. But very soon, I realised that open-source development works very differently from what I had imagined.

The first time I started experimenting with the reverb and the band-pass filter, I was mostly focused on making the idea work somehow. If the code compiled and the effect was visible, I felt like I was making good progress. But when I shared my changes and started getting feedback from my mentors, I understood that the goal was not just to make something work — the goal was to make it work in the right way.

Instead of just pointing out mistakes, the mentors explained why certain changes were not a good idea in the long run. One of the biggest things I learned was when they suggested that instead of modifying the existing reverb effect directly, it would be better to create a separate effect for the band-pass version. At first, I thought modifying the existing effect would be easier, but their explanation made a lot of sense. A real project needs to stay stable for users, and new features should not break something that is already working perfectly.

That was the moment when I realised that open-source development is not only about writing code — it is also about thinking like a developer who is working with a team. Things like code structure, maintainability, and long-term stability matter just as much as the idea itself. It also taught me how important feedback really is. Instead of feeling discouraged, I started seeing every review as something that was helping me improve.

Another thing that completely changed my mindset was the pull request process — because this was actually my first real pull request. Before this, I had never contributed to a large open-source project, so the idea that real developers would read my code, review it, and suggest improvements felt both exciting and a little scary. When I finally created my first PR, I remember checking it again and again just to make sure I hadn’t done something completely wrong.

But the experience turned out to be much more positive than I expected. Instead of rejecting it immediately, the mentors reviewed it carefully and explained what could be improved and why. Every small suggestion taught me something new — sometimes about C++, sometimes about how audio effects are implemented, and sometimes about how large projects are managed. That was the moment when I realised that a pull request is not just about submitting code, it is actually a way to learn.


## 5. What This Project Actually Changed for Me

When I started this project, I honestly didn’t think I would reach this point. At that time, I was just a first-semester student who was curious about open source and not very confident about contributing to a large project. But somewhere during this journey, that feeling slowly started to change.

The biggest change for me was confidence. Before this, I used to think that large codebases were only for very experienced developers and that beginners could not really understand them. But after spending weeks reading the code, building it, experimenting with the effects, and finally creating my first pull request, I realised that it is not about knowing everything from the beginning. It is about being patient and learning step by step.

Another important thing this project changed was the way I look at programming itself. Earlier, programming mostly meant writing small programs or solving problems. But working on Mixxx showed me what real software development actually looks like — reading other people’s code, understanding how different parts are connected, improving something that already exists, and learning from feedback. That experience felt completely different from anything I had done before.

This project also helped me become much more comfortable with C++. At the beginning, I understood the language, but I had never used it in such a large and real-world project. Now I feel much more confident reading and understanding complex code, and that is something I did not expect to learn so quickly.

But more than the technical things, what stayed with me the most is the experience of contributing to something real. Knowing that I worked on a project that is used by people around the world feels very different from working on small personal projects. It makes you feel that what you are learning actually matters.

If there is one thing I learned from this experience, it is that open source is not only for experts. Even a first-year student can start contributing if they are curious enough and willing to keep trying. And for me, this project was not just about adding a new effect — it was the moment when open source stopped feeling scary and started feeling possible.














