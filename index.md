# Welcome to my English Blog 

This is the English Version of my Blog i do really quick writeups here in none corrected slang. While i try to improve them over time.
I do not maintain a German one at present but maybe i will do a youtube channel.

## 01-10-2022 Update
i am trying to sum up the learnings from the v8 heads and try to explain why stealify is better then dart and the other concepts
- https://www.youtube.com/watch?v=P8ltWIqDPzo

In general it is importent to mention that classes and inharitance are not for code reuse they need to get avoided functional reactive programming is the feature classes where needed in a none event stream driven point in time today we want to express not only our code intend we also need flow controll cross multiple Environments and CPU Cores. This brings total new Challenges to a Coding Language while the good news is that writing functions that return functions is the way to go in ECMAScript and all other languages (Kotlin shows that well) 

i want to demo and talk about es4x compared to raw Java and why it is the future of all Languages that run on the JVM via GraalVM.

Most importent is the Concept of functional reactive streams as functions combined with a scheduler i need to talk more about the learnings of implementations like most and nils (native interactive live streams) i also need to explain eventing and promise chain streams.

i also need to talk more about just js and the future of Coding. I Try to record a Podcast in English and German. 

- Reduced boilerplate.
- better show intent. 

I need to invest more into iterator stream talks and generator stream talks and make the people understand more fast at scale while reading such text from me why they need to use that i need text examples that i put side by side so they get the concepts.

for example every Java code should get rewriten to GraalJS to speed up Application Development also for interop graal-node inlining and mksnapshot need talks to explain why this leads to faster consistent modular code reuse with less code.


## September Update

### stealify-fs 
will replace the pnp spec designed resolve algo inside Yarn and Pnpm and this way add Pnp support to Npm and all other package managers via native filesystem capabilitys powered by btrfs windows users will use https://github.com/maharmstone/btrfs or wsl maybe supported this is work in progress but ntfs will get replaced by btrfs anyway to algin the filesystem research of Stealify and overall Filesystem Development

see: 
- [ ] - https://github.com/stealify/fs/issues
- [ ] - https://github.com/frank-dspeed/berry/issues
- [ ] - https://github.com/frank-dspeed/pnpm/issues

### stealify-b8g
Big Engine will Implement a Engine spec and Compiler backend including feedback interface that Produces software as collection of stealify context objects same format also used in v8 as snapshot format. b8g is the default target for the Stealify Compiler.

we plan to implement b8g for deno as also just js so we can all 3 use the same results 
note we do not plan to get this working with NWJS or ELECTRON as both do use modifyed v8 and so fall out of Compat but maybe we can later evaluate on the idea of implementing it via the stealify compiler when it targets for example mksnapshot of ELECTRON or NWJS. 

see: [https://github.com/stealify/fs/issues](https://github.com/stealify/fs/issues)

### stealify-context
A Specification for a Context at present we share that with raw v8 but it is planed to extend that so that we can make that stable.
