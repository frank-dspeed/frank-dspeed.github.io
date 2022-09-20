# Welcome to my English Blog 

This is the English Version of my Blog i do really quick writeups here in none corrected slang. While i try to improve them over time.
I do not maintain a German one at present but maybe i will do a youtube channel.

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
