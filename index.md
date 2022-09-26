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

#### Conclusion from me the creator of Stealify
I have worked on OpenStack, GraalVM, v8, SpiderMonkey, Systemd, DBUS, libcontainer, WASM, RUST, LLVM, Typescript, Rollup, git subtree, WebRTC, Kubernetes, Chromium and all its flavors like Android and LaCrOS, Fuchsia OS Zircon & FIDL Design, Linux Kernel, git annex, IPFS, btrfs to name only a few Projects there where even more. What you and i maybe Observe Directly is that this is a Large Set of Really Large Software Stacks but i hope it makes sense that they are all more or less related to each other.

The Main Relations are fundamental principels and Problems they are sympthoms of problems that we try to solve in the existing ecosystem with our existing old thinking. I started to Tackle the Problems at the root and i guess i had success! I Saw the Patterns and did take away all abstractions as i saw the most where bad while there is a need for abstraction in general it is importent where we do that abstraction to do not end up in unlimited nested layers of abstraction that make our head explode.

as Many of my Loved Co Authors where i took my inspiration from and validated my results do aggree in the following rules they are fundamental

- Capability Based Protocols (handels)
- async / await 
- sharedArrayBuffers
- stdio/files is the last resort of compat and will be only needed until everything is Stealify.
- We Build Stack Machines this way we are isolated from the ground up 
- consistent
- reuseable
- simple 
- composition over inharitance
- functions can return functions but they need to produce the correct return stack a importent implementation detail.
- mutex futex pth is at present the best we did come up with because we had no flow control before now we could go deterministic
- eval is not bad for a compiler it is needed but the environment in that the evaluation happens matters. See Context concepts. Confined Isolated and so on.

Explaining why Dart was a failure but a good try. Dart in general was made with some right concepts and some wrong concepts as always.

- Classes are bad in General
- Flutter is bad in general everything that flutter does well needs to be ported to a more modular browser stack
- a new language is bad in general only to solve the module problem 
- JS Can Compile Static see mksnapshot and wasm in general it is always clever to use the Template abilitys of JS to Replace C++ Markos which are text search replace and Rust Macros which are lisp. As also follow some design patterns for the code and use Typescript annotations or JSDOC from time to time. 
- It could use LLVM 
- How Ever all that is solved with JavaScript Core which is LLVM Based.


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
