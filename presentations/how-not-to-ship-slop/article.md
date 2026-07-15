# AI Doesn't Ship Slop. You Do.

*How to keep the model's average out of your work.*

I can usually tell within a few seconds. A landing page loads and it's a centered headline over a soft purple gradient, three feature cards with rounded corners, a testimonial from a person who may or may not exist. Or I'm reading a blog post and the first paragraph tells me what the post is going to tell me, and the last paragraph tells me what the post just told me, and the middle is a tidy list where every item is exactly the same length. Nothing is wrong with any of it. That's the problem. It's the writing and design equivalent of elevator music: technically competent, instantly forgettable, and clearly made by someone who didn't care whether you remembered it.

We have a word for this now. Merriam-Webster made "slop" its Word of the Year for 2025, defining it as low-quality digital content produced in quantity by AI. The word stuck because everyone already knew the feeling. You can smell it before you can explain it.

I want to make an argument that sounds like a dodge but isn't: the AI is not the thing producing slop. You are. The model is just very good at giving you exactly what you asked for when you didn't actually ask for anything. Slop is a workflow failure wearing a technology costume. And once you see it that way, avoiding it stops being a vague aspiration ("use AI responsibly") and becomes a short list of concrete habits you can actually practice.

## What slop actually is

The lazy definition of slop is "content made by AI." That definition is useless, because plenty of good work now has AI somewhere in its production, and plenty of pure handmade work is slop. I've read human-written corporate blog posts that were sloppier than anything a model would produce.

A better definition: slop is content optimized for the moment of production rather than the moment of reception. It's made to exist, not to be read or used. The giveaway is always an absence. There's no specific person behind it, no stake, no point of view, no detail that could only have come from someone who was actually there. It's the median of everything that has ever been written or designed about the topic, and the median, by definition, is the part nobody remembers.

That last point is the whole game, so let me sit on it. A language model is a machine for producing the most probable next token. A diffusion model is a machine for producing the most probable next pixel. "Most probable," averaged across the entire internet, means "most average." When you give a model a thin prompt, you are explicitly asking for the center of the distribution. You're asking for the thing that is true of all SaaS landing pages and specific to none of them. The model obliges, instantly, and at infinite scale. That's not a bug you can prompt your way around with the right magic words. It's the default behavior of the tool, and the default is slop.

Which means the entire job of avoiding slop is the job of dragging your output away from that center. Everything below is a way of doing that.

## The three things the model can't give you

There are exactly three things a model cannot supply on its own, and slop is what you get when all three are missing: context, taste, and an owner.

Context is the raw material. The specific facts, the real data, the actual transcript, the thing that happened to you on Tuesday. The model doesn't have your context unless you hand it over, so without it the model reaches for the generic version of your topic.

Taste is judgment about what's good. The model has read everything but prefers nothing. It will write the cliché and the fresh line with equal enthusiasm and no idea which is which. Taste is the thing that says "no, not that, the other one."

An owner is a human being who will defend every word and every pixel. Not "approve." Defend. The defining feature of slop is that if you asked the person who shipped it to justify a particular sentence, they couldn't, because no one ever decided it on purpose. It was simply the thing that came out.

Hold onto those three. The rest of this is application.

## Not shipping slop when you write

Start with input, because it's the highest-leverage thing and almost everyone gets it wrong. Most people prompt a model with a topic: "write a post about onboarding." A topic is an invitation to the median. The model has no choice but to give you the average post about onboarding, because that's all "the topic of onboarding" contains.

Instead, generate from material. Give it the actual onboarding flow, the support tickets, the three things that surprised you, the number that made you angry. The difference in output is not subtle. With a topic you get a Wikipedia summary of received wisdom. With material you get something that could only have been written about your specific situation. The quality of anything a model writes is capped by the quality of what you put in, and a topic is nearly nothing.

The second habit is to decide the point before you generate. A model cannot have an opinion you haven't given it, and it will never tell you that you don't have one. It'll happily manufacture a confident, balanced, opinion-shaped paragraph that says nothing. So do the hard part yourself: what's the actual claim, the thing you believe that not everyone agrees with, the "so what" a reader should leave with? Figure that out first, then use the model to express it. Using the model to find your opinion is how you end up publishing the absence of one.

Then there's specificity, which is the single most reliable tell that separates real writing from slop. Slop is abstract and universally applicable. It speaks in "businesses today" and "in an ever-evolving landscape" and "leveraging cutting-edge solutions." Real writing is specific and falsifiable. It names the company, the number, the date, the actual quote. My favorite test while editing: take any sentence and ask whether it could appear, word for word, on a competitor's page. If it could, it isn't doing any work. Cut it or make it specific.

Once you have a draft, edit destructively, and edit the beginning and end hardest. Openings and closings are where slop concentrates, because models love to warm up and then summarize. The intro that announces what the piece will cover, the conclusion that restates what it just covered: both can usually be deleted outright. Start where the actual idea starts. End on the sharpest thing, not the tidiest. While you're in there, kill the tells. The rule-of-three lists where everything comes in triplets. The "it's not just X, it's Y" construction the model reaches for whenever it wants to sound profound. The hedging. And yes, the em-dashes, which models pour in so liberally that their presence has become a running joke and a minor moral panic. You'll notice there isn't a single one in this entire piece. That was a small act of discipline and a slightly petty point, because the tell was never any one tic. It's the accumulation. It's the smell of no one having made a choice.

Last, the cheapest and most effective check I know: read it out loud. Anything you would not actually say to a colleague over coffee is slop, and your mouth will catch it before your eyes do. The AI register, that smooth over-formal helpfulness, falls apart the second you try to speak it like a person.

## Not shipping slop when you design

The same logic governs anything visual, just with different defaults. The design model's center of the distribution is by now so familiar it's a meme: Inter or some other system font, a purple or blue gradient, a hero section with centered text, a row of three feature cards with little icons, a testimonial carousel, a footer with four columns of links. None of it is bad. All of it is the average. If you don't actively specify otherwise, that's what you'll get, because that's what the model has seen ten million times.

So the first habit mirrors the writing one: constrain before you generate. Decide typography, color, layout, and motion deliberately, as separate choices, rather than asking for a "modern, clean design" and accepting whatever appears. "Modern" and "clean" are slop words. Every product on earth claims them, which means they constrain nothing, which means you've just asked for the median again.

The most underused trick in visual prompting is the negative constraint. Tell the tool what not to do. "No Inter. No centered hero. No purple gradient. No card grid." Negatives are powerful because they specifically subtract the defaults the model would otherwise reach for, and they force it to find something less obvious. Anthropic's own guidance on this, in their cookbook on frontend aesthetics, has a name for the underlying problem: distributional convergence. The model converges on the safe center unless you explicitly push it off. Naming what to avoid is how you push.

Then, instead of adjectives, give a reference with an actual point of view. Not "make it sleek" but "take the palette from this IDE theme" or "lay it out like an editorial magazine spread, long column with pull quotes, not a marketing page." A real reference carries a thousand decisions the model can borrow. An adjective carries none.

And the design equivalent of the read-aloud test is the lineup. Put your screen next to three competitors. If a stranger couldn't tell which one is yours, you've shipped slop, regardless of how polished each individual pixel is. Distinctiveness, not polish, is the thing slop lacks. Polish it has in abundance. That's exactly why it's so easy to wave through review.

## The shift that actually matters

Here's the deeper change underneath all of this, and it's the part I'd want a room of people to leave thinking about.

For most of the history of making things, production was the bottleneck. Writing the words, pushing the pixels, building the thing took real time, and so the scarce, valuable skill was the ability to produce at all. AI obliterated that bottleneck. Producing is now nearly free and nearly instant. Which means the scarce skill has moved. It's no longer production. It's judgment: knowing what's worth making, and being able to tell the good version from the average one. Taste was always valuable. Now it's the whole job.

The trap, the thing that generates 90% of the slop in the world, is to take the speed and spend it on volume. The tool let you make ten times as much, so you make ten times as much. This is exactly backwards. The right move is to take the speed and spend it on quality: make fewer things, or make the same thing five times until it's actually good. Slop is, economically, a quantity play. The antidote is to refuse to play that game and compete on the axis the machine can't, which is whether anyone gives a damn.

In practice that comes down to a few unglamorous disciplines. Every artifact needs one accountable human owner, a specific person who can defend every choice in it, because "no one really decided this" is the precise definition of what we're trying to avoid. Your taste should be written down where the tool can use it, a voice guide, a design system, a folder of good-versus-bad examples, so that "good" is a thing the model can be pointed at rather than a thing you hope it stumbles into. And there should always be a last-mile human pass on anything that ships, with the most attention on the parts that face other people: the claims, the opening, the closing, the cover image, the gut-check of whether you'd put your name on it.

## The honest counterpoint

I should argue against myself, because the anti-slop position curdles fast into something obnoxious.

There's a moral panic forming around AI tells, and it's getting silly. People now treat an em-dash like a confession. They run text through "detectors" that are barely better than coin flips and accuse students and coworkers of cheating based on the output. Good writers have used em-dashes and the word "delve" for centuries, and a tic is not a crime. If you take "avoid slop" and turn it into a witch hunt for stylistic fingerprints, you've missed the point entirely. The problem was never the em-dash. The problem was the absence of a person. Plenty of slop has no em-dashes at all.

It's also worth saying that good-enough is sometimes genuinely good enough. Not everything needs to be a singular artifact. The internal status update, the throwaway utility, the first draft nobody but you will read: ship the average version, save your taste for where it counts, and don't moralize about it. Caring about everything equally is its own kind of failure. The skill is knowing which things deserve the full treatment and which things just need to exist.

And the tools are not the enemy. I use them constantly. This very piece passed through a model more than once. The point is never to prove your purity by avoiding AI. The point is to stay in charge of it, to make it produce your work faster instead of replacing your work with the average of everyone else's.

## What's left when production is free

If the model can produce infinite competent, forgettable, average work for free, then competent-and-average is worth roughly nothing now. It's the new baseline, the floor, the thing everyone has. The only things that retain value are the things the average doesn't have: a real point of view, specific knowledge, genuine taste, and a person willing to stand behind the result.

That's not a constraint to mourn. It's the most interesting development in creative work in a long time. The boring middle just got automated away, and what's left is precisely the part that was always the point. The machine will give you the average of everything forever, at no cost, on demand. Your only job, the entire job, is to be the part it can't be.
