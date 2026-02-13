# LightningLab2
Using Claude to reinforce good programming and to help understand the code, not just fixing it

## Explanation
[Paste description here]

## Step 1: Install
For windows, run this in Powershell
```
irm https://claude.ai/install.ps1 | iex
```

Once installed, you can use ```claude``` in any terminal to start logging in (Need Pro)

## Project Context
When you define what you want in the project, you can add context to the Claude.md file
This will be read for every request.
What do you want to put here?

Claude can help you make it
```
I want to create a skill that helps me write better MVVM 
ViewModels for my Starcraft bot app. It should remind me 
to use CommunityToolkit.Mvvm, follow proper property naming, 
and implement INotifyPropertyChanged correctly.
```

Keep the file smaller than 500 words. If you need more, you need to create skills

## Mentor Skill
Skills are like the overall context, but you can specify certain instructions to use. This can be a quick skill to format a page in a certain pattern, or you can use it to help your learning.

In this case, we want to use the skill to have claude act as a mentor when giving responses, asking us questions and clarifying problems as we code.

```
Create a custom Claude skill for me that acts as a senior software engineer mentor. 

The skill should:
- Focus on teaching concepts, not just providing solutions
- Ask guiding questions to help me discover answers
- Explain the "why" behind solutions, not just the "how"
- Share real-world context and best practices
- Adjust teaching style based on my level of understanding
- Encourage good coding habits

Specific behaviors:
- When I ask about a bug, help me debug it rather than just fixing it
- When I ask about patterns (like MVVM), explain the principles first
- When I paste code for review, point out learning opportunities
- When I'm stuck, ask diagnostic questions before giving answers

Context: I'm a student learning .NET MAUI development, working on a Starcraft bot controller app using MVVM patterns and BWAPI integration.

The skill should trigger whenever I:
- Ask coding questions
- Request code reviews
- Say "explain", "teach me", or "help me understand"
- Show code with issues
- Ask "why" or "how" questions
```

After the skill is created, you will have to ```/exit``` and open claude again

## Compare Responses
Ask question with and without the ```/mentor``` skill (or whatever you named it). Does it help you understand what you are doing? Can you customize the prompt to match your style?

Think of other skills that you could create for different subjects or projects.
MVVM Pattern checker skill?
API Error Handler?
Unit Test Helper?
