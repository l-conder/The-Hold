# The Hold

The Hold is an AI mentor for solo freelancers facing a client message that asks for more than was agreed.

It is built for one narrow moment: the freelancer knows the request is outside scope, the client matters, and the cursor is blinking. The mentor helps them slow down, separate the client's urgency from their own decision, name the fear underneath the impulse to say yes, and choose a response they can stand behind.

This is not a knowledge base. It does not teach freelance operations in general. It coaches the person in front of it.

## What It Does

The Hold helps you pause before responding to a client-pressure message.

It walks you through three questions:

1. What was actually agreed?
2. What exactly is being asked now?
3. What are you afraid will happen if you hold the line?

Only after the fear is named does the mentor help shape language.

## How to Use

Drop this folder into a Claude project.

In the Claude Project instructions, use:

```text
You are The Hold. Read `identity.md` for who you are, follow `rules.md` for how you coach, use `examples.md` as behavior models, and consult `reference/` only when it helps the user in the moment.

Do not act like a knowledge base. Coach the freelancer through the client-pressure moment. Do not give wording before the user names a specific fear.
```

Then start with a real scenario:

```text
A client just sent me this:

[paste the message]

Here is what we agreed to:

[briefly describe the agreement]

Help me figure out how to respond.
```

The mentor will not immediately write the reply. That is intentional.

## Folder Map

- `identity.md`: who the mentor is and who it serves
- `rules.md`: how the mentor behaves in conversation
- `examples.md`: model interactions showing what good coaching looks like
- `reference/`: frameworks, drills, patterns, and case files
- `index.html`: single-page site with ElevenLabs voice mentor embed
- `elevenlabs/agent-config.md`: dashboard-ready voice agent configuration

## Quick Test

After adding the folder to Claude, paste this:

```text
My client just wrote: "Can you also clean up the mobile layout before tomorrow's stakeholder review? Should be quick since the page is already built."

We agreed to a desktop prototype by Friday. Mobile was phase two.

Help me respond.
```

A good run does not start by writing the reply. It should first ask what was agreed, identify the new request and pressure language, ask what you are afraid will happen if you hold the line, then help shape the response.

## Best Fit

Use The Hold when:

- A freelance client asks for extra work, faster turnaround, or informal support outside the agreement.
- The relationship is still basically good-faith.
- The freelancer feels pressure to answer quickly.
- The freelancer wants help deciding and wording a response.

Do not use The Hold for:

- Legal disputes.
- Contract drafting.
- Harassment, threats, or abusive client behavior.
- Agency teams with internal approval chains.
- General freelance strategy.

## The Core Rule

No scripts before the fear.

Words offered too early usually get used from inside the same fear that caused the problem. The mentor's job is to hold the freelancer in the moment long enough for the real issue to surface.

Once the fear is named, the response usually becomes simpler: acknowledge the client, name the extra work as separate, and offer the next clean step.

## Voice Mentor

The site includes an embedded ElevenLabs voice mentor.

To recreate or tune the voice agent, use:

```text
elevenlabs/agent-config.md
```

The embedded agent is designed to open with:

```text
Tell me what happened.
```

Then it follows the same coaching rule as the Claude folder: no scripts before the fear.
