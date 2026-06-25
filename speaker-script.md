# How to not ship slop

## Just stop being average

At this point, everyone knows what "AI Slop" is. You've probably seen it on websites—titles surrounded by emoji eyelines, or badges with blinking dots. And who could forget the AI-generated photos, like the infamous crayfish Jesus or people with duplicate fingers? The same applies to copy; blog posts and articles are often filled with too many em-dashes and repetitive phrasing. It's everywhere, and it's easy to spot. However, there is a way to avoid this by following the right principles, which is what I'm going to talk about today.

My name is Perttu, and I'm a Developer Advocate at RevenueCat. My job is to help developers make more money. For those who aren't familiar with the role, being a Developer Advocate means I produce a lot of content—articles, videos, and conference talks. I also organize events; for instance, we're launching the world's largest mobile hackathon next month, which will run for two months. Because my job essentially involves being an engineer who does marketing, I use AI extensively. In fact, we use AI quite a lot at RevenueCat as well.

Using a lot of AI has the risk of producing a lot of AI slop, so today I’m going to talk about some of the rules, insights and principles around not making slop. My job is to produce content, so that means articles, videos, talks, and code. I’ve tried to make this presentation to touch a little bit on all of those. However on code I mostly focus on the UI aspects of AI written code.

So let’s get started

## My background on this topic 

To give you a little bit of background, how much AI we use at RevenueCat. Earlier this year we posted a job offering for an agentic developer advocate — meaning we were hiring an AI to produce articles, videos, and materials for developers.

Now you might think that this was a joke job posting, and our customers know that we have a tendency to do some quite silly things, but we always do them seriously. So the job, and the 10k a month salary were completely real, and we actually had a lot of agents applying for it.

Close to 100 actually, all of which me and my colleagues went through. And by going through I mean we looked at their output. You see in our job applications we had asked the agents to do three things:

* Make use of one of our new APIs by building something interesting around, for example a demo that would allow developers to see revenue insights  
* Make an article explaining the API, how the project was created, and writing it in a form that looks like RevenueCat technical article   
* Based on the two of these, make a short video for YouTube, showing the demo and explaining how it works from the tech perspective

All the candidates produced those, so there was quite a lot of stuff to go through. 

### Evaluate AI like you would evaluate human skills 

Some of the demos were actually quite impressive, but every agent failed on doing all three things well. And this is not because there was something wrong with the models, or that the instructions were too complicated, or that the task was too much. No, all the agents just produced very average results. 

And that is what AI slop is, it’s average. The default weights in the models are just averages. Without heavily weighted inputs, everything we produce with AI will converge towards the mean. 

So to not ship slop, is to not ship average.

Average, in our industry is something that kills companies. That is why at RevenueCat our hiring no-yes matrix has four grades

* Definitely no  
* No  
* Yes  
* Definitely yes

Adding a fifth option would lead to people in interviews giving that scale more often and that’s not what we want. Internally we even avoid giving the “yes” option. Because yes, is often a soft no. So instead we scale our reviews of candidates, from the Definitely yes, which also translates to “I would fight to have this person join the company”. When you think of it like that, you tend to make way better hiring decisions.

And that’s how you should approach AI content as well: if you wouldn’t fight for it, don’t ship it. 

Now getting to that stage with AI feels almost impossible, so let's look at how to actually do that.

## How to define AI slop

Let’s really quickly define AI slop, because not everything AI creates is slop. A simple way to put it would be to call it digital pollution, but Kommers et al define it pretty nicely in a paper titled [***Why slop matters***](https://dl.acm.org/doi/10.1145/3786777) by identifying three key features of AI slop:

1. **Superficial competence**   
   It looks well made, but it lacks real depth.  
2. **Asymmetric effort**   
   It takes much less effort to make than it would without AI  
3. **Mass producibility**   
   It can be produced in large quantities and shared widely online.

For our jobs as designers, engineers, and product people, the first two points are the ones we should pay attention to. A slide deck we produce with Claude for a client, is not for sharing online and producing in large quantities; but for a client it will come across as slop because of the superficial competence and the asymmetric effort.

Those two things are also the things that erode trust. When a customer is looking at your AI generated slide deck, and catches a weird statement from it. You telling them that it is an “AI hallucination” they will think:

“Huh, the slides looked good but now the whole content is questionable. And this level of quality in the slides is not actually their default level.”

## Three things AI can’t give you

AI slop is very easy to notice but knowing what leads to it is not as easy. You either have to know how LLMs work, or have a lot of experience tweaking the stuff you get out of LLMs. Instead of going down a rabbit hole of trying to understand LLMs better, I’m now just going to tell you what three things models can’t give you:

1. Context  
2. Taste  
3. Ownership

I’ll go through all of these in detail next, so 

**Context**  
After a model has been trained, the only way you can affect it is by giving it context. Generally the better context you give as a prompt, the better the output it is. Context is something that has to come from you 

**Taste**  
Context gets you something accurate. Taste is what makes it good.  
Here's the thing the model can't do: it can't tell the difference between the average version and the great one. It'll write you a cliché and a sharp, original line with exactly the same confidence, and it has no idea which is which. It has read everything and it prefers nothing.

My background is in cognitive neuroscience. Before I built mobile apps I worked in a human-computer interaction lab, where we tried to model how designers actually make decisions. The short version of what I learned: taste isn't magic. It's pattern recognition you build by looking at a lot of good work and getting told, often, when yours is average.

Go back to those \~100 agent applications. Every model could build the demo, write the article, and cut the video. All competent. Not one could make a choice: what to leave out, which single insight was worth the developer's time, where to stop. That editorial judgment is taste, and it was the exact thing missing from every one of them.

So when AI hands you twenty options, remember it can generate the twenty but it can't tell you which one to ship. That part is yours. Outsource it and you ship the mean.  
One practical tell: taste usually shows up as subtraction. The model adds. It pads, it hedges, it gives you the intro that explains what the intro is about. Taste is mostly knowing what to cut.

**Ownership**  
Making things faster or easier is not the same as making things better.  
That gap is where ownership lives. The model already gave you something approvable. That's what superficial competence means: it clears the bar at a glance. Ownership is different. Ownership is being willing to put your name on it and argue for it.

The clearest sign that nobody owned something is the sentence "oh, that's just an AI hallucination." The moment you say that to a client, you've told them the truth: no human actually stood behind this. And it's not just that one line that's now in question. It's everything. They assume the polished thing was never really your bar.

Here's the test, and it's the same one we use for hiring: would you fight for it? Not "is it fine." Not "would I approve it." Would you go to bat for this, defend every claim, every frame, every pixel? If the answer's no, you don't have an owner yet, and without an owner you've got slop, however good it looks.

In practice, ownership is unglamorous. It's reading every line. It's checking every number, especially the customer-facing ones. It's the last-mile pass you can't hand back to the machine, because the one thing that can't be generated is a person whose reputation is on the line.

## Guidelines for not generating slop 

### How to talk to AI 

I’ve worked in consulting, you work in consulting. Clients often have a certain way of speaking like:

* Can you make this more white?  
* The app is broken  
* Can you make the design pop more?

You know who also talks like this:  
\[show codex with the same text\]

You\! Stop talking to AI like a client\! 

Always be specific, that is literally your job. 

In addition to the expertise you have, your job is often to apply context, taste and ownership to turn ambiguous client requirements into an actual thing.
### Show it what good looks like

Adjectives are slop fuel. "Make it professional," "clean," "modern," "make the copy pop" all ask for the average, because each one describes ten million things at once. The fix is the one you'd use with a junior: don't describe good, show good.

So keep a swipe file. For writing, that's two or three of your best pieces plus a style guide the model can match, then "write it in this voice," not "make it engaging." You can bake this in permanently by setting a custom Claude style or custom instructions, so everything starts closer to you instead of closer to the mean.

> [demo: same brief twice. Once "write a launch post about [feature]." Once "write it in this voice: [paste 200 words of your own writing]." Read both out loud and let the room hear the gap.]

For anything visual the same rule applies, and Anthropic's own frontend cookbook spells out how. Don't say "modern and clean." Name the dimensions, point at real references, and call out what to avoid:

> Typography: pick something with a point of view (Playfair Display, JetBrains Mono, Bricolage Grotesque, Clash Display). Never Inter or Roboto.
> Color: one dominant color with sharp accents, not a timid even palette. Draw from an IDE theme or a real cultural reference.
> Motion: one well-orchestrated page load with staggered reveals beats a dozen scattered micro-interactions.
> Avoid: Inter, purple gradients on white, the predictable hero-plus-three-cards layout.

The whole move in one line: reference, don't adjective.

### Cut until it bleeds

The model's superpower is adding. Yours is taking away. Every first draft it hands you is about a third too long and far too smooth, and the smoothness is the slop.

The good news: the tells are so consistent that Wikipedia editors keep a page called "Signs of AI writing" just to catch them. Learn the five families and you'll see them everywhere:

1. **Significance inflation.** Everything is "pivotal," "crucial," "a testament to," "marks a turning point," "underscores."
2. **The vocabulary fingerprint.** "Delve," "tapestry," "intricate," "additionally," "fundamental." Where there's one, there are more.
3. **Structure tells.** Title Case Headings, bolding every other phrase, the inline-header list, curly quotes, and em-dashes three to a paragraph.
4. **Sycophancy residue.** "Great question!", "I hope this helps!", "As of my last training update."
5. **Avoidance patterns.** Dodging a plain "is" or "are," everything in threes, "not just X, but Y," synonym-cycling, and a closing paragraph of vague optimism ("the future looks bright").

Here's one in the wild. An AI wrote this about a government statistics office:

> "The Statistical Institute of Catalonia was officially established in 1989, marking a pivotal moment in the evolution of regional statistics in Spain."

A statistics office, made to sound like the signing of the Magna Carta. A human writes:

> "The Statistical Institute of Catalonia was established in 1989 to collect regional statistics independently from Spain's national office."

Same facts, no inflation.

> [demo: put a real AI draft on screen and edit it live. Strike the tells. Watch it get shorter and better in front of everyone.]

One warning, and it's the important one. Scrubbing the tells is not the finish line. If you only delete, you get writing that's clean and completely lifeless, technically passable and totally forgettable. You have to put something back: your voice, an opinion, a tangent, an admission that you're not sure. "Remote work has several advantages" is dead on arrival. "I was a remote-work skeptic for years, and I was mostly wrong" is a person. Cutting removes the robot. Only you can add the human.

The cheapest check there is: read it out loud. If you wouldn't say it to a colleague over coffee, it's slop.

### Don't accept the default look

This is the code part I promised, the UI specifically. Designers have a name for what AI does here: distributional convergence. Ask any model for an interface and it drifts to the exact same place: Inter, a purple-to-blue gradient, an oversized hero with a vague headline, three feature cards with identical 16px corners, a stock photo of people smiling at a laptop, and no real motion. It's competent, and it's why five SaaS sites now look like siblings.

The vague headline is the easiest tell to catch. "Build the future of work" could belong to anyone. Compare the real ones: Stripe says "Financial infrastructure for the internet." Linear says "Plan and build products." Specific beats aspirational every time, which is the exact same rule from the writing half of this talk.

To pull a UI off the mean, guide it on four dimensions on purpose (straight from the frontend cookbook):

* **Typography:** swap Inter for something that means something. Stripe uses a bespoke serif, Vercel commissioned Geist, Linear uses custom type. Pick one display font with a point of view.
* **Color:** use it semantically, not decoratively. A gradient is what you reach for when the color carries no meaning. Define real tokens (action, success, warning), not "gradient-start."
* **Imagery:** replace every stock photo and floating 3D blob with real product screenshots or real people. Specificity reads as trust.
* **Motion:** one orchestrated page load with staggered reveals beats a dozen random fade-ins. Motion should signal state or direct attention, never just decorate.

Then anchor all of it to a system you actually own, because the defaults creep back the moment you spin up a new page. Build the brand into a component library and CSS variables once, so every new page starts distinctive instead of generic.

> [demo: the cookbook's own before/after. "Build a SaaS landing page" with no guidance, then the same prompt with the aesthetics prompt added. Side by side, the room sees the slop and the not-slop instantly.]

And the test before you ship: the lineup. Put your screen next to three real competitors. If a stranger can't pick out which one is yours, you shipped the default.

### Verify it, then fight for it

Ownership turns into a checklist at the very end. The model is confidently wrong, and confident-wrong is the expensive kind. So before anything leaves your hands:

* Check every number, name, quote, and API method against a real source. Double for anything a customer will see.
* For code, run it and read it. Don't just accept the diff. AI code reliably ships with more bugs and security holes than you'd guess, so "it ran once" is not the bar.
* For a deck, make sure you can defend every slide.

Then the gate, the same one we use for hiring: would you fight for it? Not "is it fine." If you wouldn't go to bat for it in front of this room, it isn't done.

> [your example: a time AI invented a stat or an API method that doesn't exist, and you caught it on the last pass. A screenshot lands even harder.]

## Don't ship average

So that's the whole thing. Slop is just average wearing a nice font, and the models serve you average by default, because average is literally what they were built to produce. Everything I've shown you today is the same two-step: cut the average out, then put yourself back in.

Context, taste, and ownership are how you do that. Context is what only you can feed it. Taste is knowing which of its twenty answers is the good one, and what to cut from the one you keep. Ownership is being willing to put your name on the result and defend it. The model has none of these, and it never will. That isn't a limitation to wait out. It's the job.

And here's the part worth sitting with. A year ago, knowing how to use these tools was an edge. It isn't anymore. Everyone in this room has the same models, the same prompts, the same Codex open in another window. When the tools are identical, the only thing left to compete on is the stuff the tool can't give you. Which means taste and ownership just went from nice-to-have to the entire game.

So the next time you're about to ship the thing the AI made for you, ask the one question that matters: would you fight for it?

If yes, ship it. If not, you already know what it is.

Thanks.

> [Q&A / contact slide: name, handle, where to find your work]

---

### Sources / further reading

* "You Sound Like ChatGPT," Alex Banks, The Signal. The five families of AI tells.
* "Signs of AI writing," Wikipedia. The catalogue The Signal draws from.
* "AI Slop Web Design," 925studios. Distributional convergence, the default look, the fixes.
* "Prompting for frontend aesthetics," Anthropic Claude cookbook. The four-dimension visual guidance.
* "Why Slop Matters," Kommers et al. Superficial competence, asymmetric effort, mass producibility.
