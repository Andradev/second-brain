---
title: "How Senior Engineers Actually Build With AI in 2026 | Build a Full Stack Systems Architecture App"
source: "https://www.youtube.com/watch?v=14RP8liACqo&t=2636s"
author:
  - "[[JavaScript Mastery]]"
published: 2026-05-01
created: 2026-05-10
description: "Build a production-ready SaaS without writing code by hand. Architecture-first workflow, proper context management for AI agents, and a real app shipped with Next.js, Prisma, Postgres, TypeScript, and"
tags:
  - "WebClip"
---
![](https://www.youtube.com/watch?v=14RP8liACqo)

Build a production-ready SaaS without writing code by hand. Architecture-first workflow, proper context management for AI agents, and a real app shipped with Next.js, Prisma, Postgres, TypeScript, and Tailwind.  
  
Clerk: https://jsm.dev/ghost-clerk  
Trigger.dev: https://jsm.dev/ghost-triggerdev  
Liveblocks: https://jsm.dev/ghost-liveblocks  
CodeRabbit: https://jsm.dev/ghost-coderabbit  
  
📘 FREE Six-File Methodology for Spec-Driven Dev: https://jsm.dev/ghost-context  
📋 Join the Agentic Course Waitlist: https://jsm.dev/ghost-agentic  
🎁 Video Kit (Code, Assets, Prompts): https://jsm.dev/ghost-kit  
⭐ Join JS Mastery Pro: https://jsm.dev/ghost-jsm  
  
➤ Links not working? Some regions may need a VPN.  
  
https://discord.com/invite/n6EdbFJ https://twitter.com/jsmasterypro https://instagram.com/javascriptmastery https://linkedin.com/company/javascriptmastery  
  
Business Inquiries: contact@jsmastery.pro  
  
Timestamps:  
00:00:00 — Introduction  
00:03:15 — Crash Course  
00:14:31 — Project Setup  
00:21:43 — Preparing Context  
00:39:51 — UI Primitive Components  
00:48:14 — Layout Setup  
00:58:17 — Authentication  
01:21:05 — Project Dialogues  
01:31:00 — Prisma Setup  
01:38:58 — Project CRUD APIs  
01:51:18 — Editor: Access Sharing  
02:04:02 — Editor: Liveblocks Canvas  
02:23:54 — Editor: Canvas Features  
02:46:19 — Avatar Feature, Chat Sidebar UI & Auto Save  
03:05:01 — Trigger.dev Setup  
03:15:32 — AI Architecture Design Generation Flow  
03:39:21 — AI Spec Generation  
03:50:28 — Deployment

## Transcript

### Introduction

**0:00** · It's 2026 and most of the senior engineers I know aren't really writing code anymore. They designed the systems and let AI handle the implementation.

**0:09** · And the gap between developers who can do that and developers who can't is dividing the industry right now. This app is what that looks like when you do it well. Realtime multiplayer SAS AI agents running in the background, full production code, and I didn't write a single line of it. An agent built the whole thing. And by the end of this video, you'll have built it too. The same app, the same stack, the same way I did. And here's what makes this different from other AI build tutorials.

**0:40** · I built this app using the exact methodology the app itself is designed to teach. Specs first architecture defined every feature planned before we start building. I've been doing this architecture work by hand before every serious project for years. And at some point it hit me. I'm a developer. Why am I doing all of this manually when I could build the tool that does it with me? So I did.

**1:05** · This is Ghost AI, a real time collaborative workspace where you describe a system in plain English and an AI agent maps it onto a shared canvas live. Your team edits the design together and when it's ready, the app generates a complete technical specification you can build from. Now, if you've tried building anything serious like this with AI, you already know the wall.

**1:31** · The first few hours feel incredible, and then a week later, the agent has forgotten every decision you've made. One new feature breaks three others, and the codebase you were excited about just starts fighting you.

**1:46** · That's not an AI problem. It's an architecture problem. And it's the same wall all of you are hitting in your careers where the senior dev advice online sounds great as long as you're already senior. The developers who win in this market aren't avoiding AI and they are not handing everything over to it either. They're learning to think like senior engineers and then using AI to build at the speed of one. And that's what this video teaches.

**2:13** · By the end, you'll know how to design a system before writing any code, how to use the sixfile context system I write before every project, and how a senior engineers actually thinks when working with AI. Oh, and that sixfile context system I just mentioned, I've packaged it into a free guide you can grab and use on any of your upcoming projects, not just this one. The link is down in the description.

**2:39** · Next, the stack is Nex.js, JS React 19 live blocks for real-time collaboration with agents trigger dev for background work with AI agents clerk for o and user management prisma and posgress for data versel blob for storage all production grade and deployed by the end of the video. So, one person with the right system can now build what used to take a team. And by the end of the next few hours, that person is you. So, let's build it.

### Crash Course

**3:17** · Before we open up a single tool, I want to spend the next 10 minutes on the part of the video that I think is most important and that decides whether what you're building ships or falls apart in the third week. There's going to be no syntax and no code in this section.

**3:35** · Rather, what I'm teaching you is the way that I think before I write a single prompt and the way I plan a build before I touch the agent and the system that I use to keep AI from drifting halfway through a project so that by the end you'll know the conversations to have before you build, the six file context system that turns an AI agent from a guesser into a developer who already knows your codebase and how to break any project into units the agent can ship cleanly one at a time.

**4:07** · So, if you've been frustrated by AI breaking your code, then this is the video that fixes it. The intro touched on something I want to sit with for a minute. You heard me say senior engineers a lot. And if you're early in your career, that framing probably hit a nerve. So, let me be direct about what I mean. The job market for developers right now is harder than it was two years ago. Some entry-level work has been automated.

**4:38** · Clients who used to hire freelancers for straightforward projects are now doing it themselves. And a lot of people who learn to prompt without learning how to think are now flooding the market. So if you're worried about that, you're not wrong to be worried. But the developers getting squeezed aren't the ones who learned deeply. They're the ones who learned just enough to execute without understanding the system behind it. That was always a fragile place to be. And AI just made that fragility visible faster.

**5:12** · So the way through is to learn the kind of thinking that AI cannot replace the architectural thinking, the systems level judgment and then use AI to build at the speed of someone twice your experience. The clearer your understanding of what you're building, the better the AI output. Which means that learning properly isn't a waste of time in the AI era. It's the best investment that makes everything else possible.

**5:40** · So when I say things like think like a senior engineer in this video, I don't mean you need 10 years of experience to apply this. These are learnable habits and you can start building them today on this project. And here's something most developers outside of big tech don't really know. At Google, Amazon and Netflix, before any serious project starts, engineers spend weeks writing documents and sometimes months.

**6:09** · Design docs, one-pages, RFC's, the format changes by company, but the principle is the same. Figure out what you're building before you build it. And senior engineers at these companies sometimes go months without writing production code. They're designing systems, making architectural decisions, reviewing what other engineers ship. So software engineering has never really been about typing the most lines per day.

**6:38** · It's always been about thinking clearly about what should exist before you build it. And AI didn't invent that discipline. It just made it the most important skill in the room. And that's the whole foundation for the specdriven agentic development course that I've been developing for a long time now. So if you want to stay up to date on how that's going and receive an occasional email where I share my thoughts at the current state of the industry, I'll leave the link down below so you can subscribe for the newsletter.

**7:07** · But let me immediately make it concrete in this video. Here are two different prompts that two different developers might write to build the same feature. The first one says, "Build me a SAS app with authentication and a real-time canvas."

**7:24** · And the second one says, "I'm adding a livelocks room provider to the workspace route. O is already handled by clerk middleware. The canvas uses react flow.

**7:35** · Room tokens should be issued only after verifying project membership. Wire the provider into the existing workspace layout without touching the sidebar or navbar." Both developers want roughly the same thing, but the second prompt reveals a developer who knows their off layer, understands their component boundaries, and knows what should and shouldn't be touched. They've thought about the system, so they're communicating decisions and not wishes.

**8:05** · So, the AI isn't smarter when it reads the second prompt. The developer is. And that is the difference between vibe coding and what I'm going to teach you which is specd driven development which is also the premise behind that specd driven agentic development course that I'm actively developing. Vibe coding focuses on the outcome. You describe what you want, let the agent run, and react to whatever comes out.

**8:30** · For a weekend prototype, that's fine, but for anything you're going to maintain, it just collapses. New features break the old ones. The codebase starts contradicting itself and you spend more time untangling AI mistakes than actually building. Specdriven keeps the thinking with you and gives the agent a system to execute against. You stay the architect and the agent becomes the implementation engine. So how do you actually build that system?

**9:02** · Because that's the part that nobody really teaches. It starts before you open up any AI coding tool with a conversation.

**9:11** · When I get an idea for something I want to build, I open up a planning AI, Chad, GPT, Claude or Gemini, whichever is on hand, and I talk through it. What does this thing actually do? Who uses it?

**9:23** · What are the core flows? Where are the complex patterns? And what could go wrong? I push back on the answers and let AI pressure test my thinking until the system becomes clear in my head.

**9:36** · This conversation is the work. It's what senior engineers do before they build.

**9:41** · Except they usually do it in their head or on a whiteboard, but doing it with AI externalizes it and makes it faster.

**9:49** · When the system is clear, you write it down. And that's where the six file context system comes from. Not from sitting at a blank page trying to write documentation, but from taking the output of the architectural conversation and organizing it into documents that travel with the project for its entire life. For Ghost AI, I organized everything into one folder called context, six files.

**10:12** · And what matters is that before your AI agent writes anything, it already knows what you're building, how it fits together, what the rules are, and where things stand right now. That's what you're going to learn about in this video. But very quickly, here's what each one of them does at a glance. The project overview covers what the product is, who is it for, the core flows, and what's deliberately out of scope.

**10:39** · The architecture file defines the text stack, the boundaries between layers, and the invariance the codebase must never break. The code standards keeps the agent consistent across every unit of the build with shared TypeScript and Nex.js conventions. The AI workflow rules keep the agent disciplined, defining how to scope work and what to do when something needs a decision.

**11:02** · The UI context holds the design tokens and component conventions so the UI stays coherent across every page the agent ships. And the progress tracker, which is the one most developers skip and most need, holds the current phase, what's in progress, what's complete, and the architectural decisions made along the way. It's the only file that actually updates constantly throughout the build.

**11:30** · And it's how the agent picks up exactly where you left off in a single prompt.

**11:34** · These six files are what make the difference. An AI agent that drifts and one that executes. And you don't have to build them from scratch for every project. I've put together a free blank template of all six files with step-by-step instructions on how I generate them using AI for whichever project I'm working on. And it's not specific to Ghost AI. It works for any application. Click the link down in the description to get it so you can apply this methodology to your own projects starting today.

**12:04** · We'll open up each one of these and I'll walk you through what's actually inside in the next lesson when we set up the project architecture for real. But yeah, once these six files exist, the build runs in units. We're going to break down the project into specific scoped pieces before we start. Not vague phases like build a dashboard, but concrete units small enough to build in a single focus session with clear conditions for what done looks like.

**12:33** · That means that together for ghost AI, we'll map out the entire build. Each lesson will have its own spec file. The spec defines the goal, the design decisions, the implementation details, dependencies, and a checklist of what has to be true before the unit is complete. You write the spec in the same way you write the context file through a conversation with a planning AI. Then you give the spec to your coding agent in one prompt.

**13:01** · Make sure to read that spec, mark that unit as in progress in the progress tracker, implement it exactly as specified without going beyond scope. The agent will read your spec, read your context file, and build against a defined system instead of guessing. You review it against the checklist and if it passes, you close the unit, push the code, and move to the next spec.

**13:28** · If something's off, you write a focused corrective prompt exactly what's wrong, exactly what you expect, fix that specific thing, and move on. That's the entire workflow. The same one I used to build Ghost AI, and the same one you're about to use to build it with me. Oh, and last thing before we begin. These files take time to write. The conversation, the architectural decisions, the unit planning, all of it is real upfront work.

**13:58** · And a lot of developers skip it because they want to feel productive immediately. I mean, I've done that as well. So, you open up the agent, type a prompt, and start watching code appear.

**14:11** · But that's the trap. The time you save by skipping this is the time you'll lose in week three debugging AI output that's drifted away from anything coherent. So do this work once and you'll do it faster every project after. And finally, it's time to build.

### Project Setup

**14:33** · Okay, enough talk and let's build. Open up your desktop and create a new folder.

**14:39** · call it something like ghost AI and then simply drag and drop it into your favorite code editor. For this video, I'll be using VS Code as we have the file explorer on the left side. We have the code in the middle and then we have the chat window which you can open up by pressing command shiftp and then just search for chat or I think it's just command shift I to open it as well. No matter which agent you're using, is it Copilot, Claude, Codeex or whatever, the interface is more or less the same. This is how it looks like on Codex.

**15:10** · And this is just general chat. So this video is completely agentic tool agnostic. The thinking and the specs are what matters.

**15:22** · The tool is completely your call. I'll personally be using cloud code as that's what most people are using and what we're using internally within JSM. If you want the budget option, you can go with Codex. There's the Go plan, which is super cheap. The Plus plan, which is also cheap, and I think they're also offering a month for free. And if you're already paying for something like Cursor, Windsurf, or any other AI agent, just use that. I'll make sure you don't spend a lot of tokens, no matter what you're using, and that you'll learn a ton. Okay, so let's get started. We'll start with a fresh Nex.js project.

**15:54** · I'll do this manually with no prompts and agents. It's just a single command and it takes a couple of seconds and that'll give us a clean and predictable foundation to build everything else on top of. So simply open up your integrated terminal and run MPX create next app add latest dot which is going to create it in the current repository.

**16:17** · It'll ask you whether you want to install the next.js installer. So you can just say why yes and proceed. And I also want you to know that you don't necessarily have to follow along by using Nex.js.

**16:29** · Of course, the majority of the context for AI agents we'll be working with is going to be featured around Nex.js. But if you want to build this in Tanstack, Angular, Vue, or anything else, the concepts will still be as valuable. So let's just say Y for now. It's going to ask you whether you would like to use the defaults. So just press enter which is going to install React, TypeScript, ESLint, Tailwind CSS, and the app router. Let's give it a moment until it finishes. Once the installation finishes, we need to clear out the default boiler plate.

**17:00** · That's going to be within app and then page. NextJS ships with a lot of placeholder content that honestly we don't really need. Now, you could go ahead and clean it up manually by opening up your globals.css CSS and cleaning everything besides the Tailwind CSS directives, deleting some SVGs and other stuff within the public folder and replacing the page.tsx with a minimal component or we can use this as our first interaction with the coding agent.

**17:33** · So go ahead and open up your agent of choice. I'll just press command shift I to open up my chat sessions. And what I love about VS Code is that it's not shying away from the agnostic approach to agents. You can use their agents right here, such as Copilot CLI, or if you head over to extensions and then install an extension like Claude Code, which has like 12 million downloads, or something like Codex, which has 8 million downloads, and I installed both.

**18:07** · You can actually just navigate over to them by selecting additional views and then choosing the extension you want. Of course, alternatively, you can also just run all of these agents within the CLI by typing claude and you're in. For the longest time, I've been using Claude CLI, but the Claude VS Code extension recently got so much better. And honestly, it's working the same way as the CLI does, but with a bit of a nicer UI and the graphical interface that allows us to use it in an easier way.

**18:37** · So, that's what I'll be proceeding with.

**18:39** · I'll expand it so we have more space to work with. And you can notice that there's a little microphone button right here. So, you can either tap it or hold the command D key to speak into it. With Codex and other agents, you can either type it manually, or what you can do is use a tool like Whisper Flow, not sponsored by the way, which is what I use to write prompts when I speak with agents. Speaking is just much faster. If you install it, you can just press the command key and start speaking into it.

**19:11** · Like, clean up this Nex.js boilerplate, strip globals.css CSS down to just the Tailwind directives. Delete all SVGs in the public folder, but keep the favicon.

**19:23** · Remove page.module.css.

**19:26** · Replace page.tsx with a minimal component that just renders a center div saying ghost AI. And I can stop it right here. And you can immediately see the output. Cool stuff, right? Go ahead and write something like this. And let's see how well agent handles it. Also, just so we don't have to give it permissions every single time whenever we're doing something. For now, I will say edit manually. Oh, and of course, we have to talk about the actual models which we'll be using.

**19:54** · In this case, we're using the default model, which is Opus47 with a million token context, which is amazing, but you're going to hit the limits very soon. Instead, you'll be able to follow along this entire build with using Sonnet 46. It's fast, it's inexpensive, and it sometimes get lost unless you have the context files, which I'll teach you how to build so you guide it in a bit of a better way and make it work much more like Opus does. So, that's what I'm going to select.

**20:23** · If you're working with codecs, you can also go ahead and choose any model you'd like, like 54, 53, or anything else. Okay, let's give it a shot. It's going to think for a couple of seconds, read all the necessary files and apply all four changes. Globals, just the import page, minimal centered ghost a component, deleted five SVGs, but kept the favicon.

**20:47** · And this file that I tried to trick it with doesn't really exist, so there's nothing to delete. You can see all the changes in the diff right here. And you can also see which files have been modified on the left side. There we go.

**20:58** · just simple ghost AI and just the import for Tailwind, which means that these classes right here should work to center the div. Before we run it, let's actually head over to package.json.

**21:10** · Make sure that the project name is set to ghost AI and let's run it by running mpm rundev.

**21:18** · It'll run it on localhost 3000. So, if you open it up, you should be able to see something that looks like this. This means that our project is initialized.

**21:27** · It's cleaned up and now we are ready to move to the part that actually determines just how well everything goes. Setting up our context files and planning the build before the agent writes a single feature. So, let's do that next.

### Preparing Context

**21:45** · Not that long ago, I talked about how senior engineers spend weeks designing systems before anyone writes a line of code. They write design docs. They define boundaries and they make decisions early on so that everything else becomes predictable.

**22:02** · So let me show you how we are going to approach that. We're going to create a new folder right here in the root of our application which we're going to call context. Everything inside of it is what your coding agent will read before it does anything. This is how it knows your project and this is how it stays consistent across every session, commit or unit of the build. So you can switch multiple agents and share the context file with another developer so he can continue working with his agent from there. That's the catch.

**22:33** · We're going to have a couple of different files within the context folder. Now I don't want you to do a lot of copy pasting. So I'll provide you with the final zipped context folder so we can easily review everything together. So, delete the context folder you just created. In the video kit link down in the description, get the zipped version of the folder.

**22:54** · Unzip it and then just drag and drop it in. And here you'll see six, well, seven different files with this agents.mmd.

**23:03** · Might seem scary at first, but don't worry as I'll walk you through every single one of these files and show you how you can create them for yourself in the future. Let's start with the project overview. And let me walk you through why it's structured the way it is.

**23:18** · Because understanding this is more valuable than just copying the file.

**23:23** · Currently, we're looking at the markdown version of the file. But in VS Code, I believe this is done by default. You can also open the preview to the side by pressing command K and then V or just pressing this icon at the top. And then you can close the actual MD and just see the formatted version. I think it's a bit easier to read this way. I typically open up these project overview documents with a one paragraph summary and then a numbered list of goals. This gives the agent the big picture immediately.

**23:51** · So when a requirement gets ambiguous 3 weeks into the build, and it will, this is where you resolve it. The agent uses this constantly to understand intent when a spec isn't specific enough.

**24:08** · Notice the goals are concrete and measurable. Not build a good canvas.

**24:13** · Instead, let authenticated users create and manage architecture projects or let AI generate an initial architecture from a natural language prompt. The agent knows exactly what success looks like.

**24:27** · And yeah, this is useful for us while we are going through the process of building the app. Just so you know what we are building, just so everybody in the team, in this case me teaching you and you following along and you building it with me, are all on the same page.

**24:42** · Ghost AI is a real time collaborative system design workspace. Users describe a system in plain English and an AI agent maps that system onto a shared canvas. Collaborators refine the architecture and the app generates a technical specification document from the resulting graph. Okay, great. We have the overview, we have the goals, and then we have the core user flow. So, let me zoom this in and let's go through this together because this sequence matters.

**25:11** · The agent can sometimes lose track of how features connect to each other. By defining a full flow from signin to the spec generation, we make the logical sequence explicit. So the agent won't try to build a spec generation feature on the login page because it knows the user has to create a project and the design architecture first. In the features, we get specific about technologies. And I want to take a second on this because the tools I chose for Ghost AI weren't random.

**25:41** · I took a lot of time to choose what actually makes sense. Starting with authentication for user signin, route protection, project creation, ownership, and collaborator access, we're using clerk. Could you have gone and created the full o from scratch? I mean, sure, but it would take you a couple of days up to a couple of weeks to do it properly, even with AI. And when you do it, it's never going to be as secure as something like Clerk. And nowadays, the speed of shipping matters more than anything.

**26:14** · If you have a specific product you want to push, you want to get it in front of potential users as soon as possible. And that's why for many of these agentic builds, it's just a no-brainer to plugandplay clerk into it, especially considering just how well clerk works with your agents. You can either just copy the prompt or use clerk skills with whichever agent you're using. That way it'll immediately become a professional developer at using clerk and it'll be able to implement it within any project.

**26:45** · And there's also the MCP which is a server that allows AI agents like claude cursor or others to access clerk SDK snippets and implementation patterns and basically implement everything for you. Oh, and not to mention that clerk CLI is also being worked on. You'll just be able to ask your agent to use the Clerk CLI to add O to your app, allowing you to not even have to leave your terminal or copy and paste any API keys.

**27:12** · Clerk right now really is the leader in agentic development. And with a completely free pricing of up to 50,000 monthly recurring users, it's a no-brainer for me to build all of my applications with it. So, while we're here, I'll leave the link down in the description. you can click it and then sign up so that we can very soon more easily get started with building. Okay, on top of O the most important part of our application is the collaborative canvas and in this case I wanted to make it real time.

**27:44** · So for any kind of canvas, it makes sense to use React Flow. And if you want to make any part of your application live with cursors, so you can see what other people are doing, presence indicators, and node or edge editing. I mean, it just makes sense to use Live Blocks.

**28:01** · Livelocks is the leader for anything multiplayer. But not only apps, agents as well. Let me show you what I mean. I mean, this is the app without Live Blocks. And then if you add it, you immediately get live avatars. You can get the AI chat to generate something.

**28:19** · And you can also leave comments and track what people are doing within your app, which is super useful for the collaborative canvas we're building. But what's even cooler is interacting directly with AI assistants to do something within our application. I mean, if you try to build all of this from scratch, it would definitely take some time. But with their AI assistance feature, you can just watch an AI do it for you. Oh, and this whole React Flow thing you're seeing, that got released recently, which means that in this video, we're building the latest stuff out there.

**28:50** · Oh, and like Clerk and the many other amazing dev tools that are adapting to agentic development, LiveBlocks also offers the agent skills, which you just have to install and your agent will immediately know what it has to do to make the LiveLocks integration work. I'll teach you about all of that as we continue with the build. After the canvas, we have the starter system design, which I decided to have because it's very difficult for people to start with a blank canvas.

**29:16** · So, I want to have some kind of a curated library of pre-built system design templates where users can import a starter template into the canvas at any point during editing.

**29:28** · but also if the template doesn't do what you want it to do, we're going to allow our users to generate a system design from a prompt with AI. Then that output will be structured as canvas nodes and then we'll write it onto the canvas. And finally, we'll take a look at everything that is on the canvas and we'll convert it into a technical specification in a markdown format and then users will be able to view and download the generated specs.

**29:52** · Oh, and an additional thing that I want to teach you is while we're generating stuff with AI, that'll obviously take time as the user will likely provide a long idea of how they want to architect their app and then the AI output is going to take potentially a minute or two and running a more than 60-second AI generation call inside a Nex.js API route will just time out in production. So, that's why I'll also teach you how to use trigger dev.

**30:18** · It'll allow us to run background tasks that can run as long as they need to with the retry logic and status tracking built in. The way in which we'll combine live blocks and trigger dev is pretty amazing. So we'll have to be very clear in letting our AI agent understand that it doesn't have to invent a custom websocket implementation when liblocks is already in stack or it won't try to run AI generation inside a request handler when triggered dev is defined as the layer for that work.

**30:48** · Naming the tools we're going to use for the project in advance is crucial. Oh, and Trigger allows you to do so much more. Recently, they've been diving deeper into allowing you to build and deploy AI agents, which is something we can explore in an additional video. But in this one, we'll also focus on many of its features, specifically running background tasks and reporting back to the front end.

**31:09** · So, while a long task is happening, we can keep the user updated on what's happening behind the scenes and allow the user to continue doing whatever they're doing on the application because we're no longer blocking the front end side while handling a specific task. So I'll leave a special link pointing to trigger as well as live blocks down in the description so you can create your accounts and then we'll be able to immediately dive into the development.

**31:34** · Then we have the scope part which contains the in scope and out of scope features and it's maybe the most important section for keeping your build focused. The out of scope section is doing serious work right here. billing and subscription systems, enterprise permissions, version specification history, and so on. This is telling the agent, don't even think about them, but we can add them later on after we build the base of our application. This is great because it keeps every session focused on what we are actually building.

**32:05** · And finally, there's success criteria. Here we define what actually matters. These are the benchmarks that your agent and you can verify against after each major feature lands. Not does it look right, but can a signed in user create and open up a project? Can multiple users collaborate? Can the graph be converted into a persistent markdown specification? Very simple yet concrete.

**32:31** · So that's our project overview written in a way that makes sense to agents but also other team members working on the project. Next, let's take a look at the AI workflow rules. This file is different from others in a way that it's not about what we're building.

**32:50** · It's about how the agent behaves when building it. And the most important rule right here is to work on one feature unit or subsystem at a time. We don't want to combine unrelated system boundaries in a single implementation step. And that single rule prevents most failures that the agents cause.

**33:08** · Basically, all of these rules right here tell the agent stay in your lane. Focus on one part of what you're doing and then move on to the next one. After that, we have the code standards. So, you can open up that and let's quickly take a look. This file is what keeps the codebase consistent from our first all the way to the last chapter.

**33:28** · Without it, the agent would drift away. like specific patterns that it uses for API routes when implementing feature 5 might look different from feature 16 or maybe it's going to change some things regarding the TypeScript types or how it uses Nex.js GS how it styles things.

**33:43** · But here we add that consistency like we tell it make sure to have strict mode enabled and avoid using any or we're telling it to add use client only when the component needs browser interactivity or for styling we're telling it no raw Tailwind color classes reference the tokens through the Tailwind utility names. I think you get the point. We want to stay consistent.

**34:10** · Then we have the UI context which as you can guess dives a bit deeper into theming. Like when I was initially coming up with the design for this application, I wanted to have something that is simple yet functional and modern. And I spoke with AI a bit to generate this theme. Dark mode, no light mode. Uh all colors are already defined and we're telling the AI to use these colors.

**34:34** · And again, if you're wondering how exactly I created all six of these documents by speaking with different AI agents, that's something that I'll cover in much more detail within the specdriven agentic development course.

**34:49** · So, you can join the weight list in the description. But I think you get the idea that I didn't just sit down and handpick every color in the file. I described the aesthetic that I wanted to AI, dark, technical, precise, something that feels like an engineering tool. And then I went back and forth on the pallet um the token names and this is what it came up with. Also some font border radiuses and so on. That's exactly how you should approach your own UI. You don't need to be a designer, but you need to know the feel you're going for and then AI can help you get there.

**35:20** · Oh, and while the project overview gave some information about the project, the architecture context will give it the blueprint on how to build it. Here I specified the text stack like every technology that we want to use alongside the role that it has within the application. For O we're using clerk for user identity and route protection. For databases it's going to be prisma and posgress. For canvas it's going to be live blocks and react flow.

**35:48** · For real-time collaborative canvas for background tasks it's going to be trigger dev. And for storage we're going to use versel blobs. We also define some system boundaries like where we're going to put the request handlers. Trigger is what we're going to use for the long running background jobs and some other folders that we're going to use. Then we define the storage model where and how we're going to save something. And specifically here I decided to use a hybrid storage model which is another senior level decision.

**36:17** · We aren't going to be stuffing massive JSON blobs or three-page markdown files into our database. Instead, we're going to use Postgress only for metadata and Verscell blob for the actual files. And this keeps our database lean. And this is important. We also need to tell it how different tools are working together.

**36:38** · Since we're using clerk with liblocks, we need to set a strict rule that project memberships must be verified before a liblocks token is ever issued.

**36:48** · This ensures that our ghost AI isn't just collaborative, but secure. And finally, invariance are the rules that the system must never violate. For example, request handlers do not run longived AI works that belongs in background tasks through trigger.dev.

**37:05** · Metadata and large artifacts are stored in separate layers. O and ownership are enforced at every mutation boundary.

**37:12** · Client components only used when needed, and the canvas schema must remain consistent. Of course, we'll dive much deeper into this when we actually dive into building the application, but I wanted you to have a good idea of what it is that we're building. And finally, there's the progress tracker. This is the only file in the context folder that'll look completely different by the end of this video. Right now, it is completely empty intentionally because it reflects the actual state of the project. And right now, nothing has been built yet.

**37:44** · So, as we complete each lesson, we're going to update this file, the current phase, what's in progress, what's complete, and what's coming next.

**37:52** · And remember what I said in the beginning about agents having no memory between sessions. This file is the solution to that problem. At the start of every new session, whether that's tomorrow, next week, or 6 months from now, one prompt is all it takes to restore full context. Our agent will read the progress tracker, understand exactly where the project stands, and pick up exactly where you left off, so you don't have to reexplain yourself.

**38:18** · Even though it's going to be a small file, it does more work than any other file in the project. Oh, and finally, there's the agents.md file. Within it, we're going to wire everything together.

**38:30** · When you install Nex.js, that file was already created for you automatically at the root. This is the entry point file and every major coding agent has one. They just name it differently. Claude calls it claw.md.

**38:43** · Cursor windsurf and others use different names, but the idea is always the same.

**38:48** · It's the first thing that the agent reads at the start of every session. So, Nex.js has already added the first section for you and it tells the agent that this is a recent version and its training data might be outdated. So, read the installed documentation before writing any code. Good default and we can leave it. But now we can add our own part below it. So copy your agents MD, delete it from the context and instead move it right here. It's not long. So let's see what do we have within it.

**39:17** · We're basically instructing the agent to read all six context files in order before implementing anything. And then to update the progress tracker after each change. And you might think, isn't this going to waste context and tokens?

**39:32** · Well, I mean, sure, it has to read through the files, but that's not even onetenth of how many tokens you're going to save because there's going to be less back and forth and less mistakes and bug fixing and correcting while you're implementing the features in the first place. So, that's the system and now that you understand it, let's start building with it.

### UI Primitive Components

**39:53** · Now that the context files are ready, before we build a single feature, there's one more thing we need to set up. And skipping this one is the most common mistake I see in AI assisted projects. And that is the globals.css file. This one right here. We've defined all of our color tokens within our UI context right here. But if we don't translate those tokens into actual CSS custom properties within the globals.css CSS file. Well, it'll just write the inline colors.

**40:23** · So, instead of maybe saying something like text faint, it'll just write #505 060. And the moment you want to change it, you have to change it across all places. So, let's set it up correctly. And this is also the first real demonstration of the specd driven workflow in action. So, let's do it properly. Create a new folder inside of the context folder and call it feature specs like this. And then inside of it, create the first spec file 01 design system.

**41:00** · And then within it, we want to tell it something like read the agents file before starting. Then we need to tell it what we're doing here, like adding the design system and UI components. Then we are telling it to install and configure chat CN UI. And then we wanted to add the following components. I figured we're going to use these across the rest of the application. We never wanted to modify these files after the installation.

**41:27** · So we can specify that we can also ask it to install lucid react for icons and create a lib utils.ts ts with a reusable class names helper for merging tail class names. Although I think it would do this by default, it's good to mention it. Finally, we want to ensure that all of the components match the existing dark theme within globals.css.

**41:54** · And then we want to apply some checks when it is done. For example, we want to make sure that all components import without errors, that the CN works properly, and that no default light styling appears. This is what we call a feature specification or a feature spec.

**42:12** · Every unit we build from here on has one. The spec tells the agent exactly what to do, exactly what not to touch, and how to verify when it's done. No guessing. So let's open up our agent by pressing commandshift I. As I said, you can use anyone. I'll use claw code. I'll start a new chat. And you can even open up that file which will automatically put it within its context.

**42:36** · And then you can tell it something like read add01 design system update the progress tracker MD file to mark this as in progress and then implement exactly as specified. This is the same template we'll use often, but the only thing that's going to change is going to be the spec of the feature we're developing. So let's go ahead and run it. And notice what will happen before the agent writes a single line of code.

**43:09** · It'll read the specification and then update the progress tracker. You can see how it's going through all the files we prepared for it. And only once it has enough context, it'll write and save the plan and then execute it. And only when it has a full plan, it will update the progress tracker.md and then start doing it. So we can already take a look at the progress tracker. And I'll open it up so we can see what it is doing. And you can see that the current phase is feature01 system design.

**43:38** · The current goal to install and configure shaten with dark theme. And that is currently in progress with the feature 02 to be done. And it's also adding the architectural decisions needed for every step as well as the session notes. It's going to ask us whether want to run this command to install shaden. So I'll say yes, go ahead. And after it installs everything, it'll verify it with TypeScript. It looks like it completed with zero errors. And finally, it needs to update the progress tracker to completed.

**44:06** · So we can already open it up right here under progress tracker. And it should move it from current phase over to completed. So now at any point in our application if we come back two months later it'll know that it's using SHAT CN tailwind v4 with the following components only using dark theme and all the additional helpers as well as the architectural decisions. So once it finishes the agent will have configured chat installed the components and verified it all works.

**44:38** · So, what do you say that we test it out? Back on localhost 3000, the first good sign should be that we are now officially in dark mode. And if you head over to the homepage, that's going to be within app page. We can try to use a chaten button component coming from components UI button. And we can try to make it say something like click me. You can see it's coming from there. And it follows our UI theme. That's it. Our first feature being the theming and chassis and setup is done.

**45:09** · And that's the spectrum workflow I was telling you about. We define the specifications. We run the prompt. We verify the output.

**45:19** · And then we move on. But just before we move on to our second feature, I want to add just one little extra step to this whole workflow that's going to make our codebase even more scalable, predictable, and less errorprone. and that is whenever we implement a specific feature, let's also review it with code rabbit. There's been a report that says that AI code creates 1.7 times more problems, which means that even though we're faster, we're producing more issues per PR.

**45:47** · Also, the code becomes less readable naturally and the error handling isn't being done properly.

**45:54** · Security also suffers. So, let's add that one additional line of defense.

**45:59** · Let's review every single feature that we add to our project. In the same way that biggest teams such as the developers over at Nvidia are doing it.

**46:07** · I'll leave the link down in the description so you can create your free account and follow along. You can log in with GitHub. And once you're in, you'll be able to see that I already gave it access to many of my repos. But first, we got to push our project over to GitHub. So, head over to github.com/new and create a new repo. You can call it ghostai.

**46:30** · and just create it. Next, you can copy these commands one by one or you can just copy all of them together. Open up your agent and paste it. Then press enter. It's going to ask us whether we're going to allow it to stage all the changes. So, I'll say yeah, go ahead.

**46:46** · And they'll also allow all future commits as that's going to help us speed up the workflow as well as adding a remote. And finally, push. You can see that the changes have been pushed successfully. So if you come back and reload, you'll be able to see the current list of changes over on the repo. It's always good to make your project descriptive.

**47:04** · So you can remove the releases, deployments, and packages and add a short description such as Ghost AI is an interactive systems architecture builder. We can route to the deployed website. For now, I'll just route it to jsmastery.com. And here we can put the different topics such as Nex.js, React, Live Blocks, Clerk, Trigger Dev, and even Code Rabbit, which we'll be using for reviewing your code.

**47:35** · And I like how AI always adds nice commit messages and not random gibberish that I'm used to. But yeah, now back within Code Rabbit, you can head over to add repositories, sign in, and give it access to all your repos. And then when you're back, you can just find your project right here, which means that it's automatically being tracked.

**47:59** · So as soon as we start adding real features to the app, we'll be able to open up a PR for every new feature as we're developing within a large organization and then get it reviewed and only when Code Rabbit gives it a green light, merge it over to main.

### Layout Setup

**48:16** · Now that our colors are in and the initial chassis components are in as well, we are ready to start building the actual application and the first thing that we need is the editor including the top navbar and the left sidebar because they're the foundation of every feature we're going to build from here on. We're not yet touching off and we're not building this project creation. We just need to establish the layout so when these features come, they have somewhere to go. So inside of feature specs folder, create a new file called 02 editor.md.

**48:49** · And within it, we're going to follow a similar structure we followed before. We want to start with explaining what we need, such as the base Chrome components that frame every editor screen, the top knob bar and the left sidebar shell.

**49:04** · These will be reused and extended in every chapter that follows. Then we need to focus on what are we actually creating. That's going to be the editor navbar. So we wanted to create a new component within the editor editor navbar file. And then we want to specify some requirements that follow. We want this navbar to be of a fixed height at the top. We want it to have both left, center, and right sections, which you can see right here. On the left, we open up the sidebar. In the middle, we have the name.

**49:34** · And on the right side, we have additional actions. That's exactly what we explained right here.

**49:41** · And of course, it's going to be of a dark background with a subtle bottom border. Next, we want to explain what we want to do with the project sidebar. So, right below, we can say create a project sidebar component. It should float above the editor canvas. Opening it should not push the page content. So, you can see it remains where it is and slides in from the left. It has the header that says projects and title and a close button right here.

**50:09** · It can use the shhats and tabs component and both tabs show empty placeholder state full width new project button at the bottom with the plus icon. So something like this. Oh and finally when we click create new project we need this kind of a dialogue uh a new popup that shows.

**50:29** · So for that we can say something along the lines of dialogue pattern use the existing color tokens from globals for dialogue styling. It supports title description and footer action but don't build any dialogues yet. We just want to create the component for it. Finally to check whether it is done we can check whether new components compile without TypeScript errors, no lint errors and diagram pattern is ready for future use.

**50:57** · So hopefully you were typing this out with me or maybe you paused the screen and typed it with your own words. But this course isn't at all about typing.

**51:06** · It is about understanding what we're doing right here. So if you don't really feel like typing, nor you should. In the video kit link down in the description, I'll provide you with all the prompts that we're going to use throughout the rest of this course. So, if at any point I'm going too fast when explaining them and you just want to have it on your end and listen along, you can totally do that. But yeah, let me quickly walk you through the structure because this is the template that every spec file in this project will follow. We start with a goal, one or two sentences. What does this unit produce when it is done?

**51:38** · Then we go over some specific design decisions. Is it visual or structural or something specific to the component like layout behavior responsiveness? And this is where we can refer to that UI context file so that the agent isn't guessing the colors. Then we go over into implementation. And in this case, I decided to separate it into sections. So we have the editor navbar, the project sidebar, and the dialogue pattern. And finally, the verification checklist. So let's open up our agent.

**52:10** · Whenever you're building a new feature, always open up a new chat and don't use one of the older chats. That's because we don't want some stale context lingering around. Only remain within the same chat when what you're about to do next is related to what you've done before, such as when you want to fix specific issues. You can see that it already has access to the editor file.

**52:31** · So I'll say read this file and update the tasks on the progress tracker and then implement it exactly as specified and press enter. And in about a minute it's all done. It developed the editor navbar the sidebar and also the dialogue pattern. Type script and eslint both pass clean. Progress tracker also got updated.

**53:02** · So let's check the progress tracker first. It'll be right here within the progress tracker. So if you check feature 2 completed, editor navbar and project sidebar both implemented.

**53:16** · You can see them right here under editor editor navbar and project sidebar. We just created them so far, but they're not yet being used within the layout.

**53:25** · And even though this wasn't part of the checks, I want to actually be able to see them. I want to tell it to use the navbar and the sidebar right now within the project. So I'll open up the chat in the same context window and tell it to use these two components within a layout. And within a minute, it put it to use. It even created a placeholder page. So we can navigate over to the editor and check it out.

**53:47** · So head over to localhost 3000/editor and you can see a canvas coming soon but there is a top bar and a left sidebar which opens up the projects. So you can see that what we requested indeed got implemented. Since we're not yet at the point where we need that because we don't even yet have the editor. I actually want to show you how you can undo the changes at least right here in cloud code.

**54:13** · The only thing you have to do is press this back arrow on the message that you used to create these components and then say rewind code to here which is going to bring us back and only give us what the specification wanted and that is the components that we can then use and that compile but we're not using them quite yet. Perfect.

**54:32** · So now that we have the navbar and a toggable sidebar, let's quickly check them out. The editor navbar is pretty straightforward. And the sidebar accepts some props such as is open and on close and uses the chats and tabs to modify what's being shown. But when you're writing code yourself, you have a natural understanding of every decision you made. Heck, you wrote it. You know why a function is structured in a specific way or why you used specific props.

**55:01** · But AI generated code doesn't come with that context. The agent made decisions that were reasonable most of the time, but you didn't make them. And that means that reviewing AI output isn't optional.

**55:15** · It's the step that keeps you in control of your own codebase. So, that's the perfect use case to test out the code rabbit edition that we added in the last lesson. I'll open up the chat and tell it to push all the current changes to a new branch called development. Typically in real production databases, you often have multiple branches such as dev, staging, and only then main. So for now, we want to push this over to the development branch, get it reviewed, and only if it's good, merge it over to main.

**55:46** · So by giving it this quick message, it'll run a couple of git commands, figure out that we're currently on main, that we need to switch over and push to that new branch.

**55:56** · And that's a little pro tip. Uh, I mean, sure, you could run these commands through the terminal, but I find it super easy to just stay in flow and tell the agent to push the code for me, which you can see it just did. So, if you head back over to your repo, you'll see that the development branch had recent pushes 3 seconds ago. So, let's go ahead and compare them and open up the pull request. We have 333 new lines of code across five different files.

**56:22** · So, Code Rabbit immediately hooked itself onto the PR and we'll see whether it'll be able to pull out some bugs out of the hat. Let's give it a minute and then I'll be right back. And we got back the walkthrough where it says exactly what we introduced in this project such as two new React components for an editor UI Chrome, an editor navbar, and a project sidebar. These are super simple as this was a simple review. Later on, these are going to get much more detailed.

**56:52** · But yeah, let's check whether we have some potential issues even on a simple PR such as this one. There's one major issue that says hide the offscreen sidebar from focus order and assistive tech when closed. So specifically, this is an accessibility fix, which is definitely a good implementation. Since we haven't yet utilized this component in our app, I'll leave this so we can add it later. There's also a minor issue where the spec lists only the is open for the sidebar, but the implementation also requires on close. So actually it's suggesting to change the specification.

**57:27** · This is interesting because sometimes you're going to miss some stuff from the spec. And it's okay if AI tries to fix it or add some stuff, but it's equally as important for Code Rabbit to flag it because the whole reason why we're writing specs in the first place is so we can have predictive output. So basically you can just copy this part right here. Go back to your codebase where we're saying accepts and then it's going to be is open prop but we're going to say accepts both is open and on close props.

**57:57** · Little change I know but now our codebase is consistent with the spec.

**58:03** · And that's it for this simple PR. As we continue developing more components the reviews are going to get significantly more detailed. So for now, I'm going to go ahead and merge it, which means that we are ready to continue developing the next component.

### Authentication

**58:18** · For this type of application, we don't really need a traditional homepage. Most tools like this drop you straight into the editor. You sign in from a simple sign-in page and you manage everything from the canvas. And that's exactly what we'll do within our app. But we need O sign in, sign up, and other similar pages where you explain how your application works and then allow users to sign back in. So to get that set up, click the clerk link down in the description and sign in.

**58:49** · You can sign in with Google or GitHub. And once you're in, you can head over to applications and create a new app on the dashboard.

**58:58** · You can give it a name such as ghost AI and choose the sign-in options such as email, Google and since this is a development website, we can also do GitHub. Then click create application.

**59:11** · We are building on Nex.js. So what you can do is just install add clerk/nextgs by copying this command and paste it straight into the terminal. And while that is being installed, you can also set up your clerk API keys by copying them from here and creating a new file called env.local and then paste them right here.

**59:34** · Now, before we hand anything over to the agent, there are two things you need to know about clerk and nex.js16 specifically because if you skip this, the agent will get it wrong. And it says it right here. If you're using Nex.js JS15 or lower, name your file middleware.ts instead of proxy.ts.

**59:56** · The code itself remains the same. Only the file name changes. But because most agents were trained on NexJS 14 and 15 code bases, it'll almost certainly create a middleware.ts file by default.

**1:00:09** · So we'll have to specify proxy.ts explicitly in our spec so it doesn't have to guess. Oh, and another important thing is that just by adding middleware, it doesn't automatically protect all routes. As you can see right here, by default, it leaves all the routes public. And this catches a lot of developers. You have to explicitly define which routes are protected and which are public, which means that we have to configure everything intentionally. And this is exactly why reading the updated documentation before building with AI matters.

**1:00:38** · The agent knows Clerk, not necessarily the version of Clerk you just installed or the version of Nex.js you're running on. The spec bridges that gap. Oh, but we can also use agent skills. As I told you at the start, most major frameworks and libraries now publish official skill packages specifically for this problem.

**1:00:59** · It gives your agent up-to-date knowledge, current APIs and patterns, and the best practices of the library you're using. So, if you search on Google or within the docs clerk agent skills, you'll be redirected to this page. Then, simply copy the installation command. Head back over to your codebase and paste it in your terminal. MPX skills add clerk skills. Press enter.

**1:01:24** · You might need to install the skills package by saying Y and then enter. And then by pressing the arrow up and down keys and the space key, you can select specific packages such as core clerk, you can either select some additional clerk features or some additional clerk frameworks like in this case I'm going to go with clerk next.js patterns and press enter. Then you can select additional agents that you want to add it to. By default, it's going to work on codeex cursor anti-gravity.

**1:01:53** · But if you want to add clot code, you have to select it here and press enter. And we can install it in project scope via sim link. That's the recommended way. So just proceed with installation. Perfect.

**1:02:08** · Our skill is installed and we'll be able to invoke it later on once we focus on implementing the odd functionality.

**1:02:15** · So now we are ready to write the spec.

**1:02:19** · Open up your context feature specs and create a new file called 03 o.md.

**1:02:26** · And once again, the full feature specs files are linked in the description in case you want to just copy them and then follow along or you can slowly type it out with me. Let's start by telling it that clerk is already installed and connected. So we just need to wire it into the next.js GS app provider o pages redirects route protections and the user menu. When it comes to the design, we just want to use the clerk's dark theme from the add clerk UI themes as the base.

**1:02:57** · And then we want to override the clerk appearance variables using the app's existing CSS variables with no hard-coded colors for the sign up and signin pages. This is what we want to develop on large screens. We just want to have a simple two panel layout. On the left side, a logo, a tagline, and texton features. On the right side, a centered clerk form. And on small screens, forms only.

**1:03:25** · We don't want to have any kind of gradients as that's going to seem AI-ish. No oversized hero sections, cards, or scrollheavy layouts. Keep the layout minimal and professional. And then we can dive into a bit more details on the full implementation.

**1:03:44** · So we can say wrap the root layout with the clerk provider using the clerk's dark theme. Create sign in and sign up pages using clerk components. And as I told you before, we have to be specific and telling it that it should use the proxy.ts file name at the project route instead of the middleware.ts.

**1:04:06** · And then we have to define public routes using the existing sign in and sign up environment variables protect everything else by default which means that we have to update our homepage so that when authenticated users visit it we redirect them to the editor or when unauthenticated users visit it we redirect them to the sign-in page. We also want to implement Clerk's built-in user button to the editor navbar right section for profile settings and logout.

**1:04:38** · We want to keep clerk's default user menu and profile flows intact and not rebuild heavily customized clerk internals and want to use existing clerk environment variables without renaming or inventing new ones. Finally, we can specify additional dependencies such as clerk UI if we need to install it. And then when it's done, we want to check that proxy file is there, that all routes are protected except public off routes. All pages use CSS variables with no hard-coded colors.

**1:05:09** · Clerk provider wraps the layout and the build passes.

**1:05:15** · This is our complete authentication implementation. Now you know the drill.

**1:05:20** · Go ahead and open up your agent. Give it access to this file and tell it to read this file and update the progress tracker.md file accordingly. Then implement the o feature exactly as specified in the o.md file. Okay, you can see that the built-in microphone feature right here still isn't perfect.

**1:05:42** · Let me try to do the same thing with whisper flow specified in o.md file.

**1:05:50** · There we go. That's a bit better. And specifically, it's 03.

**1:05:54** · MD. Perfect. Let's go ahead and run it.

**1:05:58** · First, it's asking me to run some bash commands to check whether clerk has been properly installed. And we'll say, yeah, go ahead. You can run it. It took him about 2 minutes or so to go through all the context we shared. And only then it'll start to implement everything in parallel. And this is much better than if it started right away and then just ended up with a bunch of mistakes. So the list of updates that it put right here is to update the env.local with clerk signin and signup URL varss.

**1:06:29** · Create a proxy with clerk middleware route protection. Update the app layout with the clerk provider and dark theme.

**1:06:36** · Create signin and signup pages with a two panel layout. Update the app page to redirect based on the off state. add the user button to editor navbar and create editor page and then update the progress tracker and run mpm run build to verify.

**1:06:52** · It's going to ask me whether it has the ability to create some directories and I'll tell it, yeah, go ahead. And in the future, we can give it some more permissions so it can do things a bit more freely. And after it came up with the initial plan, it actually built out everything pretty quickly, maybe even in less time than it used to think how to approach it in the first place, which shows you just how important the initial context and a proper task are. And there we go. The build passes. And here's the summary of everything that was implemented.

**1:07:23** · I think all of these things right here shouldn't come as a surprise because we initially specified them in this spec. Then it updated the to-dos and now it just did it. And yeah, it's pretty interesting that it even notes right here that it would have gotten confused about this middleware proxy thing if we didn't specify it properly.

**1:07:44** · But thankfully, it did it in the right way thanks to the research that we've done at the start. So, what do you say that we take it for a spin? The application is running on localhost 3000, but whenever I make some bigger changes, I like to rerun it. But initially, if you head over to localhost, you might get redirected to this clerk handshake part, which is going to lead to a broken page. But after you reload, it should properly redirect you back to the homepage. And after that, it should just work.

**1:08:11** · This is something that we can polish and fix up later on. But yeah, this is looking interesting. Definitely not quite as nice as the original application that I've showed you that's deployed. So, what are some of the things that we can do to make it look more similar to that one? Well, step one is to search some kind of design websites online like Dribble or award-winning websites and then just take a screenshot and try to get it to match to that closer.

**1:08:41** · Or in this case, you can head over to the deployed version of this application, take a screenshot of this whole UI that you can see right here, and then we can feed it over into our chat. So, go ahead and open up the chat. Keep in mind that we can still stay within the authentication window that we worked on because now we're fixing some parts about that specific implementation. So, what you can do is just click this plus right here and upload from computer or just drag and drop the screenshot. then select it.

**1:09:13** · And then we can further point out to some things that could be improved, not just the layout. It seems like it didn't properly read the fonts that the right side of the screen is taking a larger portion. So maybe we can split them 50/50, same as it is right here, and make the font size a bit larger. So it's not just the layout.

**1:09:31** · We needed to review the screenshot and update the UI of our current application to look more like the one on the screenshot. means 50/50 left and right side layout with some kind of a color on the left side to differentiate it from a dark background as well as we need to fix the fonts so that it uses the ones outlined in our UI guidelines. I think for now this is going to be enough for it to get closer to the design we want to get. So press enter and let's see how it handles it. And there we go.

**1:10:02** · The build passes. It updated the globals from circular font reference to the one that should be correct right now. The body was pointing at itself. So, this font was never actually applied to anything. Same fix for the heading. And it also implemented some other fixes.

**1:10:20** · Let's check it out. The design now looks much closer to the finished product. The fonts are being properly applied and that makes a big difference. So does the increase in font size and this shift between the two different background colors. Of course, later on we can come up with a unique logo that we can put right here. But for now, this is looking great. And believe it or not, we have a fully functional authentication system built in right here. So, what do you say that we go ahead and test it out?

**1:10:48** · You can head over to signup to see whether that works. And it does. Later on, if you want to, you can modify the contents on the left side depending on whether you're in sign in or sign up page. And then let's use something like GitHub to sign in. I'll authorize it. And the redirect redirects us to a page that currently breaks. So I'll try to head back over to localhost 3000 one more time. And now when we get back, it actually redirects to the editor properly.

**1:11:18** · You can see that we have the sidebar. We have a space for the canvas that's about to come in the future. And then on top right, we see all the information about our currently logged in account, which is beautiful. I mean, we get complete user management within a single prompt that we've done. Let's also try to sign out for now. And we do get one issue when we click that button saying there's an unexpected response received from the server. So, if we head back over here and open up the terminal, we can see an unhandled rejection.

**1:11:50** · Unexpected response was received from the server. And then in the terminal, we see something like this, which doesn't really tell us much. Now, what we could do is just copy this, open up the chat window one more time by heading over here, and then just pasting this error and telling it to fix it. But I'm actually glad that this error happened because I can teach you a bit better and more precise way to handle these issues and so that when you try to fix them, you don't cause new ones.

**1:12:17** · So instead of pasting this right into the chat, we're actually going to open up a new file right here within context and call it current issues.md.

**1:12:31** · You can even do it within feature specs.

**1:12:33** · Either way works. Then you can paste any kind of errors that you have and explain what's happening. So I'll explain that when I click the log out button the following error appears and now I can paste this error message and we can also specify that sometimes when we log in we get redirected to this weird long URL which doesn't show anything on the page and then we can just paste this URL right here.

**1:13:03** · Again, the errors on your end might be a bit different from what I'm seeing right here. Whatever they are, I don't want to teach you how to copy and paste. I want to teach you how to solve the problems for yourself.

**1:13:16** · Explore the current issues file and deeply analyze the problem. Only when you have the analysis, give it back to me with the idea of how you're planning to solve it and then wait for me to give it the green light to execute it. So yeah, writing something like this makes sense because that way it doesn't go into the spiral of trying to fix its own bugs while breaking 10 other things. You provided the error. It's going to come back with the analysis. You're the one deciding whether that analysis makes sense and whether it can actually execute it.

**1:13:47** · So let's run it and see what it comes back with. And after some thinking, it's back with the analysis.

**1:13:55** · And this is so much better and so much more detailed than if we just told it to fix it immediately. Now it actually tried it out and has a deep idea of what's happening. The server log is the key clue. Proxy took 373 milliseconds out of a half a second total request.

**1:14:13** · Almost all time is spent in the proxy.

**1:14:16** · So that already points it in the right direction. As a human person, I would never figure this out on my own. at least not from such a vague error message. But yeah, here it figures out that this button needs an after sign out URL. So it's just going to add it. And a similar thing is happening with the handshake URL. It basically needs to configure that after signup URL and that way it's going to route it properly. So it provided a twoix plan. So this looks plausible to me. Looks good.

**1:14:46** · So let's just tell it to execute the plan and fix the issues. There we go. So, the fix now seems very apparent. We just needed this after sign out URL. And if you want to learn more tips and tricks just like this one about actually analyzing and fixing the errors and how I approach building these production level applications, definitely check out the specdriven agentic development course.

**1:15:11** · It's not out yet as it's going to be super detailed and it's going to follow the best practices from the strongest developer teams out there. But yeah, it'll be out soon. But I'm still super glad that while I'm developing that, you can still learn how I develop these applications with the agentic ways with this new video that you're watching right now. And you can let me know down in the comments how you like this new type of video.

**1:15:34** · I get that it's completely different from manual coding, but I still think there's so much to learn and we can have a predictable development workflow even with AI doing the writing for us. So let's see whether this actually fixes it. And the build passes. The after sign out URL prop was removed from the user button as it belongs in clerk options and is set via environment variables. So we'll soon be able to verify whether that actually fixes it.

**1:16:02** · But before I want to open up my terminal, stop it from running and then rerun it again on localhost 3000 because we changed the env. So we want to make sure that they're read by the browser. So now heading back over to localhost 3000. Maybe you're signed in already, which is fine. You can simply sign out now. And that brings us to another error, which is the same one we've had before. And another thing you can do is head over to inspect element, switch over to the application tab, and then clear all the cookies.

**1:16:31** · So find the cookies for localhost 3000, clear them, and then reload the page. You'll be redirected back to the homepage. And now we can retry with a clean slate. So, I'll sign in using GitHub the same way I did before. That works. I automatically got redirected over to the editor, which is great. And now I'll sign out. And that worked. So now head back over within your terminal. Run git add dot git commit-m implement o and then get push.

**1:17:03** · This is going to push all the changes to origin development allowing us to open up a pull request over to the main branch. Then you can open up a PR and let's wait for Code Rabbit to review it. This time we had many changes but not many of them are directly related to what we did in the code. We just added these agent skills so that everybody else's agents working on this codebase also well become smart in the technologies that we're using for the project.

**1:17:32** · And then yeah of course we implemented a couple of different files that Code Rabbit will verify. But primarily what we've done is right here within app signin and signup pages we have added some features that would display on the left side and then the sign-in page where on the right side we just render the signin component coming from clerk. Similar thing happens over to the signup page. So right here we're just rendering the signup UI.

**1:18:01** · Then over in the layout, we are wrapping everything with a clerk provider, setting the theme to dark, and setting some custom variables. That's it.

**1:18:14** · Everything else remains the same. And then within the editor page, we're simply showing the navbar and the sidebar as well as the rest of the content. In the navbar, we display the clerk user button, allowing us to see more info about the user and allowing us to log us out. Pretty straightforward so far. As our components and features get more detailed, we're going to do deeper dives into the codebase. But so far so good. Let's wait for the review. And quickly, we're back with a full walkthrough.

**1:18:43** · This pull request integrates clerk o into a nextjs application and establishes comprehensive agent skills for clerk integration across multiple frameworks.

**1:18:54** · It also adds O middleware, signin and signup pages, clerk provider setup, and introduces five new skill definitions for supporting scripts, documentation, and so on. So, obviously, a lot of the checks right here from Code Rabbit are going to be about the skills that we set up, but we can skip those for now and focus on the ones about the actual files we implemented. In this case, it looks like there's one critical issue, and that is within the context current issues.md.

**1:19:24** · Well, you never want to publish current issues to GitHub anyways because you want people to see your code and not your mistakes. Um, what we're doing here is even worse. We're exposing the handshake or the JWT token from the track docs. So, this is a real security issue. So, what we need to do is delete this file. Obviously, this won't delete it from the git history, but that's fine for us because this JWT is no longer in use.

**1:19:52** · So, right here over to get ignore, I'm going to add our forward slashcontext forward slash and that's going to be the current issues.mmd file. And I'll also remove everything that is within it. Not that it matters right now because we're adding it to get ignore anyway. So let's go ahead and push those changes by saying get add dot getit commit update.getit ignore and get push.

**1:20:20** · Immediately the changes will be recognized which means that we can merge this over to the main branch.

**1:20:27** · And while we're here we can also head over into context on the main branch and remove the current issues file right here from GitHub by simply deleting the file and committing the changes. We can also do the same thing on the development branch by heading over to context and heading over to current issues and just removing the file so that it's no longer here and it's not going to be pushed to GitHub any longer because we added it to get ignore.

**1:20:56** · Perfect. With that in mind, we've successfully implemented the full UI and functionality for the authentication within our application.

### Project Dialogues

**1:21:07** · Now that our authentication is done and we can actually sign into our application, let's make the sidebar actually do something. As right now it is just static. Before we hook up any real data, we need the UI in place. The create, rename, and delete dialogues plus the editor home state. So we're keeping this prompt focused on UI only with no API calls yet. Head over into context feature specs and add a new file called 04 project dialogues.

**1:21:37** · Within it, we can specify that the goal is to build the editor home screen and add the project dialogues and sidebar actions with no API calls yet. So, what does this specifically mean? Well, it means that on the homepage, we want to reuse the existing editor layout without modifying the navbar or sidebar behavior, but in the center of the page, we want to add a heading, create a project or open up an existing one, and a description.

**1:22:07** · Start a new architecture workspace or choose a project from the sidebar and a new project button with a plus icon. keeping the layout minimal without wrapping this content in cards.

**1:22:19** · And then clicking new project should open up the create project dialogue. Let me actually show you what I mean by all of this by heading over to the finished version of the application and quickly signing in. Notice how right here in the middle we have some text greeting us even though the canvas is empty allowing us to create a new project which then opens up this dialogue. That's exactly what we want to achieve. So, we'll have a dialogue for creating a new project as well as for editing one and deleting it.

**1:22:50** · So, let's specify these three dialogues below. We're going to have one for creating a project that takes in the project name input, the live slug preview based on the name, and preview updates as the user types. Then, the one for the rename with prefilled project name input, and the one for delete.

**1:23:09** · Finally, on the sidebar, we want to add the following project item actions.

**1:23:14** · Rename and delete. Show actions only for the projects that we own and hide actions for the shared or projects belonging to collaborators. And on mobile, tapping outside the sidebar closes it. And want to add some kind of a backdrop scrim. Finally, let's specify the implementation right here by telling it to create a dedicated hook to manage the dialogue state, the form state and the loading state. That way, we can reuse the functionality.

**1:23:40** · And then we want to wire the editor home new project to create dialogue, the sidebar create button to create dialogue as well, sidebar rename to rename dialogue, and sidebar delete to delete dialogue. For now, we only want to use mock project data with no API calls. And to check when it is done, we need to check that sidebar actions are wired, that slug preview works, that no TypeScript errors exist, and there's also no linting errors.

**1:24:10** · So, let's open up Claude code or your AI agent of choice. And then we can tell it to read this file, update the progress tracker.md to mark this as in progress, and then implement it exactly as specified. And let's run it. And in about a minute or so, feature 4 is done.

**1:24:33** · Here's what's built. New file hooks use project dialogues which centralizes the dialogue type form including the name and the slug the loading state and mock data which exposes these different functions to deal with the dialogues.

**1:24:48** · Then there's the dialogue component as well as within the project sidebar we also call the dialogues when needed. So let's quickly check this hooks file that it implemented. You can see that it is strictly typed right here with the project interface. the dialogue type to slug which takes in the name and turns it into a human readable ID and it even created some mock 3 projects that we can verify.

**1:25:12** · It came up with a lot of different use states uh keeping track of all the projects, the dialogue type, the selected project, the name, slug and loading and all of these are going to be used within the dialogues themselves.

**1:25:27** · Then it returns the data so we can actually use them. Let's check where the dialogue is being used. Most often it is right here within project dialogues where we have the actual code for how the dialogue looks like. If the dialogue is of a type create, then we show this one. If it's of a type of rename, we show this one. And if it's delete, we show the one below. Before we test it out, let's check out the progress tracker that says that the current phase is the feature 4 dialogues.

**1:25:55** · It has the goal to do it. And it has actually completed the project dialogues with all of these different components.

**1:26:02** · So now, if you come back to the editor, this is going to look much better. It's no longer just a blank screen, but rather in the middle it says create a project or open up an existing one.

**1:26:12** · start a new architecture workspace or choose a project from the sidebar. And if you click create project, it actually opens up a new project dialogue where you can type something like my project.

**1:26:26** · It automatically creates a slug at the bottom as well. And if you click create, you saw that creating loading. And of course, the data is currently static, but you can see how it's going to look once it actually picks the data from the database. So we have ghost AI core which you can select to edit its name as well as to delete it. This means that the UI for all of the dialogue functionalities has now been implemented alongside this centerpiece of the application.

**1:26:55** · Which means that now that the majority of the UI is done in the next lesson we can start focusing on implementing real data with a real database to make our app come to life. But before we dive into the database, let's make sure that our current code is good. And I want to show you another Code Rabbit feature allowing you to review your code directly within your VS Code, which means that you don't even have to create a PR and you can be that much faster. You can install the Code Rabbit extension, authenticate to your account.

**1:27:26** · It'll notice the changes that you have right now. So you can just click review all changes and the review will start directly within your editor.

**1:27:37** · So, let's give it a minute. We'll check the changes and if they're good, push them. If not, we're going to fix them.

**1:27:43** · And within a minute, the review is in and Code Rabbit left the comments directly on our codebase. So, you can expand all the files and click on them to see exactly what's happening. For example, right here, specify confirmation message and project name display. The delete project dialogue lacks key detail. What text should be shown to the user? Should the dialogue show which project is being deleted? And should we show the cancel button as well? These are some important questions.

**1:28:11** · And it's good because in this case, Code Rabbit is telling us that we can be even more precise with our feature specifications. But let's see if it has any comments within our codebase.

**1:28:21** · It says right here that the project item, that is this one right here, appears clickable, but it lacks interaction handling. It has a cursor pointer. That is this one right here in the sidebar. But when I click on it, it doesn't do anything. That's fine for now because later on we're going to make it open the actual canvas of that project.

**1:28:40** · Since that is not implemented yet, that's totally fine. Then another inconsistency. Feature 4 is being marked as both in the current phase as well as finished right here at the bottom. So we need to modify the progress tracker to say that the feature five is to be done and then and then modify the current goal to be determined for feature 5.

**1:29:01** · Next up feature five. This is good. And finally in the use project dialogue hooks we have a couple of comments as well. First we have missing validation for empty slug edge case. If the user enters a name containing only special characters, it passes the truthy check but returns an empty string resulting in a project with an empty slug. So if I head back right here and try to create something, take a look. It's true.

**1:29:26** · I can actually create a new project, but nothing gets added to the slug because these are not valid slug characters. So we definitely have to fix this.

**1:29:38** · Thankfully, what we need to do is add slug validation. So I'll just press accept right here and it'll update the code for me. That's another perk of using code rabbit within VS Code. And I think there is one other comment right here in this dialogue which is the same issue right here. Same as before, the rename operation has the edge case where the slug could end up empty. So we definitely want to fix the validation there as well.

**1:30:03** · Now we can push the changes by saying get add dot git commit-m implement dialogues and then get pull to pull the latest changes and then run git push-force to push the latest changes because remember we deleted that file directly on GitHub but still we want to push the local changes as well.

**1:30:26** · So now if you want to you can manually open up a PR by heading over to new pull request from the development branch over to the main branch and we can immediately merge it because we've already reviewed all the changes with code rabbit with their VS code extension. So back within the application you can run gitpool and you can also check out to main and run gitpool there as well to be up to date.

**1:30:53** · But make sure to switch back to the development branch because that is where we're actively developing new features.

### Prisma Setup

**1:31:02** · Now that our project management UI is wired up, we need the actual database behind it. And for that we're going to use Prisma with Postgress. If you prefer a different database, the process is the same. Just swap the provider in the schema. Prisma supports Postgress, MySQL, SQLite, and more. So let's start with a manual installation right here within the terminal. Stop the app from running and then run mpm install prisma tsx at types/pg-save-dev.

**1:31:34** · These are the dev dependencies so we have a nice development workflow. After that is done, you can install all the necessary packages needed for us to set up our database such as add prisma/client prisma adapter pgenv and pg itself and press enter. After that is done, initialize prisma with the correct output path for the nextgs router. You can do that by running mpx prisma init-out/app generated prisma.

**1:32:04** · This creates a new Prisma folder with the schema.prisma file and an env file at the root. So head over to the Prisma dashboard. I'll leave the link down in the description and create a new account. You can sign in with GitHub or Google. And once you're in, you can create a new project.

**1:32:25** · I'll call it Ghost AI. And they'll give you a one command setup. But in this case, we can proceed with the connection string. So you can just copy it and then head over into yourv and override the current database URL with the new one that you just got from the dashboard. As a matter of fact, we can take this database URL and put it within thev local as that's what we're using for our environment variables. Then open up your prisma.config.ts and update the path to the schema. It's just going to be prisma slash.

**1:32:55** · We want to remove this schema.prisma Prisma because we'll make a separate Prisma model. So just use Prisma forward slash.

**1:33:05** · Now before we run our spec, let's also install Prisma agent skill. We did the same thing with Clerk. So the same idea applies just for a different library.

**1:33:16** · Open up your terminal and run MPX skills add Prisma skills.

**1:33:22** · It'll ask you which ones you specifically want to install. And in this case, you can select all of them.

**1:33:28** · CLI client API database setup Postgress Postgress setup and upgrade v7 and press enter. You can install them for cloud code within this project with sim link and we can proceed with installation.

**1:33:42** · And now we are ready to generate our schemas. So let's create a new file right here within our context feature specs05-prisma.md.

**1:33:54** · and one sentence update is that Prisma is already installed but we needed to add the project data models Prisma client singleton and the first migration. So then we have to start specifying the models that we want to install that we want to set up. First we're going to have the project model.

**1:34:11** · So we'll ask it to add project that has to have an owner ID mapped to the clerk user a name an optional description a status enum either draft or archived a canvas JSON path for future canvas blob storage timestamps and indexes on owner ID and creation date so we can actually search through them. The second model we want to have is going to be the project collaborator which is a project relation with cascading delete.

**1:34:44** · It includes collaborator email timestamp and some constraints on the project and email and indexes so we can actually map over it.

**1:34:55** · Do not add any extra fields unless required by Prisma. Finally, to be able to use these models, we have to set up Prisma client. So create a lib prisma.ts ts file as a cached singleton branch by database URL. If it starts with prisma plus posgress then use accelerate else direct to add prisma adapter pg. In our case, it's going to start with posgress slash which means that it is actually hosted somewhere.

**1:35:23** · Finally, we want to ask it to run the migrations and generate that Prisma client. And we want to verify whether it has installed all the dependencies such as Prisma, Prisma client, Prisma adapter PG and PG itself.

**1:35:38** · And some checks are whether schema has both models with correct relations and indexes. The lib Prisma file exports one cache Prisma instance. The migration runs successfully and the mpm run build passes. So let's open up cloud code, give it this file, and tell it to read this file, update the progress tracker, and implement it exactly as specified. I think you get the idea with these prompts. The actual spec file is doing the heavy lifting. So let's see how it approaches it.

**1:36:10** · It'll first read the Prisma spec, the progress tracker, the architecture context, and only then will it start implementing it. It'll first verify we have all the necessary packages and it might even consult the Prisma skill so the agent does a better way implementing the best practices. So let's give it some time and I'll be right back. Now it's in the process of creating the Prisma models for the project and the project collaborator then creating the Prisma singleton so we can actually have the client and run it.

**1:36:43** · It's asking us whether we can actually run Prisma migrate. So I'll allow it to run it.

**1:36:49** · and then it'll verify everything is done and we'll be able to check it all out.

**1:36:54** · You can see that we have many files changed but once again the majority of these are coming from the agents that we installed or the agent skills. The actual generated files that we care about are going to be within just a couple of files such as this Prisma model right here and this Prisma client.

**1:37:12** · That's it. But okay, let's let it do its thing and the feature 5 is done. Here's what's created. just two files that we need to take a look at. The first one is the project model and the second one is the Prisma client. So let's go ahead and check them out. I'll first open up the model that is going to be within models project.prisma. And it looks like I'm missing the Prisma syntax highlighting.

**1:37:38** · So I'll head over into extensions and install Prisma, which should add the syntax highlighting, formatting, autocomp completion, and more. There we go. This now looks better. But yeah, essentially we have created a new model for the project with the ID, owner ID, name, description, status, the canvas which is going to be attached to a project very soon and a potential list of collaborators. And we also made it indexable so we can search for these projects. Same thing happens with the project collaborator.

**1:38:07** · That's going to be a clerk ID connected to it and it's going to have access to one or more projects.

**1:38:15** · Then if we take a look at the actual Prisma client that's going to be within lib Prisma, we're just using the Prisma.

**1:38:23** · PG adapter to create a new Prisma client and connect it to it. Then we export this global Prisma instance that we can use to make any kind of database calls.

**1:38:35** · We can't really test a lot of stuff right here because we've just built a database. But in the next lesson, we can build a couple of API routes that'll bring us one step closer to actually making use of this data. So for time being, let's just run git add dot getit commit-m implement prisma and then get push.

### Project CRUD APIs

**1:39:00** · Now that our schema is ready, we're ready to build the API routes that sit on top of it. This is backend only.

**1:39:08** · We're not yet wiring the UI. That'll come next. But right now, we need to focus on one single thing. A clean, secure set of routes for creating, listing, renaming, and deleting projects. So, create a new spec right here under context feature specs 06 project APIs.md.

**1:39:33** · And within it, we want to tell it that the database schema is ready. So we need to build the backend project API routes.

**1:39:41** · The routes are as follows. The rest endpoints for get API project which is going to list the current users projects. The post for API projects which creates a project. We have the patch for renaming and delete for obviously deleting.

**1:39:57** · We can also give it a couple of rules such as use the authenticated clerk user ID as an owner ID and when creating default missing project to untitled project and use the schema's existing ID strategy without adding sequential IDs. We also want to tighten up the security a bit by telling it that the unauthenticated requests return 401 and only the project owner can rename or delete. Non-owners mutations return 40 or three.

**1:40:28** · Which means that we're making our app secure not only on the client side, but the server side API calls are also going to return invalid responses if somebody tries to break them. And again, we're not yet wiring any UI. And finally to verify we need to check whether the routes exist, whether the owner checks are enforced, whether 401 and 403 responses are handled correctly, and that the mpm rundev build passes. You know the drill. Open up cloud code, tell it to read the file and execute.

**1:41:03** · Read this file, update the progress tracker, and implement it exactly as specified. Let's see how it does.

**1:41:10** · The process of actually creating four REST API routes would take us some time and you most likely already know how to do that. But our agent is just going to do it much more quickly for us. And then when you take a look at it, you can fully understand the structure and you'll be able to add any other additional routes very easily because it's mostly boilerplate. So let's give it some time and I'll be right back.

**1:41:32** · There we go. That was quick. Four routes have been created and the build is clean. All of them are right here within project routes or project project ID route. So these are the general ones and these are the ones for update and delete. Let's go ahead and check them out. They are right here under app API route.ts for general project routes where we have a asynchronous get function where we first get the user ID from O belonging to clerk.

**1:42:06** · We check whether the user ID doesn't exist. In that case, we return a 401.

**1:42:11** · But if it does exist, we try to find all the projects that match with that user and then we return them. Similarly, if the user is trying to create a post, we get all the data from request.json, we take the name and finally create it.

**1:42:27** · Then if we want to update or delete them, you can head over to the project ID route where we can patch it based on the project ID. So we first check whether the user has access. If they do, we take a look at the context params, find the project, parse the data, update the project data, and then return it.

**1:42:48** · And the same thing goes with the delete.

**1:42:50** · It's going to be even simpler. We find it, we delete it, and we call it a day.

**1:42:55** · It's even returning a proper 204 status which means deleted. But now in the same lesson, I want to actually create an additional feature spec which is going to be 07 wire editor home.md where we want to wire the editor home sidebar and dialogues to the real project APIs we just created. So first we got to deal with data fetching because the editor homepage is a server component.

**1:43:25** · So we need to fetch owned and shared projects server side using the existing project data helper and pass both lists to the sidebar and I don't want to see any client side fetching for the initial load. Now we can do that by using the project actions. So I want to create a new hook in the hooks folder that manages dialogue state and project mutation. That's going to look something like this. Create manage create dialogue state manage project name input.

**1:43:58** · Generate a short unique suffix slugify the name. Call the post API projects and then navigate over to the new workspace.

**1:44:07** · The project ID and livelocks room ID should stay aligned. And we can do a similar thing for rename and delete. The rename simply has to store the target project ID plus current name and then patch the name and delete has to store the target project ID and then patch it.

**1:44:25** · Finally, we are ready to wire it all together by connecting the hook to the sidebar and dialogues. Create dialogue will show a room ID preview. Rename dialogue will prefill the current name and delete dialogue will show the project name. As usual, we want to run some checks when we are done and that is to see whether the sidebar uses real

**1:44:46** · project data, not the fake dummy data uses right now, whether the create actually navigates to the workspace, whether the rename updates correctly, and whether delete refreshes or redirects correctly. Finally, the build has to pass. So this is the moment that our sidebar goes from mock data to real data. So let's open up our agent, tell it to read the file, update the progress tracker, and implement it exactly as specified.

**1:45:15** · So let's let it do its thing and once it's done, we can test it out in the browser. And after some time, we are back. The build passes clean, and it created a couple of new files. The lib projects is used for fetching the own projects and shared projects. We can quickly check that out right here under lib projects.

**1:45:34** · And you can see that this file simply exports one function called get projects for user which calls all the projects where the owner ID is the user ID that is currently signed in and then it returns all the owned and shared projects. It also created a hook that deals with all the project actions and modified some additional files such as the editor, the project's route, and some more types and props updates over the sidebar and the dialogues.

**1:46:06** · So, don't forget to rerun your application by running mpm rundev.

**1:46:10** · And then back on localhost 3000, we are ready to test it out by creating a new project. I'll give it a name such as my system design.

**1:46:22** · And you can see that it's going to give it an additional slug right here. And we can click create project. It's creating it. And we get redirected to editor my system design. So the redirect is actually working, but there's no route under that page. But that's to be expected because so far we just wanted to test whether we can wire the database functions with the API routes. So, if I head back over to the editor and then open up the sidebar, you'll see that there's a new my system design project.

**1:46:53** · And you can also rename it to something like ghost AI system architecture. And you can see that it updates it in real time or you can also just delete it.

**1:47:04** · Let's test it out. Yep, that works. And it updates in real time. So this means that we have not only implemented the dialogues to create all of this but also implemented the API routes that handle the functionality. And if you're wondering why we didn't do all of this in a single prompt, well the API routes touch the backend layer and the UI wiring touches the front end and server components. Combining them gives the agent too much surface area to make assumptions across.

**1:47:34** · Instead, we had two focused prompts, which means that we got back two clean results without messing up stuff on front end and the back end.

**1:47:44** · So, before we go ahead and review these changes, head over to GitHub and merge the previous PR which contained implementing Prisma and even more importantly adding all of those additional files for agent skills. So, I'll just go ahead and merge it. So, now when we push this over to GitHub, we'll be able to review just those changes. So run git add dot git commit-m wire up prisma ui and rest apis and run git push.

**1:48:14** · You can head over to your repo, open up a new pull request and do it specifically from the development branch. This one will be fairly quick as there's only 11 files changed. So let's give the doctor code rabbit some time to review it. In this PR, we've finally introduced the REST APIs and CRUD functionalities, making our app well full stack. We've done that across all the different files.

**1:48:37** · And I always like when Code Rabbit thinks the functionality is so detailed that it actually gives us a diagram that we can review. So, as the user clicks the new project, the actions.open create dialogue runs. Then we initialize the dialogue and generate the room ID with the suffix. We ask the user to enter the project name and submit.

**1:49:00** · After they submit, we set the loading and we then make a post request to our API projects which is our CRUD rest API route which then calls Prisma project create. As soon as the project is created in the database, we return the project data, set the loading to false, and bring it back and navigate over to the new project. It looks like we have one issue where we need to import the use project actions as a value and not as a type.

**1:49:27** · So return type off requires the hook in a value space but import type is a typeon import that TypeScript erases from the value name space. So what we can do is just copy this import right here. Find where we're already importing a type specifically the use project actions.

**1:49:49** · That's going to be right here. And instead of it, we can just import the use project actions without the type at the start.

**1:49:57** · That way, when it's referred right here, we can say type off use project actions, which is a function that TypeScript can now actually understand. This is a pretty nice save. And there's another issue in the use project actions where we need to handle the failed mutations before closing or redirecting. So rename and delete always close the dialogue and refresh push even if the API calls fail.

**1:50:21** · So a server or O error can look like a success. We need to gate those transitions on res.Kay and keep the dialogue open on failure. Thankfully there's a quick fix right here or we can copy just this part which is going to be the submit function. So copy the submit head over into the project actions or use project actions and again the these changes might be different for you as they are for me. So if you have some other issues to fix you can definitely do that.

**1:50:50** · I'll remove the submit bring in the correct one. Push the changes by running git add dot git commit-m implement code rabbit suggested fixes and run get push.

**1:51:10** · The changes will automatically be recognized right here. So we can go ahead and merge it and we are ready to continue.

### Editor: Access Sharing

**1:51:20** · Before we build the canvas, let me quickly explain how Live Blocks works.

**1:51:24** · Because once you understand it, the build order will make complete sense.

**1:51:29** · Livelocks gives every project a shared realtime room. Think of it like a live session. Everyone who opens the same project connects to that room over websockets and any change one person makes instantly appears on everyone else's. that canvas state, multiple users cursors, the AI drawing nodes, all of it lives in that shared room and syncs in real time. Livelocks rooms are open by default. So technically anyone could connect if we let them.

**1:51:59** · But since Ghost AI is a project-based app where only owners and collaborators should have access, we need to control who gets in with a sharing mechanism. So before liblocks connects a user to a room, it has to call authentication endpoints first and when we check whether that user belongs to a specific project only if they do we issue a token to let them in. That token endpoint is what we're building in this chapter.

**1:52:28** · And for it to work the access control and the collaborator model have to exist. So we're doing it in this order. Workspace access first. So each project has a secure route only authorized users can enter. And then we'll focus on the collaborator model second so the system knows exactly who those authorized users are. Then live blocks and then the canvas. So head over into context feature specs and create a new file called 08editor-workspace-shell.md.

**1:53:03** · And within it we'll explain exactly what has to happen next. So, let's go through it together. The goal of this prompt is to build the editor room ID workspace.

**1:53:14** · Remember, that's that page that we got redirected to and we saw a 404. So, if I create a new spec right here and we navigate over to it, we get a 404. So, this is the page we're building. Before rendering, the unauthenticated users will be redirected to sign in. The users without project access will see the access denied and non-existent projects will also show access denied.

**1:53:37** · Then we need to create that access denied component with a centered layout lock icon short message and a link back to the editor. And we can also create some helpers that are going to make it simpler for us to reuse the access functionality such as getting access to clerk's identity and checking whether they can access a specific project.

**1:53:58** · When it comes to the layout, we want to build a full viewport workspace layout with a top bar showing the project name, navbar actions at the top right, the existing project sidebar on the left, the current room highlighted in the sidebar, central canvas placeholder with a dark background and a centered message, and the right sidebar placeholder for future AI chat. This is exactly how the final version of the application looks like.

**1:54:26** · We have the left sidebar with the currently open project highlighted. the top bar with the icons on the right and then we have the AI chat which is going to be coming soon. The canvas area of course should fill the remaining space and in this case we want to tell it to not add any real canvas logic live blocks AI chat or sharing behavior yet.

**1:54:48** · That's the keyword right here. When it's done, it should perform the following checks. So, let's open it up within our agent and tell it to read the current file, update the progress, and execute it exactly as specified. Of course, make sure that it knows what file you're talking about. Let's run it and give it some time to process it. And after a couple of minutes, it is done. I actually took Codex for a spin to see how well it can handle it. And yeah, it said that it implemented feature 8 as specified.

**1:55:19** · The guarded workspace route now lives under this page, stays server side, and redirects unauthenticated users to sign in. The workspace shell component is right here, and it includes a project aware topn navbar with buttons to share. Okay, so let's go ahead and test it. Oh, this is looking nice. It is a bit different from the final design, but I actually love it. You can see how the sidebar collapses and then the central part actually expands. Later on, we can play a bit more with the design, but so far I love it.

**1:55:49** · So, right now, we are looking the details of the new spec project because you can see that we're on that specific URL. And if you just head over to the editor, you'll be able to see something like this. You can expand the sidebar and then navigate over to the details page. If the redirect isn't working for whatever reason, send a small corrective prompt describing exactly what's happening and it'll fix it. Now, let's test access control. Open up an incognito tab and then head over to the same URL.

**1:56:19** · You'll automatically be redirected back to sign in which is the first good sign. Go ahead and create a new account. I'll try to use the email and password this time.

**1:56:31** · Let's go with contact JSMy Pro and a password. And it's good to see that clerk is trying to keep us safe. So, it's suggesting a stronger password. So, let me do that. There we go. And for the email, I'll use a secondary email that I have because the first one is already tied with GitHub. There we go. And we're going to even have the email verification. So, you're going to get an email that looks something like this. Go ahead and copy the verification code.

**1:56:59** · Then paste it right here. And you'll be logged in and redirected to the editor.

**1:57:04** · So, if once again you try to go to that same project URL, you should hit the access denied screen.

**1:57:11** · you don't have access to this workspace, head back to your editor home to open up a project you actually can access.

**1:57:17** · That's great. So now let's allow this user to actually invite that collaborator. To do that, I'll head over within our context feature specs and create a new file called 09 share dialogue.md.

**1:57:33** · Let's go through it together. In this case, we're basically working on the share button. It's going to be within the editor navbar and it's going to open up the share dialogue allowing owners to invite collaborators by email. View current collaborators, remove collaborators, and copy the project link with the temporary copied feedback.

**1:57:54** · Collaborators can view the collaborator list only and not invite, remove, or manage access. It's also important that we're going to use clerk data for the collaborator sharing system. So, they're going to be stored by email in the database and we'll use clerk's backend API to enrich the collaborator email with display name and avatar image. And if a clerk user is not found for an email, then we can fall back to showing the email only. We want to add the required API logic for listing, inviting, and removing collaborators.

**1:58:27** · And we want to enforce ownership server side, not client side, for inviting and removing actions. Finally, we have a couple of checks to see whether everything's been done properly. So once again, let's open up Codex or whichever agent you're using and tell it to read the 09 share dialogue, update the progress tracker and implement it exactly as specified. We can do it within the same chat because this is somewhat related to the functionality we just worked on.

**1:58:56** · Let's give it some time and I'll be right back. And in about 5 minutes, feature number nine got implemented exactly within the specs scope. The workspace navbar share button now opens a new dialogue. So what do you say that we actually test it out? Back within the browser, but not the anonymous one, which doesn't have the access, we have to go to the one that is the owner of this workspace. We can now click this share button, which allows us to copy the workspace link or invite them via email. And I love this share interface.

**1:59:30** · So, I'll enter the email of my second account and click invite. You can see that the user has been invited as the collaborator. And since we signed up via email, this user doesn't have a profile photo. So now, if you head back and reload, check this out. The user now has access.

**1:59:50** · And for this user, it's not under my projects, but under shared projects. And this user doesn't have the permissions to update, rename, or delete. Whereas for this user, you can see that it's under my projects and we have full permissions. That's the full collaborator flow working end to end. On our invites, collaborator receives the invites and nobody else can access it.

**2:00:13** · And before we push the changes, let's review them with code rabbit. This time I'll do it directly within VS Code through the code rabbit extension. And as soon as the comments are in, we can go ahead and check them out within the use project share.ts file. That is the hook that the share button borrows the functionality from. And right here where we have the copy link button, this does nothing else than basically copy the URL to clipboard. But currently the copy link doesn't handle the clipboard API failures and the timer lacks cleanup.

**2:00:43** · So if the clipboard fails due to permissions or something else, the set timeout will still fire letting the user know that it has been copied. Whereas that's not really true. So we have to set the error in case something goes wrong. We can very easily do that. I'll just copy this part right here with a try and catch block. And we have to replace everything from await navigator.

**2:01:10** · So right here, await navigator. Replace it with this part right here. And we have to remove these plus signs right here at the start. Okay, great. So this one has been fixed. And I believe there's another one right here where we have the reload functionality. Reload silently swallows errors which may cause stale UI state. If the reload function fails due to a network error, the error is not captured and the UI may show outdated collaborator data after a successful invite or remove.

**2:01:39** · Which means that here we also have to check for errors and display them if there are any. So once again, I'll copy this part and replace the old one. And don't forget to remove the plus signs just to make sure it works. Wonderful. So two comments in this file resolved. We have one more in the project share dialogue.

**2:02:01** · This is the actual dialogue where we have a key collision when collaborators share the same email or display name.

**2:02:09** · Well, that's not really going to happen, right? Because each one of the collaborators is unique. So this isn't unlikely but it's impossible. So yeah, this one is good. And finally, there is one more under project collaborators where it says batch emails in chunks of 500 to respect clerk's API limit. Well, yeah, here where we're getting the users. Uh we definitely don't want to fetch more than 500 users. This is great regardless of clerk's limit, but I'm glad that it caught it because you never want to fetch so many emails at the same time.

**2:02:40** · So, in this case, it's not just a copy and paste, a couple of lines of code. What we can do here is use our agent to fix it. So, if you click that button, it's going to copy a little prompt and put it into the chat that's going to know exactly which part it has to fix. So, let's give it a second to read it and fix it. And it's done. The get clerk email now batches emails into chunks of 500 so that it doesn't go over the limit. But instead of doing that, what I actually want to do is never fetch more than 500. I mean, that's too much. So, I'll tell it.

**2:03:12** · Instead of chunking the emails, maybe we just don't have to fetch so many. We can just fetch fewer emails. So, let's see how it handles a bit more vague response. I mean, so far it has been implementing everything so perfectly because our prompts or our specs, should I say, were so precise. So, it never had any issues.

**2:03:35** · But yeah, in this case, it simplified it. It's going to call fewer emails.

**2:03:39** · Good. So, we're going to keep this. And now that all the issues have been fixed, we actually fixed these two manually. We can just go ahead and push all of these changes by opening up our terminal and running get addit-m implement share functionality and get push. Perfect. Great job.

### Editor: Liveblocks Canvas

**2:04:04** · Now that the access control is done and collaborators and sharing is enabled, we are ready to finally build the canvas.

**2:04:13** · First, click the link down in the description and head over to Live Blocks.

**2:04:18** · If you haven't already, create a new account. Create a new project, call it Ghost AI, and choose a region that is closest to you. And the environment can be set to development for now. Once the project is created, select personalized setup and multiplayer. Then select canvases as we want to focus on workflow diagrams, whiteboards, design tools, or in this case code architecture. And then for the guide, you can select React Flow with Nex.js. That's exactly what we're using.

**2:04:48** · Then copy the first command that you can see right here and paste it within your terminal. You can press enter. And here we're installing a couple of things. The liblocks client is the core client that manages the websocket connection to liblocks. Then there's the liblocks react which contains the react hooks for accessing shared room state presence and storage.

**2:05:11** · There's also the liblocks react UI containing the pre-built UI components.

**2:05:16** · There's also liblocks react flow which is the bridge between liblocks and react flow. So canvases are synced in real time across all the connected users. And finally the XY flow is the React flow itself which handles the canvas nodes, edges and interaction. Once that is done, we can initialize the liblocks config file. So go ahead and copy this command and paste it into the terminal and press enter.

**2:05:45** · This will generate a liblocks config.ts file at the root of our directory. This is where we define the TypeScript types for the shared room, what the presence will look like, what user data we want to attach to each connected session. You can think of it as the contract that describes everything shared between users in real time. And we'll configure it with AI. But before we do, let's install liblocks agent skills. Same pattern as with clerk and prisma. We want to allow our agent to be fluent in how liblocks works.

**2:06:17** · So go ahead and copy this command or follow along with me and just run mpx skills add liblocks skills.

**2:06:30** · Say y to updated and then select liblocks best practices and we don't need this second part. Press enter.

**2:06:38** · Select claude or whichever agent you're using and install it for the project and using sim link. Perfect. This was quick.

**2:06:47** · Now I want to split this specific feature implementation into three separate spec files. So let's take it step by step and I'll walk you through everything. First let's dive into feature number 10 liblocks setup. Here we want to tell it to set up the real-time collaboration infrastructure using liblocks. This file will wire up the entire collaboration infrastructure.

**2:07:11** · the config file. We'll get the presence and user metadata types and then we'll create a liblocks client. Finally, we'll build the O endpoints like API liblocks o so we can verify that people can actually access the room. So go ahead and open it with either codeex or cloud code. Tell it to read this file, update the progress and execute everything as specified and press enter.

**2:07:36** · Let's give it some time to do all the hard work for us while we remain the architect and monitor exactly what it is doing. And very soon feature 10 is complete. It implemented just three separate files.

**2:07:52** · The liblocks config now with types for the presence and user metadata. The lib libelocks file which allows us to fetch the cached liblocks node client so we can use its instance. And we also have the function that maps out a specific user color. Most importantly, we have the post endpoint that verifies whether the user has been authenticated and whether it has access to the project. If it does, it returns all the data. And we're one step closer to testing it out.

**2:08:22** · But all of these were just some functionalities that we need to use within our code, but we're not using them yet. So instead of testing at this point, what I want to do is head over to feature number 11. That's going to be the base canvas MD. So right here in lesson 11, we want to replace the canvas placeholder with a real liblocksbacked ReactFlow canvas, allowing multiple users to connect to a Liblocks room and share the same canvas state.

**2:08:53** · That means that the nodes and edges will sync in real time. And after that, we can basically say that we have a full collaborative canvas application. Not yet polished, but real. We don't want to add any controls yet or custom nodes or edges. We just want to create that canvas. So, let's open this up in a new chat. As usual, I'll tell it to read the file, update the progress, and execute as specified.

**2:09:25** · And I've just went to grab a coffee and feature 11 is done. So let's review it. It built out the canvas types so that our application remains heavily typed. Then it added the storage part over to the lib blocks config. This matters right here because it knows that we're going to be keeping track of the presence of the cursors and whether they're thinking, but also the storage of different nodes and edges and users on the screens. Later on, we're going to fill up these two.

**2:09:53** · And finally using liblocks provider and the room provider it created the canvas room and most importantly the canvas placeholder got replaced with that room. So what do you say that we go ahead and test it out?

**2:10:08** · Back on localhost 3000 we got connecting to a room but there is one issue. It says liblocks authentication failed reason not provided. Maybe because this project was created before our whole lib block setup. So, what I'll do is delete it, reload the page, and create a new project. I'll call it liblocks live room, and create. Unfortunately, we still get the same issue. Thankfully, the error in the terminal gives us a bit more info. It looks like we're missing the livelocks keys.

**2:10:39** · So, if you head over to your project under API keys, you'll be able to see your public key and the secret key. So, go ahead and copy them and add them to your env.local. local where we can first specify the liblocks public key as well as the liblocks secret key. With these two keys in place, head back over to your application and reload. And after connecting to room, you'll be able to see the actual canvas.

**2:11:07** · This is the ReactFlow canvas underneath that you can move through. And there's even a little window that you'll be able to scroll through to very quickly access specific parts of the workspace. This is looking absolutely amazing. We can even expand it by collapsing the left sidebar. Oh, and the right sidebar is collapsible too. So now we have a real fully functional React Flow canvas. But of course, what is the canvas for if we can't add any elements on top of it?

**2:11:36** · So let's create a little bottom navigation that allows us to add some shapes that are going to act as specific parts of the diagrams within our application.

**2:11:47** · We'll do that by creating a new feature spec called 12 shape panel.md.

**2:11:55** · You can add it right here. This one will be simple. And what this does is it adds a floating toolbar at the bottom of the canvas where users can drag shapes onto the canvas to create nodes, rectangle, diamond shapes, circles, pills, cylinders, and hexagons for databases.

**2:12:14** · And after this, users will actually be able to start creating the architectural diagrams. We want to allow the users to drag a shape including the shape name and the default size. Then they can also drag and drop it. And on drop, we need to read the dragged shape payload, convert it to the screen position, create a new node at that position, use an empty label and the default color. We then want to give each one of these shapes a node ID with their shape name, time stamp, and a counter.

**2:12:45** · And we want to render it. So, this is an exciting one. So, let's get it built, read the file, update the progress, and execute it exactly as specified. I'm sure there's an easier way for me to just read the file, and not have to repeat this sentence every now and then. I mean, I could have put it at the top of that file and just shared the file itself. That would have worked. Uh, but yeah, I don't mind it. It's the actual work that you put before that saves you so much time later down the line.

**2:13:14** · This one took a bit longer, but feature 12 is done. It created the canvas node renderer and a floating pill toolbar at the bottom with six dragable shapes. So, if you head back over to your room, take a look at the bottom. You have the rectangle, which you can drag and drop.

**2:13:35** · Hopefully, nope. As I dropped it, it didn't appear on the screen. Let's try with a second one. It looks like I can drag and drop them, but they're not actually showing up on the screen, which makes it a great opportunity to debug it the proper way by specifying in detail the current issue that we're experiencing. So, I took a second to write all of the issues that I believe we currently have with the application, at least that I have on my version of the app. Your agent might have done something different.

**2:14:04** · So, let's go through everything together first, and then you'll be able to tell your agent to fix some issues that you see on your end as well. Let's think of this as a little corrective prompt. So, review the editor canvas implementation and fix the visual issues. The canvas currently looks like it's floating above the background inside a border box instead of feeling like a real design canvas.

**2:14:27** · And I want to teach you how we can also add images to the context. So right here within the context you can create a new folder called screenshots and then you can screenshot the entire design and simply drag and drop it in. Of course I'll rename it to image as I specified right here within the document. That way you can also give your agent some visual feedback.

**2:14:51** · Also read the current canvas component code in the components editor. And here are a couple of issues to look for.

**2:14:57** · Obviously, and first of all, the drag and drop issues, right? The canvas nodes from the node panel cannot be dragged and dropped under the canvas. We need to investigate the full drag and drop pipeline. We need to confirm that the dragable nodes in the node panel have the correct dragable attribute. That the canvas has the on drag over handler and on drop allowing us to drop them. that the drop handler reads the node type from data transfer, calculates the coordinates, and then actually creates a new node at the drop position.

**2:15:28** · And while we're fixing the drag and drop issues, I also thought we can fix some uh visual inconsistencies, such as the way that the canvas and the left and the right sidebar are positioned. So the left and the right sidebar should float over the canvas, not push or shrink it. sidebars must use fixed position or absolute with a higher Z-index and so on. So after documenting all issues, we want to fix all of the above so that it basically corrects what we specified. So let's actually open this up right here.

**2:15:59** · We can tell it to read this file and fix all of the listed issues and then run it. So we've done three things. First, we gave Claude code some file references up front and the screenshots right here.

**2:16:16** · This stops it from wandering around the entire project trying to figure out where things live. We're pointing it exactly where to look. We're listing every issue one by one and mixing some technical hints alongside them. These technical details act as shortcuts. They give the AI the stronger starting point so it can find and fix the root cause faster instead of guessing. And third, at the bottom, we describe exactly what success looks like. The AI now knows not just what's broken, but what's done looks like.

**2:16:47** · So, let's see if it can manage to correct itself and fix it quickly. After reading through some of these files, it has a full picture of all the issues. So, it's going to use the to-do write to track the fixes and then implement them. Fix the canvas layout was the first thing. removing the card styling and making it a fill full viewport. Fixing the left sidebar not fully hiding when closed. Fixing the dotted canvas background visibility. And finally, and most importantly, verifying the drag and drop pipeline. And see how well we did. Uh it's even thanking us.

**2:17:21** · Uh specifying that the core issue is clear from the screenshot of the code.

**2:17:26** · The canvas is boxed inside a padded main with card styling and the layout shrinks the canvas to accommodate sidebars instead of floating over them. So, it's going to fix it very easily. Perfect.

**2:17:39** · Hopefully, this video is teaching you how you can approach developing apps with AI. You are the architect and agent is just a coder. And there we go. All four files have been updated. So, let's test it out. Back into the browser, I will reload. You can see that now the canvas spans across left and right and the left and right sidebar appear to be floating on top of it. So if you want to hide it, it just gets completely hidden away, which is great.

**2:18:08** · And the right sidebar also gets completely hidden away. So we have a complete canvas. This is a big difference from what we had before because now if you hide the sidebars, you have so much more space to work with. And what happens if we try to drag and drop an element? It looks like that functionality is still not working properly. And I think that's because Claude focused mostly on cosmetic changes and the layout. I don't see too many mentions of the drag and drop functionality being fixed.

**2:18:38** · So what we can do now is head over into the current issues and specify that we want to fix the drag and drop functionality.

**2:18:50** · So, we're going to remove everything else besides the drag and drop and keep the last part saying nodes can be dragged from the node panel and dropped under the canvas correctly. So, now we can say read the current issues file again and fix the remaining issue and press enter.

**2:19:09** · This time it's all about the drag and drop. And after some thinking, it looks like it found the root cause. The ReactFlow viewport has pointer events none. And React Flow internally uses D3 zoom or native pointer listeners that call prevent default on pointer down. So when the shape panel is rendered inside of the React flow as a panel, those pointer handlers interfere with the browser's drag gesture recognition before dragstart can fire.

**2:19:36** · The standard React Flow drag and drop pattern puts drag sources outside of the React Flow and puts onrop or on drag over on a wrapper div not on the React Flow component. So, it's going to fix this issue for both the canvas editor and the shape panel. That's it. No types of errors. The fix is clean.

**2:19:55** · We specified what was wrong and the fix was to move the on drag over and on drop from the react flow component to the outer wrapper and also to replace the panel position from bottom center which is react internal panel with a plain absolutely position div. So let's test it out back on local host 3000 within a specific project. I'll drag and drop this rectangle and it still doesn't do it. So what I'm thinking is maybe we can make use of that liblocks agent skills that we installed earlier.

**2:20:26** · I mean this is the exact situation they're built for. So in the same context window, let's simply tell the agent to check the lib blocks best practices and fix the drag and drop flow. Dragging shapes from the shape panel should create new nodes on the canvas, but it's still not working. Nodes should be draggable from the panel and dropped onto the canvas correctly. So by telling it to check the liblocks best practices, I'm hoping that it's going to consult the liblocks agent skill. So let's give it a shot.

**2:20:57** · And you can see that that is the first thing that it did. Libbel blocks best practices. After analyzing it, it came back with the complete picture with three things that are wrong. The storage type declares stople nodes and edges, but use slime blocks flow actually stores everything under a nested flow key within the canvas room. The initial storage creates tople nodes and edges.

**2:21:20** · Once again, wrong schema. And then the canvas editor add node mutation calls storage.get nodes, which writes to the wrong storage path.

**2:21:30** · Instead, it should use on nodes change with a type of ad and then the item we're adding. So, let's wait until it fixes all three. And it says clean. So, let's actually test it out. Back within the browser, I'll reload the page. And I'll try drag and dropping a node once again. And you can see that this time we actually get a shape. Now, if you try drag and dropping another shape, you'll see that it'll just give you another rectangle. And yet another rectangle of a different size. You're only getting rectangles.

**2:22:00** · And that's okay for now because in the next lessons, we're going to turn these rectangles into different shapes. We'll basically make it like a real architecture canvas where you can connect different nodes and give them titles and make them make sense. But thankfully, we fixed this shape drag and dropping feature, which is one of the bigger features in the app. And while fixing it, I wanted to keep the full process of me doing that. So, you're not just watching me copy and paste from the other screen. We're actually debugging this together. And in this case, the solution was to invoke an agent skill.

**2:22:35** · So, whenever you're working with specific tools, always verify that they also have their agent skills, install them, and ask your agent to use them.

**2:22:44** · Okay, great. So let's actually get these changes pushed by saying get add dot get commit-m implement drag and drop canvas functionality and then run get push and I'll actually open up a PR for this and get it merged so that in the next lesson we can focus on adding more canvas features. For these, we already reviewed most of the changes before, so I won't be reviewing them again. And we have to resolve the conflicts right here within our current issues. And there's a fix with copilot thing right here.

**2:23:15** · Resolve the merge conflicts in this pull request by clearing the current issues.md file.

**2:23:25** · We basically want to make it empty. As we said, we don't need to push whatever is in the current issues file. This is also a new feature by GitHub where the copilot can automatically fix it on our behalf. And once it does, we'll be able to merge it back to the main branch and continue developing. And there we go. It basically cleared out the file and we're good to merge it. So now back within the editor, you can just run get pull to pull the latest changes and we're ready to continue with the next feature.

### Editor: Canvas Features

**2:23:55** · In this lesson, the goal is to make the canvas feel like a real product. So, open up your feature specs and go ahead and create another one that's going to be 13 node shape.md.

**2:24:09** · In this lesson, we're going to actually polish and add six features. Each one will add a distinct layer of interaction so that by the end, the canvas will have proper shape rendering, node colors, edge behavior, and keyboard shortcuts.

**2:24:24** · everything that makes a difference between a working prototype and something that genuinely feels polished to use. So, starting with the first one, it's going to be the node shape. It's a fairly simple one where we just want to replace the placeholder node renderer with proper shape rendering and a drag preview. So, instead of a placeholder node shape, which is just a rectangle, we want to render all of these different types of shapes through SVGs. They should scale with the node size and we want to keep the border subtle.

**2:24:53** · We also want to add a shape drag preview while we're dragging. We want to keep the node rendering connected to the existing collaborative canvas state. We don't want to rebuild anything. And when we're done, we want to check that the node renderer renders the correct shape variant for each type. So, you know the drill. Open up your agent and let's ask it to read this file, update the progress and implement it as specified.

**2:25:22** · Let's give it some time and I'll be right back. And a couple of minutes after feature 13 is done, it replaced the single style placeholder with a shape aware rendering and also added the cursor tracking ghost preview. I'll show you what that means quickly, but basically now you can see that our array of rectangles that we created before is now a bunch of different shapes and we can actually move across the canvas and drag and drop different shapes.

**2:25:49** · There's a mini map at the bottom as well which we can later on remove as we don't need it as we'll be mostly working within a single centralized place. But yeah, we now have the shapes and you can actually connect the shapes together. But we still can't change the size of the nodes, right? They are always of the same size and we can't edit their labels. Like currently these are just shapes. They don't have any data associated with them. So what we can do is create another file right here, another feature 14 node editing.md.

**2:26:23** · And within it, we essentially want to add resizing and inline label editing to the canvas. so that when we select a specific node, we can resize it and scale them however we need to. And if we doubleclick it, we'll be able to edit its label. So this is the next feature that we're going to develop. I'll tell it to read the file, update the progress, and implement it exactly as specified. And you know what? I will actually copy this part right here. So in the future, I can just paste it into the prompt. Okay.

**2:26:55** · And after some wearing and coitating and thinking, let's see what it'll actually come up with. And as it's close to being done after running a couple of minutes, um near the end, uh when it tries to build and check for errors, it almost always finds some type issues. Like right here, it was complaining about the canvas node. So it expanded the types and made it a bit more type- safe.

**2:27:22** · And only once that is done, it actually updates the progress tracker and then finishes with the feature. So it's always great to ask it to test the application and test the output. Okay, great. So the resizer from XY flow now renders when a node is selected and we can resize dimension changes through live's on node change automatically. Also double clicking any node opens up a text area. So let's go ahead and test it out. We now have these labels which is perfect. But first, let's test the resizing.

**2:27:54** · If I now pull it at any of the borders or even at any of the edges, you can see that this is very precise and would take us some time to implement properly. You can now resize it both horizontally and vertically or if you want to keep the aspect ratio, you can resize it by the edges. This is absolutely amazing. And let's also test changing the label by double clicking right here and typing something like start of the app and leaving it.

**2:28:26** · And you can see that it looks good. It quickly brings the text up in case you want to type more stuff into it. But but we can fix that later on because the text will mostly always stay centered. So if we pull some kind of a label, we can now mark this as a Postgress DB for example and it's going to fall down right here. And we can now connect the application that way.

**2:28:50** · Perfect. Let's just quickly tell it that even though while we're typing into the field, we want the text to stay in the middle. Right now it jumps to the start.

**2:28:58** · So, I'll take a quick screenshot while I am typing and drag and drop it into the chat and tell it while the label editing is focused, the text appears at the top of the element instead of in the middle where it falls back to when not focused any longer. Make it so that when we're typing, we're also typing within the middle of the element. Hopefully, this should be clear enough for a little quick corrective fix. And very quickly, the build passes. It just sweped the text area for the content editable div.

**2:29:31** · So now if we head back right here and start typing, you can see that it remains in the middle. And you can say start here, we can say label. And as soon as we start typing, it basically centers itself right in the middle. Wonderful. So now that we can actually type within these inputs, what do you say that we implement the functionality to also be able to differentiate them by color? So create a new feature spec called 15 nodes color toolbar.m MD.

**2:30:01** · And here we want to add a floating color toolbar that appears when a node is selected. We then want to allow the user to pick a color and both the node background and text color will update instantly synced across all collaborators in real time. So it'll check our UI context for the node color palette, include a background color as well as a matching text color so that the contrast is nice and we want to reuse existing colors if they exist in globals.

**2:30:31** · Otherwise, it can keep the palette in the canvas types. Then we want to add a toolbar above the selected node that'll only show when the node is selected. And when a color is selected, we want to update the node background color and text color. I think this is pretty understandable. So, let's actually build it by telling it our usual secret sentence, which is super simple, but again, the spec file does the heavy lifting. This one, for some reason, was super quick.

**2:31:01** · It added the text color, the ability to choose between a predefined set of colors, and also the color background. So, if we head back over here and select an element, would you look at that? I mean, this is really starting to come into life. And I'm not sure how much time this would take me to manually code it out, but this way we just have to think of an idea, write a fairly simple yet descriptive uh spec file, and then it does it instantly.

**2:31:29** · And take a look, you can actually select the colors of each one of the nodes separately. So if I make this one purple, the database, for example, can be green. Uh, yep. For example, this one can be MongoDB in its classic green color. Then we can have some kind of an algorithm right here going on which can be orange. And yeah, it is all working wonderfully. So on top of the colors, what else is there to implement?

**2:32:00** · Currently, there's these custom edges from all four sides. But no matter what you select, it's always going to start making a connection from the bottom as you can see right here.

**2:32:09** · And it'll connect it to the bottom or the top as well. So, we want to fix that edge behavior. So, I'll create a new spec just for that. And you can see how I'm being very specific with the specs, only focusing on the smallest thing possible. So, 16 edge behavior MD. And the goal of this spec is to just replace the default canvas edges with custom edges that feel easier to follow, easier to click, and support inline labels.

**2:32:39** · So, we want to add connection handles to every node at the top, right, bottom, and left sides. And users should be able to connect from any handle to any other handle. Oh, and another thing you can notice is that we're opening up a new chat for every single one of these specs. This helps us with lowering the overall context window and the amount of tokens that we are spending for each transaction. And it also makes the agent that much more focused on the task at hand.

**2:33:08** · And all these little things together like the separate feature spec MD files instead of just regular messages or the current issues file where we can specify what's wrong and these six files that altogether make the system work just makes it a breeze to work with an AI which is typically not the case because it starts imagining things and creating stuff that we don't want or breaking other things. But this way it is super predictable.

**2:33:32** · And if you take a look at the progress tracker, which we haven't looked at in a long time now, you'll see that everything we've done so far is written right here.

**2:33:45** · But what I care more about is that it even kept some additional architectural decision so that it knows what we're doing and the session notes for specifically what it thought is very important like the specific versions of different tools that we're using. the fact that the Prisma config uses Prisma forward slash and not some other path and that it reads the database URL from the env. It kept everything it needs and everything that future sessions with AI or other developers continuing to develop this project need to do it in a sane and happy way.

**2:34:16** · And another build passes. It implemented the canvas edge data pieces allowing us to connect the source and the end. So if you head back over here, you can see that we have plenty of different lines happening. But now if you select it from the left side, you can see how it creates a bit of a different kind of connection. And you can now connect it to another element.

**2:34:40** · This line looks a bit different from other more organic looking lines. Oh, and right now we cannot even delete the elements. So we have plenty of elements on the screen. But I'll create a new one right here and another database on the right. drag the canvas so we can see them right here. Now the mini map starts making a bit more sense as you can see.

**2:35:00** · But if you try to connect it, you can now do that in a bit of a more consistent and better way. Now that the canvas is looking so good, I guess we can focus on little quality of life fixes. Like under feature specs, we're going to do 17 canvas ergonomics.md.

**2:35:18** · And within it, we can focus on adding a little floating control bar for zooming in and out and undoing or redoing and then wiring those actions to keyboard as well. So if you press plus or equal, it's going to zoom in, minus to zoom out, command or control Z or Y to undo and redo. And I also don't like that mini map at the bottom right. I don't think our app will need it. So I'll simply say remove the mini map at the bottom right.

**2:35:46** · It's just a personal preference, but yeah, this is that finishing layer that makes the canvas feel like a tool that somebody would actually use every day. So, let's implement this one as well. And very quickly, feature 17 is done as well. We now have a new pillshaped floating bar at the bottom left for zooming in and out or fitting within the view. So, if we collapse the sidebars, you'll be able to see it right here at the bottom. Ooh, it it actually looks very nice.

**2:36:12** · And if I move some things around, you can see that the left arrow or the undo actually starts shining and you can undo previous actions or redo them. You can also use command or control Z or Y to actually go back and forth which is absolutely amazing. There's this fit in view which is going to fit all the elements within the view. So if you're working on something that is a bit closer together, it's going to actually increase the view which is always nice.

**2:36:40** · And you can zoom in or you can zoom out, but that's hidden by the Nex.js logo, but that's only in development.

**2:36:48** · So these little things really do make a big difference. And finally, I had an idea that isn't even necessary, but I want to make it work. So let's create a new feature spec 18 starter template.md.

**2:37:03** · The goal of this one is to create a template library that lets users start from a pre-built diagram instead of blank canvases. So we can start with some ideas like let's say microservices or a CI/CD pipeline or an event-driven system. Each one will load directly into the shared canvas. That's going to make it easier for users to figure out how to actually use the app and what are the different use cases because maybe somebody is not going to even get the idea of what they can use this app for.

**2:37:34** · So, the templates should give them a pretty good idea. This one took a bit longer, but feature 18 is done. We now have the starter templates file. So, if you head over here and collapse everything, maybe we should start with a blank canvas, but we can keep doing it within our mess right here. Uh, at the top right there's the templates button.

**2:37:56** · And if you click it, you'll see a couple of different starter templates which aren't looking that good right now. They look a bit too vertical, but yeah, as soon as you click import, it'll actually import a lot of stuff pre-labeled. Uh, but it might be better to do that within a new project so we can see it a bit better. So, I'll call it CICD and create a new project. And then we'll start from a template by going with maybe the CI/CD pipeline or let's go with microservices.

**2:38:27** · And you can take a look that that immediately tells you a bit about how we can start structuring the application infrastructure. But yeah, this right now is looking a bit too vertical. The design is not actually being displayed.

**2:38:40** · So we want to take this screenshot and we want to feed it into the chat by holding the shift key and then drag and dropping. And then we want to compare that with how it looks like on the finished product where we can clearly see the full template before we drag and drop it. So I'll also put that here. And I'll say I'll pass in the screenshot of how the templates look right now. They look a bit too vertical and the actual elements are not clearly visible.

**2:39:09** · Whereas on another screenshot which is the finished product, you can see how each card gets its own space and they show the entire diagram or the entire template that's going to be entered in once clicked. Make it look more similar to that. So once again, this is a little corrective prompt with two different screenshots, one before and one after.

**2:39:29** · Let's see how well it does. So currently it looks like this. So I'm going to snap my fingers and we come down to something that looks like this. Definitely not good. Even though now it's a bit better as it's showing the full template that's going to be inserted in, but I'm not quite sure why it cannot get the widths right. So, we could be a bit more specific and tell it to increase the width of the whole import template card and then to increase the width of the cards within it so that they're the same as this.

**2:39:58** · And that's what I'll tell it for the second time by saying increase the width of the entire import template overlay. And then increase the width of the card within it as well. So it looks the same as on the final screenshot. And I'm purposefully being not as descriptive right here as we are within our spec files because I want to show you how it can cost you a lot by not being specific from the start. A lot of back and forth messages, conversations, and corrective fixes.

**2:40:27** · And very soon the fix is in and now it actually looks amazing. It increased the width and it's much clearer what it's actually going to insert in. So that means that we now also officially have the templates. So we implemented a lot of stuff across these five separate feature specs. 18 files changed in total which means a lot of stuff to review. This actually deserves its own pull request. So let's go ahead and push the changes either via terminal or via the source control right here.

**2:40:56** · It's going to autocraft a nice message such as improved node shape, added resizing and inline labels and adding color toolbars.

**2:41:05** · Then once you commit and sync back on GitHub, you'll see that the development branch had recent pushes 7 seconds ago.

**2:41:13** · So let's just open up a new pull request and let's wait to provide us with a review. I think this walkthrough will be particularly useful as we've covered many different features. So, this PR implements a comprehensive canvas editing feature set, including custom edge rendering with inline labels, node resizing with color toolbars, keyboard shortcuts for zooming and undoing and redoing, a canvas control bar, and a starter template system with a modal dialogue and SVGbased previews. We've made changes across 19 different files.

**2:41:47** · And here is the sequence diagram. The user clicks the templates button. It opens the editor navbar and then we open up the templates. We display the templates with card previews. The user imports them and then once they do, we pass the pending template prop. Then we forward that pending template to the canvas editor. Live blocks clears the existing nodes or edges, adds the templates, syncs this new graph to the canvas, triggers the fit view automatically, and then once it's imported, we bring it back to the user.

**2:42:20** · This is a nice diagram on the starter templates feature. This was a complex PR, so I'm assuming there's going to be a lot of different things we can fix.

**2:42:29** · The first one points out to exposing an accessible name on these icon buttons because title is not a dependable accessible label. It's telling us to add the area label title for the zoom, fit, undo, redo buttons for people who are using some assisted technologies. So, if I head back over here and hover over them, it will tell me that this is an undo. But for people with screen readers, this is not going to do it. And they will have no idea what these buttons are all about.

**2:42:58** · I mean, it's rare that these types of people would be using this kind of an application anyway. But it's always great to implement anything you're doing with best practices in mind. So, in this case, Code Rabbit provided me with a prompt for AI agents to use. So, we can add those area labels. After that, there's a major potential issue on avoiding double committing the edge label on enter or escape. So when pressing enter or escape, it'll call the commit edit immediately. Then the inputs on blur handler will call it again when the element loses focus.

**2:43:29** · This sends two mutations through live blocks, creating duplicate undo retries for a single edit. That's interesting. So the fix is simply to call the prevent default and prevent blur instead of commit edit. So let's find that. I'll find where this commit edit is getting called. It is right here in canvas edge component.

**2:43:51** · Specifically, we are looking at it on the enter key or the escape key. So right here. And instead of that, we want to apply those two lines prevent blur and prevent default. And we also want to remove the commit edit from the dependency array. After that, there's a minor issue to move ref updates into a sync effect to comply with React 19 ref values. So, basically, it's telling us to put it within a use effect. That's super simple. Let's just find where in the code this is.

**2:44:21** · And after that, you can see that even it's complaining right here about the code, but we didn't take a look at it because we weren't looking at the actual code. It's always good to use the best practices. So, we just need a use effect right here below. That's going to put all of these node refs into edges and nodes like this. And everybody's happy. After that, we're missing the enter key for handling the label commit. So if it says save the label on blur, enter or escape. But on handle key down, we only add escape.

**2:44:53** · So right here, we also have to add the enter key. I think we searched for this across the codebase just before. That was right here in the canvas edge, but not this instance. the instance where we just had the escape. So I'll search for escape and it's right here. We have to replace it with if key is escape or if is key is enter. And once again for you these suggestions might be completely different from mine and that's normal because agentic development is not predictable.

**2:45:24** · So for me it's adding some accessibility names or guarding some colors. For you it's going to be something else. But I always love learning about everything that Code Rabbit throws at me because next time I can immediately do it better. Or in this case, we can make our feature specs more specific so that our agents don't make these mistakes in the first place. Oh, and this one is interesting. When trying to undo or redo, it's currently looking only at a lowercase letter Z. But in case somebody has caps lock turned on, we also wanted to take a look at the uppercase C. This is interesting.

**2:45:55** · So, let's go ahead and push those code rabbit suggested fixes.

**2:46:02** · All of them were within the canvas.

**2:46:06** · And then once they're up, we can simply go ahead and merge this BR.

**2:46:12** · Amazing job on adding all of these little improvements that make our canvas that much more interactive.

### Avatar Feature, Chat Sidebar UI & Auto Save

**2:46:21** · In this chapter, we'll add the collaborators avatar. So when somebody else is moving something on the screen, you can see who is messing with you.

**2:46:29** · We'll also complete the chat sidebar UI and implement a canvas autosave which will save our canvas data to our versel blob so when you create something you don't lose it. And I'll break down all of these within three separate feature spec files. Each one is independent but together they complete the collaborative experience before AI generation enters the picture. So back within our application, create a new 19 presence avatars cursors.m MD chat.

**2:46:59** · The goal of this spec is to implement presence avatars and cursors because right now multiple users can edit the same canvas, but they can't see each other. And after this, every connected collaborator will appear as a live cursor directly on the canvas with their name and color. So we want to render those collaborator avatars and add those cursors to the canvas.

**2:47:28** · And also on the top right, we can show a stacked group of avatars where we can see everyone in the room at one place. So you know the drill. Let's get it implemented. And the presence feature has now been implemented.

**2:47:43** · There's a new component rendered inside of the canvas wrapper called the presence cursor as well as the collaborators avatars. So if you head back over to a specific project, we can stay within the CI/CD. Open up this project within a second tab. And check this out. Right here on top, you should see that Adrian is also within this canvas. But in this case, both of us are Adrian's. So you can see another person's cursor. And if I put these tabs side by side, take a look at this.

**2:48:12** · Using live blocks, while one user is doing something, all the other users in the room can see exactly what they're doing. So, this is a great first step toward interactivity. But we can do more. Head over and create a new feature spec or just get it from the zip called 20 AI sidebar shell.md.

**2:48:35** · The goal of this one is to create a sidebar placeholder that'll later on get replaced with a proper UI. Two tabs, the AI architect and the specs. The AI architect tab will have a scrollable chat area, starter prompt, chips, message bubbles, and a composer input, while the specs tab will have a generate button and a placeholder spec card. No backend logic yet, just the UI that everything else will connect to. So let's run it and let's see how it does.

**2:49:08** · And after a couple of minutes, it is done. In this case, it touched only the AI sidebar, which is a new standalone component as well as the editor workspace client where it replaced the old aside with this new AI sidebar. So now we got a new sidebar that looks something like this. You can see it on the right side. There's the AI architect, which soon enough will allow you to design full workflows and systems within the canvas, which looks like a chat because you're speaking with an agent.

**2:49:38** · And then there is a specs tab, which allows you to generate a specific specification and then later on download it. This is just the UI for now, but soon enough this will become real. You can also type multiple messages by pressing shift and then enter, which is useful for those longer prompt. Oh, and before we run the next spec, which is all about autosaving what we're currently working on, we need to set up Verscell blob storage. Verscel blob is basically an object storage service.

**2:50:08** · Think of it like a cloud drive for your app. So instead of storing large files directly in your database, you upload them to the blob and store only the URL reference in Prisma. We're using it for two different things in Ghost AI. canvas snapshots as save JSON and generated specs that will be available for download later on through Markdown. It's completely free to get started with. You can just head over to versell.com. Then on the left side, click storage and create a new database. Choose blob.

**2:50:37** · For store name, enter something like ghost aai and we'll set it to private because private storage means that your blob URLs require a token to access. Without this, anyone who gets a hold of your blob URL can read the file directly, which means the canvas data and generated specs would be publicly readable. But private storage keeps everything scoped to your application only.

**2:51:04** · So create it and once it is created, click on it and right here you'll be able to find your ENV local where you can just copy the snippet. Then within your env.local, local. You can simply add this new env blob read write token and we are ready to execute our next feature spec by adding a file called 21 canvas autosave.md.

**2:51:30** · Before we add that AI generation canvas state needs to persist. So after this every change to the canvas is automatically saved to versel blob which we just set up. And then we'll save the blob URL, store it in Prisma, and our canvas data will be saved securely. So this spec is all about saving the current canvas state. It should be pretty simple for our agent to implement given that we gave it all the information about the versel blob and about the environment variable that it can use to save data. And after a couple of minutes, it is done.

**2:52:02** · A versel blob is installed and blob readr token is already present in the env.local.

**2:52:10** · But if we get back to the editor, at least on my end, there seems to be a bug. So, let me show you how I would approach fixing it. To fix this issue, you can just copy it, head back over to our application, specifically into the current issues.mmd, and specify that this is the current error that I'm seeing on the screen. And you can paste it right here. It's going to give it all the necessary information and you can say fix it.

**2:52:42** · So make sure that it has access to the current issues and say fix it or you could have just pasted that into the chat itself. For just a singular issue like this, it should be totally okay.

**2:52:53** · And as it's working through it, I can already see what was the issue. Even though we ran MPX Prisma generate and migrate, the generated client is correct, but there's a stale. Next cache bundling the old schema. So, it's going to clear the old cache and then delete it, which forces TurboAC to recompile from a freshly generated Prisma client, which already has the canvas blob URL.

**2:53:17** · Then, we just have to restart our server and the error will be gone. So open up your terminal and just rerun it by saying mpm rundev and then back on localhost 3000. If you reload the error will be gone. So now we are ready to test that final feature we implemented.

**2:53:33** · Head over to one of the active projects.

**2:53:35** · Add a couple of nodes right here.

**2:53:37** · Refresh the page and make sure it remains at the exact space where you left it at. So, I'll try to change its name and move it below the O service and just make sure that it actually remains there, which would mean that the autosave is working. Perfect. But even though it saved it, it wasn't saved through a blob because if you head over to the Ghost AI blob storage, you'll see that there is absolutely nothing there.

**2:54:00** · So, let's fix this issue and a couple others. I went through the application, tested it deeply, and came up with a couple of different issues that I added in the current issues.md file. You should already have a file like this in your zip, which you can just refer to.

**2:54:17** · But again, it's possible that for you, you'll have to go through the app yourself, try to find some specific issues within your app, and then write the prompt to fix them. But yeah, in this case, let's go over the most important one, which is the saving button in the workspace navbar. Uh the workspace snapper is missing a save button. The autosave hook exists but we need to wire the button to it. It should default to save. While saving it should switch over to saving. After successful save it should switch over to save. And that's it.

**2:54:48** · The most important thing that I noticed right here is in this canvas route. TS file if you take a look at the blob storage the access is set to public. And remember what I said before, it has to be set to private because we don't want other people to be able to view the changes we make within the canvas. So we need to set it to private and we're not asking it to change anything else for now. For now, I just want to focus on issue one and then later on go through all of the other issues. So yeah, let's ask it to fix the save button first.

**2:55:21** · I'll open up a new chat and tell it to read the current issue MD file. Check the issue one and fix it. After fixing it, mark it as pending to test. Let's run it and see how well it does. And very quickly, issue one is fully implemented and marked as pending for tests. So, let's go ahead and test it out. You can see the save button right here. And as you move something on the screen and change its color and click save, you can see that the saving indicator is not really changing.

**2:55:51** · So, you can quickly head over to the codebase. See, there's no errors in the terminal, but it's still not doing its thing. So let's send it one quick corrective prompt by telling it that issue one still hasn't been fully fixed. The saving status indicator is not being changed and when I click the save button nothing is changing either analyze the issue further and fix it and we can send it out and it was doing a bit of thinking but it came back with a response that the root cause was react

**2:56:22** · mode enabled by default in nextJS app router. It double invokes effects in development. So on initial mount, the cleanup is intentionally fired by the strict mode before remount and then remount effect only registers the cleanup again, but it never resets. So that means that the ismounted is permanently set to false in development.

**2:56:42** · So the save exited every time. This fix removes the ismounted refer uh because React 18 made this guard unnecessary. Perfect. So, if we head back right here and reload, and if you move something around and then press save at the top right, you can see that it says saving. And then we get an error. Save failed. If I move it again a couple of times and click save again, it says save failed.

**2:57:11** · It's funny because when I tested it initially, it actually said saving and then saved. So back in the blob storage, you can see that I have this new canvas and it actually stored the JSON data.

**2:57:22** · But then when I try doing it again, it failed. So if you open up the terminal, you'll see that we have an error with the versel blob saying that the blob already exists. So we should add allow override is set to true if we want to override it. So what we can do is simply find this file that's the canvas root.

**2:57:42** · So you can go over to canvas root and just add an additional prop of allow overwrite is set to true. This single line should immediately allow us to save every other time not just the first time. You can see it says saved and back when the blob you can see that it got modified less than a minute ago which means that it is consistently saving data. And right now the size of this JSON file is 6.11 kilobytes.

**2:58:12** · But if we head back and add a couple more labels and models and shapes and some pieces of text within them and then save again and then head to the blob, you can see that now the size increased which means that it is properly saving all the data. So now that our issue one has been fixed right here, uh we can ask it to continue fixing the other issues. uh specifically some issues that are found are about deleting nodes and edges.

**2:58:39** · Uh so right now we don't have a way to delete anything. So if I try pressing backspace or the delete keys or anything, I can't do it. So the solution is simple. We just need to add a key down event listener to the canvas that listens for the delete and backspace keys. doesn't fire when the event target is an input or text area but just gets fired when we are selecting specific nodes and then it deletes them.

**2:59:07** · As the third issue uh currently we can also just connect from top to the top of the handle. You can see even if I drag from the right handle it connects from top to top. We want to be able to drag and drop from any side of the element to any other side. that will allow us to make these graphics so much more customizable. So, we just want to allow it to be connected from top, right, bottom, and left.

**2:59:34** · Then, as the fourth issue, I noticed that when I drag and drop specific elements, they drop a bit lower than where they're supposed to. So, I just wanted to fix that offset.

**2:59:48** · And notice when I dragged and dropped it, it actually said saving at the bottom left right here. And then saved, which means that the autosave functionality is working. And then the fifth issue is the auto zoom on first node. We want to read the live blocks agent skills before implementing it. And then as soon as we drop it, we want to zoom it in. And for six and seven, we want to check the clerk skills. Um, and we have some issues with the collaborator avatar images. If the image is coming from clerk, we want to add it to next config so it gets properly shown.

**3:00:19** · And also currently we have two different clerk buttons. We just want to keep the one and remove the other one.

**3:00:27** · So let's ask it to fix the errors from two all the way to 7. Okay. Now that the issue one in the current issues.md file has been fixed, uh analyze and fix issues from 2 to 7. Press enter and let's see how well it does. Okay, it looks like all the remaining issues have been implemented and uh it marked them for pending test. Uh which is a good thing for us to test.

**3:00:53** · Right now we have to test deleting the nodes and edges um handling uh the positions or the lines in between the elements, draw position offset, auto zooming and then clerk images. So, if I head back right here and reload the page, let's first test the drag and drop. So, if I try to drag and drop it here, you can see that it gets placed at the exact position. This is pretty crazy. Take a look at once again. I'll try to place it right here.

**3:01:24** · And it worked. Of course, it's going to depend on the zoom position. I think if we at a normal regular zoom and you once again drag and drop it to a specific position, that's exactly where it places it. So, that has been fixed. Also, now there's just one clerk icon right here where you can see your account. Uh, what else did we fix? The edges connections.

**3:01:46** · So, for example, let's try to drag and drop the bottom of this edge right here to the left side of the test suite. And take a look at how well it connects. It even places the arrow from here to here.

**3:01:58** · Or maybe when I go into the package, that works as well. And the arrows move.

**3:02:03** · This makes our application so much more usable because now for example we can connect the O service horizontally with the database and then take the database output and do something with it. Again this canvas is becoming a mess right now because there's so much stuff happening.

**3:02:21** · So it would make sense to test out delete. Select a couple of elements and try to press the backspace or the delete key and see whether it's going to remove them. because for me it doesn't. So it looks like that's the last issue that's still pending. So let's just tell it that issue two remains unfixed. When I select an element and press the backspace or the delete key, the element is still there and isn't being deleted from the canvas. Analyze it and fix it.

**3:02:51** · So let's see if we can just narrow it down to one issue whether it can finish that last one. And again, this just shows you that whenever you give it more stuff to fix, uh it's easy for some of these to uh fall through because it maybe didn't analyze them as deeply in isolation. Uh so you can see why these feature specs worked so well so far because they were super detailed and well documented. But as soon as you go deeper into the conversation, the agent can easily get lost.

**3:03:22** · So this is its last chance. Let's see how well it does.

**3:03:27** · It looks like it was able to find a root cause in about 30 seconds. In apply node changes inside of the liblocks react flow source. We had a case of remove which was not doing anything. Uh so it was silently ignoring the remove type changes. Whereas livelocks exposes a dedicated ondee function that correctly deletes from the live map. So it fixed it and let's see how well it does right now.

**3:03:55** · I'll reload the page and then I'll select a couple of elements and press the backspace key and now it deletes them properly. Now, if you don't want to delete them one by one, you can also hold the shift key and then drag and drop over multiple and remove them that way. Also, another thing that I didn't tell you so far is that you can also add uh text to the lines connecting different elements like we want to build and then run the test suite.

**3:04:22** · So, this way kind of it makes more sense with the connection, but you can also use the text on the lines for significantly more detailed instructions when it comes to connecting different elements. But yeah, now that all of these issues are fixed, we can go ahead and push them. So say get add dot get commit-m and this lesson was all about canvas interaction. So say implement improved canvas interaction and then run get push.

**3:04:53** · Now in the next lesson we'll focus on the AI collaborative side of the application.

### Trigger.dev Setup

**3:05:02** · And now that we have the full canvas right here where we can drag and drop elements, move things around and create our own architectural systems, we are ready to help our users a bit by implementing the AI workspace where we can allow our users to collaborate with our AI agent within the application that I'll teach you how to implement right now.

**3:05:27** · But I want you to think about it a bit like before we start building the AI generation features um you need to understand why these can't run inside a normal API route. See, when a user sends a prompt to Ghost AI, something like this, to design an e-commerce backend, the agent doesn't just make one call. It analyzes the request, runs multiple AI steps, generates nodes and edges, and syncs everything back to the canvas, all while keeping the user updated.

**3:05:58** · And that can easily take 30 to 60 seconds, maybe even a couple of minutes. And I mean you've already seen this pattern when you generate an image with Chad GPT or Gemini. It doesn't happen instantly. The work runs in the background and you keep receiving the updates until the response is ready. And the API routes within our application are not designed for that.

**3:06:21** · They have execution limits which means that long running requests can time out.

**3:06:26** · And even if they didn't, keeping a request open for that long isn't how production systems are built. That's when I'll teach you how to implement trigger dev to solve this problem. In the final version of the application, if you give it a detailed prompt and send it, you'll be able to see direct updates as it is working on the thing.

**3:06:44** · It'll first start with analyzing your architecture request and all of these functions will run as durable background tasks outside of the request life cycle which means that the work is running in the background and you'll be updated on the process. So the work of the API route is to just trigger the task and then return while the heavy work continues in the background.

**3:07:08** · And that's why both the AI design generation and the spec generation in Ghost AI run through trigger dev instead of directly in API routes. And even before we used trigger on Ghost AI, I was already using it within jsmastery.com platform where

**3:07:27** · every time that users go through different lessons, check out the overviews, contents or transcripts, we can perform some actions on the back end without slowing down or freezing what the user can see on the front end, which is super helpful for quizzes or sharing the status of the AI interviewer that we worked on. So yeah, let me show you how we can set up trigger dev in your project.

**3:07:49** · First, click the link down in the description to be able to follow along and see exactly what I'm seeing and then create a new account. Once you're in, you should be able to see your dashboard that looks something like this. So, go ahead and create a new project. I'll call it Ghost AI.

**3:08:08** · We are working on an AI agent. And under technologies, I thought that Gemini works the best. So, you can proceed with Google Gemini. And what are we trying to do with trigger? Well, we're still learning how trigger works as well as potentially shipping a production workflow. So, let's create it. Then, once it is created, you can run this CLI command to initialize it in the existing project. So, just copy it, head back, open up the terminal.

**3:08:35** · You can do it under a new tab, and just run MPX trigger.dev at latest init. and then pass your specific project ID. Say yes to install the TriggerDev CLI. And this will now install the Trigger Dev SDK and initialize the config file. But it'll first ask you a couple of questions such as choose how you want to initialize your project. In this case, we'll proceed with the Trigger Dev MCP, which allows you to vibe your way to a new project.

**3:09:07** · Well, in this case, write detailed project specifications to come up with a new scalable project. It's going to ask you whether you want to restrict the MCP server to the dev environment only. I'll say no. And then you'll be able to choose one or more clients to install the MCP server into.

**3:09:25** · You can choose all the ones that you're using such as Cloud Code, VS Code, OpenAI Codeex, or really anything else that you want. And then press enter.

**3:09:35** · Where should the MCP server for cloud code be installed? I'll go over with the project.

**3:09:42** · Same thing for all the other ones.

**3:09:45** · And that's it. We now need to restart our MCP clients. In your client, look for a server named trigger and then get started with Trigger Dev by asking it to add Trigger to our project. So, let's do just that. I'll open up our Claude code and that's going to be on a new chat window. And I'll simply tell it to add trigger dev to my project. And we can now run it. But just before I do, I want to share another thing with you.

**3:10:10** · And that is that trigger also supports agent skills to teach any AI coding assistant best practices for writing tasks, agents, and workflows. So we can install it as we did for all the other dev tools by opening up the terminal and running mpx skills at trigger.dev skills.

**3:10:32** · We can choose uh trigger agents, config, and maybe setup. I think that's going to be all we need for now, but you can just go ahead and add all of them as well.

**3:10:43** · Choose your specific agents you want to add it for. Do it within the projects through Sim Link and then quickly install it. Now, let's go ahead and ask it to add Trigger Dev to my project.

**3:10:56** · Then, let's run it. It's going to explore the project structure, find all the relevant files and the architecture context, which matters a lot. It's going to get the full picture, and it'll start with configuring the trigger config.ts, creating a trigger directory with example tasks, adding the trigger.dev route handler, and finally updating the progress tracker. And there we go. After a couple of minutes, the trigger dev is now set up. So, it first added the trigger config.js. js. So let's quickly go over into it.

**3:11:28** · That's going to be within our trigger.config.ts in the root of the application and it looks something like this. It is coming from trigger dev SDK. We define a specific configuration and then we need to connect it to a project reference.

**3:11:48** · This is coming from our environment variables. So very soon we'll have to find it in our trigger dev dashboard and then add it to ourvves. Then below the project we can add a runtime and set the environment to node. When it comes to directories /trigger is going to be fine or in this case I think we can just leave it to trigger. Now max duration stands for the max compute seconds a task is allowed to run.

**3:12:15** · If the tasks exceed this duration, it'll be stopped. And by default, we can set it to something like 3600 so that any task can run up to an hour before it stopped. But again, that's not needed because most of our AI tasks will be done in a couple of minutes. And then for the retries, if something fails, Trigger Dev will retry it up to three times with increasing delays between each attempt. So having that built right in to make sure that if something does go wrong, which it often does with AI generation, it retries it.

**3:12:45** · So when your user comes back to your app, whatever they were waiting for from an AI agent is waiting for them there. Okay. So let's get those keys. I'll head back over to Trigger Dev. Specifically, scroll down to API keys. And right here, you'll be able to find your secret key.

**3:13:04** · So simply copy it. Then head over into your env.local.

**3:13:10** · And here we can add as it specifies the trigger project ref as well as the trigger secret key. So the secret key is the one we just copied. And the project key you can find right here by going over to the tasks and copying it right here from the end part of the CLI init command. And then just paste it over here. And the next part is to start your local dev workflow. And I think this is the exact second step from our 3minut setup. MPX trigger dev at latestdev.

**3:13:41** · So you can open up your terminal. Make sure that it's not the one running your application. And before we run this, let me actually explain what it does. This is specific to local development.

**3:13:55** · Trigger dev background tasks don't run on your machine automatically. They need a local worker process running alongside your next.js dev server. So just run this command. Would you like to install the trigger dev code agent rules? Well, yeah. Go ahead. We can select it for cloud code or whichever other agent you're using and choose the rules you want to install. Uh let's go with basic advanced. You know what? Let me go with all of them.

**3:14:24** · Now it's going to wait for you to log in to your Trigger Dev account, which you can do by simply heading over to this URL and then authenticating your account. Once you're successfully authenticated, you can head back and you'll be able to see a screen that looks something like this.

**3:14:40** · Log in successfully. Trigger dev is running and the local worker is ready.

**3:14:46** · So keep this running whenever you're developing locally because without it, any task you trigger will cue but never execute. And in production on Versell, this isn't needed because trigger dev will handle the worker infrastructure for you. So, if you now head back over to your dashboard, you'll be able to see two different tasks, generate design and generate spec, which is absolutely amazing. This was going to be one of my upcoming project specifications to add, but it looks like the MCP already figured out exactly what we want and it created those tasks right here.

**3:15:17** · So, soon enough, you'll be able to see how those tasks actually run and then see more information about it. So that was it for the setup and then in the next lesson, let's build the AI generation logic.

### AI Architecture Design Generation Flow

**3:15:33** · Okay, Trigger Dev and the agent together already created for us the task skeletons, but in this lesson, we'll build the full AI generation flow. Now, before we make our systems design agent logic, we'll have to install a couple more packages. So, open up your terminal. We'll have to go with the third one right here. and run mpm install at trigger.dev/react hooks which lets the front end subscribe to a live trigger dev background run without manually pulling.

**3:16:04** · So think of it like instead of asking is the job done yet every few seconds. The hook will stream in real time status updates directly to the UI as the task progresses. Then there's the at AI SDK Google which is the Google provider for the Verscell AI SDK. And in this case, we'll be using Gemini for both design generation and spec generation. But of course, feel free to use any other agent you prefer.

**3:16:31** · And finally, AI is the core Versel AI SDK, which is going to give us utilities for generating text or generating different objects by working consistently with any kind of AI provider. So, go ahead and install these three. And while they're getting installed, head over to aistudio.google.com, which we're going to connect with TriggerDev to infuse it with all sorts of different functionalities. So, click get started. Make sure to authenticate with your account.

**3:17:01** · And Google AI Studio will give you free credits in most regions, which is going to be enough to test out the generation flow throughout this build. So, click get API key. Then, create a new API key.

**3:17:14** · You can call it something like ghost AI and then you'll be given all your API key details. So first copy the actual API key and paste it into yourv.local.

**3:17:28** · Specifically that's going to be under google\_ai\_appi\_key and it's going to be set to this key you just copied. Or if you want to get a completely free alternative to Google Gemini, Open Router has a pretty good selection of free models, I'd recommend this Nvidia Numatron 3 Nano Omni. That's a mouthful, which is a free model that has a 256,000 context window and it handles the architecture generation pretty well.

**3:18:00** · Just keep in mind that the free tier models always have usage limits. So if you go that route, simply swap that AI SDK Google thing for the open router SDK in the generation task.

**3:18:12** · For this video, I'll personally use Google AI Studio, but again, as with the AI agents, follow along with whichever one works for you. So now with the setup ready, we are ready to start adding the trigger dev task spec files. So head over into our context feature specs and find or create a new one called 22 design agent API.md.

**3:18:38** · The goal of this feature is to set up the backend flow for design generation using trigger dev. And keep in mind that when we're referring to design here, we're referring to the systems or architecture design of our applications.

**3:18:51** · So, we're setting up this design agent API for the backend wiring. Starting with the trigger route where we need to create a specific post route that should accept the design prompt and some context and then trigger the design task through trigger dev because as I said these tasks and these AI prompts can take some time to process. Then we'll add task tracking. This is going to be a special model in Prisma to track triggerdev runs and verify ownership.

**3:19:21** · Who created the run, when, and what is it all about. We should add the token route to verify ownership and then finally create the actual design task.

**3:19:32** · We want to check the existing trigger dev setup and installed agent features.

**3:19:36** · Reuse the existing setup, export a minimal design task, and for now, not add any design logic yet. just the infrastructure that makes the next spec possible. You learned that already. Spec by spec, we're getting closer to the final solution.

**3:19:53** · So, let's go ahead and run it. As usual, you can just tell it to read the current file, update the context progress tracker, and implement it exactly as specified. And after some work, feature 22, the design agent API has now been completed. It created a new Prisma model called task run with run ID, project ID, user ID, so we know which projects are being run over in trigger dev.

**3:20:18** · Then there's the design agent itself, which is a minimal task accepting a prompt in a room ID, which logs and echoes the inputs. So if you open it up, you'll see that it looks like this. Currently, there's no logic and functionality, but we'll add it very soon.

**3:20:36** · Then there's the post API AI design which requires authentication and what this one does is it basically figures out whether the user is authenticated, takes in the body and finally creates a new task run in the database. But of course before it hands it over to trigger dev. But now the actual task is pretty empty. It's just console logging design agent triggered and it's not doing anything else.

**3:21:03** · So our next task is to implement the full AI design agent logic so a user prompt results in real-time updates on the canvas. To do that, head over into our feature specs. And let's focus on adding the 23rd spec, which is design agent logic.md.

**3:21:25** · And as I said, the goal here is to implement the full AI design agent logic. So first we need to update the file which was just created before we want to check the product behavior of the system. Check the live blocks and trigger agent skills. This is very important. Sometimes you have to explicitly tell it to check the skills.

**3:21:44** · Follow the trigger dev setup and agent patterns already set up. Reuse the existing lib blocks flow and presence patterns instead of creating new ones.

**3:21:52** · And then implement use Gemini logic to interpret the user prompt. Update the canvas using the collaborative flow utilities supporting actions like adding nodes, moving them, resizing them, updating them, deleting them. Basically, everything that our application is already doing. Then we want to publish that AI activity to the shared status feed so all users can see the progress, update the AI presence through cursors and thinking state and push clear status messages at key steps.

**3:22:22** · If you think about it, this is a very important and big feature spec, maybe the biggest one in our application so far because now we are essentially telling our AI agent and trigger to figure out the entirety of our application and to replicate its functionality on its own while following the user prompt like the user is telling it to create something on the canvas and it should create it.

**3:22:51** · So, let's go ahead and see how well it does by opening up a new clot code window, giving it access to the file, and asking it to read the spec file, update the progress document, and implement it exactly as specified. This is a big one, so I'm super excited to see how well it actually does it. And feature 23 is now complete. Uh, this one took a bit longer because it's a it's a huge one.

**3:23:19** · And we now have a full AI agent built within our application powered by trigger.dev.

**3:23:27** · It uses Gemini 2.0 Flash via create Google generative AI plus generate text with output object to produce a typed list of canvas actions for adding, moving, resizing, updating, and deleting nodes and edges. It sets the AI presence by thinking is set to true. So all collaborators can see the AI cursor. It broadcasts three different statuses, start, thinking, and complete. And it applies all mutations atomically in a single mutate storage call. Perfect.

**3:24:02** · This is exactly what we wanted. So while we can't see it on the screen just yet, what we can do is head over to our trigger.dev dashboard under tasks.

**3:24:13** · Currently, we have three separate tasks.

**3:24:15** · That's because our initial setup task created the skeletons for generate design and generate spec, but the new one is right here under design agent.

**3:24:23** · So, what we can do is maybe we can clean up the other two just so they're not confusing us. So, under trigger, we can remove the generate design and generate spec, which are just empty placeholders.

**3:24:36** · And instead, we can just leave the design agent right here. So, that's the only one that remains. Now open it up and perform a test run. It's going to ask you to pass the data as a regular user would through the application. And we can write something like room ID. And you'll have to get this room ID directly from one of your canvases. So head over here and create a new project. Let's call it something like um system design.

**3:25:06** · Create it. And you can copy the project ID directly from the URL right here at the top.

**3:25:13** · Then if you head back, you can update it over here. And we can ask it to architect a real-time chat application.

**3:25:20** · I need a websocket server for live messaging, a present service to track online users, and a relational database for message history. Connect the services using a pub subsystem like Reddus so it can scale horizontally and include an S3 bucket for media attachments. I'll give you a prompt like this in the video kit link down in the description so you can copy it and paste it. But make sure to update the room ID.

**3:25:46** · And now let's go ahead and run the test.

**3:25:48** · Oh, but before make sure that your dev server is connected right here. If it's not connected and then we'll be able to run the test.

**3:25:57** · As you run it, you'll be able to see all the information about this specific task run. When it was triggered, when it was ceued, and when it has started. Now, immediately it'll fail after three attempts saying that we exceeded our current quota, and we need to check our Google billing plan. So, it's super convenient to be able to test the runs directly within the trigger dashboard.

**3:26:20** · So once you top it up or change your providers, uh you can just reload your trigger dev server and then replay the run.

**3:26:28** · Hopefully this time it continues running after just a couple of seconds. And we get another little API error saying that models Gemini 2.0 flash is no longer available. Um I wish they made those backwards compatible, but it is what it is. We got to find one that actually is compatible. So, instead of using 20 flash, I'll head over into this design agent file. That's going to be right here. And I'll switch it over to 2.5 flash. I believe that is the latest running model.

**3:27:00** · Then, when you change it, don't forget to rerun your server again, the trigger dev server by running mpx trigger at latestdev. Then, after it creates the local worker, go ahead and replay the run. Third times the charm or apparently not because after about 20 seconds we got a little error saying no object generated response did not match the schema.

**3:27:27** · So open up a new chat and let's tell it something like this. while implementing at 23 that's going to be the 23rd design spec that we try to do the agent logic

**3:27:44** · or rather we can say after implementing I try to run a test and then I give it some more information that we use for the test itself and then pasted the error that we got which you can get from the web finally we can tell it something like analyze trigger.dev dev and liblocks best practices analyzed this doc and I shared it a link to the doc of

**3:28:06** · the generating structure data part because so far it generated it just as text but what we need to do instead is have some kind of a schema that we can validate against. So currently it is using this output but what we can do is use a so-called tool calling approach with generate text with a tools object.

**3:28:28** · So I'll tell it analyze this docs page and the error and then I'll pass some additional info which I think is the reason for why it's failing. So that design agent is failing because generate text is being used with output object for structured output. That experimental API is causing the runtime error. So instead replace it with a tool calling approach using generate text with a tools object. Each canvas action should be its own tool. So we have the add node, move node and so on.

**3:28:58** · And this way it's going to follow the schema precisely. So have a message that looks like this and send it out.

**3:29:08** · This is also a useful approach uh to share it a link uh to a specific documentation page so that it can do a web fetch and figure out how it works.

**3:29:17** · Or alternatively, there's also this context 7 which is a library of the latest documentations that you can directly fuse with cursor claude or other LLMs. For example, it has the latest docs for Nex.js updated 9 hours ago. Same thing for React and most likely for AI agents as well. There we go. AI SDK. This is what we're using.

**3:29:40** · So, if we hook this up with our agent, and you can do that very easily just by copy and pasting this thing right here, it would have all the latest docs. But let's see what it can do with just the URL. And very quickly, the build passes.

**3:29:53** · Here's what changed. The output object in generate text relies on the model emitting a single structured JSON blob, but Gemini 2.5 Flash returned a response that didn't match the schema, triggering the AI no object generated. So in this case we're replacing the output with a tool approach where each canvas action is its own name tool like add node move node and so on. So after generation all tool calls are collected and then we get the final canvas. Okay. So let's go ahead and test it out.

**3:30:24** · Back on trigger dev we can just replay the run. And in about 15 seconds it finished. We got a successful output with 11 actions applied and a summary of what happened.

**3:30:37** · Now, let's make it even better by adding another feature spec right here. That's going to be 24 AI presence state.md.

**3:30:48** · And the goal of this one is to add a shared activity indicator so that when AI is generating, everyone in the room will see it. A status indicator in the sidebar as well as a thinking spinner cursor and the input will be disabled while generation is active. So, let's go ahead and run it with the usual message.

**3:31:11** · And let's give it a minute. And I sped up the process for you, but this one definitely took some time, but thankfully the build passes cleanly. We added some new types for the tasks.ts, modified the liblocks config, and added the presence cursors. But before we actually go ahead and test this out, I want to finish the implementation of the sidebar so we can test everything we've been working on together. So go ahead and open up a 25 sidebar chat feed.md file.

**3:31:45** · And within this one, the goal is to wire up the AI chat libelocks feed into the sidebar. See, live feeds are realtime message channels. Think of them like a group chat that is tied to a specific project room. Anyone in that room can send a message and everyone else can instantly see it. In this case, we're using two separate feeds. The AI chat feed and the AI status feed.

**3:32:11** · The AI status feed is simply for some kind of progress signals and AI chat is for the actual conversation. This spec handles the chat side where users can send messages and make them appear across every connected client. So let's go ahead and run it and I'll speed it up for you. And feature 25 is done. Here's what was changed across three files.

**3:32:37** · First added some additional types. Then in the config we extended the feed message data with optional chat fields.

**3:32:46** · So now it also supports the sender roll content and timestamp alongside the existing AI status fields. So they both coexist under the same type. The key addition right here was the chat feed ID constant. So now we support the chat alongside the status updates as well.

**3:33:05** · And finally just one more thing before we test it. We have to wire everything together. So far this is just the UI. In the last couple of prompts, we implemented the UI side of things and liblocks side of functionality. Just before that, we implemented background tasks through trigger.dev. But now we have to wire it all together. So go ahead and open up 26 design agentfrontend.

**3:33:34** · And as I said, the goal here is really to connect everything together. We are submitting a prompt from the AI sidebar.

**3:33:43** · Then we are tracking the status live through the use realtime run function.

**3:33:49** · We're also showing a status trip while the task runs. And we're letting live blocks handle the updates of the canvas automatically. So let's go ahead and run it. And as soon as it is finished, we're going to test everything together. And in a couple of minutes, definitely much faster than it would take me to do all of this, feature 26 is done. Again, just modify some of the types, modify the config to widen it just a bit.

**3:34:17** · And then most importantly, the major rework happened within the AI sidebar where the handle send now actually pushes the user message to AI chat calls API endpoint to get the run ID and then the token as well to get the public token and then stores both in state.

**3:34:39** · Finally, trigger dev hooks run. We track the run and once it reaches a final status it pushes the final AI message to the AI chat resetting the loading state and clearing the presence. So what do you say that we head back over to localhost 3000 reload the page and you'll see a missing access token in trigger context o or use API client options. We can quickly head back over to just localhost 3000 and editor. It is possible that that's because of this specific project. So I'll create a new project now.

**3:35:11** · I'll call it testing AI designs and create it. And once again, we immediately get the missing access token in trigger o context or use API client options. So there's this handy little copy error info click that you can copy and then you can directly paste the full error right here. when I try to open a specific canvas, this is the error that I get.

**3:35:40** · And then we can just display that error, tell it to analyze it by following the best practices from both liblocks and trigger.dev and provide me your reasoning and idea of what is wrong and how to fix it.

**3:35:56** · So something like this does I notice when you don't ask it to fix it immediately but rather you first ask it to analyze it and give you the idea of what it would do that's not cluttering the context as much and it gives you the ability to say whether you would like it to execute what it suggests or not. So let's see what it comes up with and then we can potentially execute it. And very quickly it was able to figure out the reasoning and I believe it actually applied it because it was just a couple of lines of code.

**3:36:26** · The root cause was that the use real-time run performs an eager validation check for access token on every render and it doesn't wait for a connection attempt. So if we pass empty string, it's the same as if we don't pass it at all. So it immediately throws the error on the first render. But rather we need to wait and only when there's an active run then we need to check for the token. So now if we head back you can see that we can open up a design the new one as well as the old one.

**3:36:57** · So now let's go within the new project we created and we are ready to describe a new system to AI. In this case you can really go ahead and type anything. I'll write something like this. You can also pause your screen and write it with me. But the goal here is to design a high-scale ecommerce back-end architecture including an API gateway, a user service with O, a product catalog service using a NoSQL database, and an order processing system that communicates via a message Q.

**3:37:28** · Also, don't forget to add a Reddis cache for the catalog to handle high traffic. And now we can go ahead and click send.

**3:37:40** · You can see that Ghost AI is analyzing your request in real time right now.

**3:37:46** · I'm going to zoom it in. So this is the first status that we're seeing. It says working right here. And then immediately after we were able to see a completed product. So in this case, we get the API gateway, the user accessing it, browsing different products, placing an order through the product catalog service, and that goes into the message queue. and then the order is actually processed.

**3:38:09** · So this is a great and pretty detailed system architecture diagram and we were able to generate it using AI very quickly because we already had the underlying system for creating different nodes and adding labels within the elements and the edges and then we just created a system that works in the background through trigger.dev dev that makes use of all of those functionalities within the app, generates that JSON, and then we just slap it onto the canvas.

**3:38:39** · So now that everything is working so well, the last missing piece of the puzzle is to generate the specs. We need to take everything that is on the canvas and generate a markdown document that we can then actually feed into a thinking or planning AI agent which is going to make it the strongest possible starting point for starting to develop any kind of an application for real. But the first step is now done.

**3:39:06** · It's all about approaching the architecture from a planning and very detailed way like you are an architect really designing a specification document. So in the next lesson, let's focus on generating that spec.

### AI Spec Generation

**3:39:23** · The flow for generating the spec is almost the same pattern as for generating the design. A trigger route, a background task, and a token route for ownership tracking. Then persistence to versel blob, and finally a piece of UI to then view and download the result.

**3:39:42** · Because we've already built this pattern once, these specs will move faster. So let's go ahead and build it one by one by creating a feature spec number 27 called spec generation flow.md.

**3:39:58** · And yeah, as I told you, the goal of this one is to build the full backend, the trigger route and the trigger.dev task that calls Gemini and then generates a markdown spec. But most importantly, it generates it from the canvas state and the chat history. You can see that right here. Spec generation based on the project ID, room ID, chat history, nodes, and edges. No backend yet. We just wanted to execute that task.

**3:40:29** · So, let's go ahead and run it. 27 spec already. I'm not sure how to feel about it. Is it too high or too low of a number? I mean considering what we've implemented and what we've done so far like a full stack full canvas AI powered application with templates and everything else we've done. I mean I think this would take us months to develop manually.

**3:40:53** · And yeah, now that I think about it, I'm sure 27 spec files is definitely not a lot for this production ready application we've developed so far. We're very close. So, I believe we'll be able to get it done in under 30. Let's make it run. In this case, it looks like it's actually running all three files in parallel.

**3:41:15** · This one was actually pretty quick.

**3:41:17** · Feature 27 is complete. And the only thing we need to check from this one is the trigger task called generate spec.

**3:41:25** · So, let's head over into that file. And you'll notice that it's quite similar to design agent. It takes all the schemas, it builds the context, returns it all, and here's a system prompt saying that we are a Ghost AI senior technical architect whose job is to generate a comprehensive markdown technical specification document based on the provider architecture canvas and the conversation context. And we then give it some information on how to structure the spec. Finally, we call the schema task coming from trigger.

**3:41:56** · Give it an ID, the schema of what it needs to do, the ability to retry it after specific options, and then what is it actually running? In this case, we're calling the Google generative AI, and asking it to generate the spec, build a context, generate it in text. Again, we have to use 2.5 flash 2.0 is no longer there.

**3:42:21** · And then finally it gets the spec and returns it. Before we go ahead and test it, we have to first implement a couple of functionalities and then wire it to the sidebar. So go ahead and open feature specs and create a unit 28 spec persistence download MD. The goal of this one is to save the generated spec file to versel blob. store the URL in project spec prisma model and then add a secure download route.

**3:42:52** · Basically same Prisma metadata plus the blob content pattern that we used for the canvas autosave.

**3:42:59** · That's how we want to save it. And then finally we want to ensure that it's downloadable through this specific API route. It should authenticate the user, verify the access, verify the spec belongs to that project, and then fetch the file and return it as a downloadable markdown file. Go ahead and open this with your AI agent. As usual, we'll tell it to read the file, update our progress tracker, and then implement it exactly as specified.

**3:43:29** · And while it's doing its job, let's quickly check how the progress tracker is coming along. I mean, we've implemented so many features so far, and all of it is here for future developers within your team or future agents working on the project to check out and then continue developing new features on top of all the architecture decisions, session notes, and more. So, yeah, let's see how it approaches this one. And feature 28 is done.

**3:43:55** · A summary right here is that it added a project spec Prisma model with the ID project ID file path and created that and it's attached to a project. So if we delete it, it's going to be deleted as well. Migrations have already been applied for us. Uh I love agents for doing that automatically. So we don't have to run Prisma generate and migrate on our own.

**3:44:17** · And finally, it updated the generate spec so that after the markdown is generated, it uploads it to a versel blob. so that we can download it later on and this route is responsible for that. So now just before we test it, we need to wire everything together. You know how I like to make sure that these spec files are really only handling one thing at a time. So in 27 we handled the spec generation flow.

**3:44:45** · Then we made it persist by storing it into versel blob and creating a download route. And now finally in 29 spec ui integration.mmd we are going to wire everything together into the specs tab in the AI sidebar through a list of generated specs. We can have multiple a preview model that renders the markdown in case you want to preview it in the browser and finally a download action to download it on your device. So go ahead and run it and let's give it some time to implement it.

**3:45:17** · And let's let it do its thing. And now that feature 29 is fully implemented and the build passes, which is important, we'll soon be ready to test it out. So there's two new backend routes. The first one gets access to all the project specifications for a specific project and then the second one actually creates a downloadable markdown text. and the AI sidebar got updated so we can test it all out.

**3:45:44** · Back within the browser, if you now head over to specs and click generate spec, you'll notice that at least on my end, nothing's happening. On your end, it might be working. Maybe your agent did a bit of a better job, but at least here it's not budging. But thankfully, we are getting some errors right here within the terminal. So, I'll go ahead and copy these errors and tell it when I click the generate spec button, it doesn't do anything. And this is what I see in the terminal.

**3:46:14** · I pasted it and then I'll say analyze it and provide a solution.

**3:46:21** · Refer to trigger.dev and liblock skills if needed and press enter.

**3:46:28** · I find it that sometimes it's great to explicitly mention that it can refer to specific skills if you think it's going to be useful. Yeah, this definitely took some time, but yeah, it says right here just to restart your server. It did some additional changes, but I think after all the changes, it's necessary to just reload it. So, that's what I'm going to do. Back on localhost 3000, it's going to be active.

**3:46:54** · Make sure to reload the page and then head over to specs. Click generate spec.

**3:47:00** · And it is generating. While it is actually generating, you can head over to trigger.dev under runs and you can see generate spec is being executed as we speak. So here you can see a bit more information on exactly what is happening. This is the payload that we sent into it. All the different nodes, all the information about the architecture and more. And it looks like it generated it and returned it. So now if you head back, you'll be able to see a new markdown file that when you click on it, it'll be opened within a markdown previewer right here in the browser.

**3:47:36** · There we go. It's a bit tiny. We can definitely increase its width, but yeah, I mean, take a look at this. this architecture diagram. It was able to generate a pretty hefty technical specification document that outlines this huge system that we can send over to our planning agent and start developing it. Let's test the download functionality as well. I click the button and it opened it up.

**3:47:58** · It's a long file, but if you've been following along with this course, you know that specifications have to be long, especially if you're creating one spec for the entire system. So that's it.

**3:48:13** · That's the full Ghost AI feature set working end to end. So what do you say that we test out the functionalities one more time on two separate screens? At least right now I'm on two separate tabs. So still logged in with the same account, but that should be okay. So I'll say final test and create a new project.

**3:48:34** · That project will immediately show up right here as well after reloading the page. And now we are viewing it from both sides.

**3:48:44** · Both of us are in the same room and you can see my name and cursor pointing to different locations.

**3:48:51** · Of course, if it were some other people right here, you'll be able to see their profiles as well. And as soon as I drag and drop something, you can see that it appears immediately. It also auto zoomed in right here. And we can continue creating the diagram. You can see it happens in real time and that's the beauty of live blocks. What we can do next is test the AI functionalities. So I'll open up the AI window right here.

**3:49:20** · And let's go with something simple and default like design an e-commerce backend. I'll first select all of these by holding the shift key and then remove them. and design that e-commerce backend by sending a new AI chat message. It'll start working on it and very quickly it'll generate the full UI right here and that UI got generated for the other user as well.

**3:49:46** · Finally, we can generate some specs out of it and of course this is happening in the background as a task that is being ran on the trigger.dev dev side of things or specifically we are running an agent in this case Gemini to process something but of course you can run all sorts of different AI agents media processing media generation like there's tons of different use cases for how trigger can be used and we can definitely explore some more of it in one of the upcoming videos but yeah the

**3:50:17** · spec is here we can preview it download it and that's it that is the entire app so in the next lesson Let's get it deployed.

### Deployment

**3:50:30** · Okay, now that the app is complete, before we deploy, we need to switch a few services from development to production. Dev keys are rate limited and aren't meant for real traffic. So, we have to update live blocks, trigger dev, and make sure that every environment variable is set correctly in Versell. Let's start with live blocks.

**3:50:53** · create a new project and call it Ghost AI production or something like that and set the environment to production. Then from the API key section, simply copy the public key, head over into yourv.local and paste it right here. Live public key, you can override the development one or in case you want to keep it, you can just comment it out. But again, make sure to add new production ones right here.

**3:51:23** · Or at least when we are deploying the project on Verscell, you'll have to put these new updated ones. So yeah, let's go ahead and update it. Uh the live blocks public key is going to be this new prod key right here. And also let's generate a secret key, which you can copy and then also override right here.

**3:51:44** · Step two is get the trigger dev production API keys by heading over to the dashboard and then in the top selector right here where it says environment switch it over from development to production. Then from the project settings right here under API keys go ahead and copy the secret key and replace the existing one right here under env.

**3:52:11** · Once again, I will comment out the previous one and just update this one that's going to have prod right here in the middle. And below the API keys, you can head over to general project settings and copy the project ref, which I believe should be the same. So if you duplicate it and override it here, you'll see that one is actually the same. So we can leave it as it is. Now go ahead and copy all of your env. And we have to push our changes.

**3:52:39** · So run git add dot get commit-m finalize the app and prepare it for deployment and then run git push. Then head over to versel click add a new project and just import it from git.

**3:52:57** · Once pushed it should have changes a couple of seconds ago not a couple of hours ago but the reason it says 5 hours here is because we've pushed the changes to our dev branch. So for them to show up on Versell, we first have to push them over to the main branch by creating a new PR.

**3:53:16** · And in this case, there were so many changes that we've done, most of which are actually agent skills that we installed. So there's going to be 1.7 million lines of code to review. In this case, what I'm going to do just to get it deployed is I will first fix the conflict we have with Copilot. I'll just tell it to completely remove the current issues.m MD file, which should fix the conflict. Obviously, that's because we're hoping not to have any more issues.

**3:53:47** · It's going to look into it and start implementing it right away. And as soon as it has been removed, we're ready to merge the PR, which means that the latest changes under the Ghost AI project should be reflected momentarily.

**3:54:01** · And after a reload, they'd say just now.

**3:54:05** · So we can go ahead and import it and immediately add the environment variables by pasting all of them into this first key and value pair and it'll automatically populate all of them. So go ahead and scroll down and click deploy. Now we've implemented so many individual features within this application, integrated and wired up so many services across front end and backend and Prisma databases.

**3:54:32** · It would be a miracle if it worked first try. So just as I said that in about 8 seconds the initial build failed saying that we can find a full log right here.

**3:54:43** · So I'll go ahead and inspect the deployment and it looks like it just failed on running mpm install. So typically when we face an error this early with the mpm install most likely culprit is going to be the package lock json.

**3:54:58** · So what I like to do in this situation is just make sure that we are on the main branch and we are and we want to delete the package lock JSON entirely and then push to the main without it by running get add dot get commit-m remove package lock JSON and running get push. This is going to push it straight over to main which means that it should automatically re-trigger another deployment.

**3:55:26** · And this time it is building past second 8 successfully installing the dependencies. So this time we've gotten a bit further but it still breaks right here on Prisma. Uh this is a typical procedure whenever you're publishing a NexJS project on Versel with Prisma. You also have to add an additional script to the package JSON.

**3:55:50** · That's going to be right here. Right after lint, go ahead and add a post install script where you can run prisma generate. So once again, you can make that change and push it over to the main branch.

**3:56:08** · As I told you, it's going to be unlikely that the build is going to succeed from the first try as we've been developing this project for so long locally and in development version and now we want to run it in production. But don't worry, we're going to get there. And third times the charm because the status is now ready and we are live.

**3:56:26** · So go to the project overview and visit your URL which brings us back to our off and homepage at the same time where after you sign in, you are redirected to an empty project screen or since we already logged in with the same account, you can find all of your previous projects. This means that everything is working exactly as it's supposed to, even on the deployed version of the application. So, congrats.

**3:56:54** · This was a long build and quite a different one from the typical ones where we manually code everything out. So, I want to hear from you. How did you like this new approach? Would you like to dive even deeper within the Agentic course that I'm working on? If so, you can join the wait list. And if you haven't already, also go ahead and download that sixfile context system for agentic development that I prepared for you alongside this video. That way you can use the same system we followed along with this build and implement it with your future builds.

**3:57:27** · And yeah, huge thanks to Trigger for amazing background tasks and AI agent functionalities that they allow you to add to your app. Also, huge thanks to liblocks for allowing us to make our applications interactive.

**3:57:42** · And finally to Clerk for simplifying authentication and user management.

**3:57:47** · Thank you not only for sponsoring this video but for developing such amazing developer tools that I get to share with you guys watching this video. That was it for this one. I'll see you within jsmastery.com or if not there within one of the upcoming videos on the YouTube channel.

**3:58:05** · Once again thank you for watching and have a wonderful day.