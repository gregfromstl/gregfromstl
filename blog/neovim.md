# 11 Things I Learned After 12 Months of Neovim

Exactly 12 months ago today, I setup Neovim for the first time. What started as curiosity has since changed the way I write and read code for the better. I thought I'd share why after 12 months I exclusively use and advocate for Neovim over other IDEs.

### 1. Good things take time

The first month with Neovim isn't fun, isn't productive, and most of all isn't easy. Learning an new way of navigating my code was like starting over. The basics of Neovim alone were worth the switch, but it wasn't until I got beyond the basics that the advantages became obvious. Once I learned Vim motions and understood configurations, I could make it my own. I created my own shortcuts, plugins, and built my editor to reflect how I programmed.

The beginning is frustrating and confusing. You want to quit daily. You remember the days of flying through VS Code pointing and clicking wherever you want. You're fumbling around the keyboard trying to remember dozens of shortcuts, all for what? You need to remember why you started. What's over the hill. The amount of control you'll have once you learn to master it.

This isn't specific to Neovim. Any worthwhile skill starts difficult. When we're children, everything's difficult so you perservere. There's no way to go but forward. Once we're adults, we've formed habits and mastered certain things. For the rest of our lives these habits' and skills' momentum pull us in that direction. This is why its so difficult to change careers or learn a new skill. The easy path is to do what you know, but the easy path can only take you in the same direction. Those who learn to choose their own direction control their future. Those who don't let their past control them.

### 2. New doesn't mean better

When people find out I use Neovim the most common reaction is "How long have you been programming for?". The assummption here is I'm a luddite who started with Neovim 20 years ago and never moved on. This couldn't be further from the truth. I used VS Code for most of my career, then switched to Cursor very shortly after release. I was one of their first paying customers, and loved the product (still do). I even used Zed for a bit. I switched to Neovim only after trying every alternative the space had to offer.

Those other IDEs had their advantages, and you could  line them up and compare which one is better. Neovim was different though. When my programming environment is my own, writing code feels like a new activity. I was trying every IDE imaginable thinking the "newest" would be best. An entirely different approach, one that had existed long before I even started programming, was where I finally landed.

### 3. Self-sufficiency is invaluable

There are two types of programmers. When one starts having trouble, they cry for help. They ask other people to solve their problems so they don't need to. The other type dives deeper. They don't want a solution, they want to understand both the solution and the problem. These programmers gain an arsenal of problems they've solved to help them solve future problems.

Neovim puts the controls in my hands. It's raw, configurable, and dependent on my abilities to make it work. When my LSP starts bugging out, I have to roll up my sleeves and figure it out. There's no billion dollar VC-backed startup that cares if my config works. In the moment this is frustrating, but in the long term it forced me into that second group of developers. Whether I liked it or not, I had to become self-sufficient.

Note: I'm not saying don't ask for help. I'm saying don't ask for solutions. Instead, ask for a better understanding. If someone gives me a fix, don't take it at face value. Demand to know why it works. You have both a right and a duty to understand the code you ship.

### 4. Typing speed matters

Once I got the hang of Vim motions, I realized typing speed is a limiting factor on any programming I did. This limit has always been there, but with a mouse-heavy GUI there was nothing I could do to move faster. I could only move a mouse across the screen so fast.

Now that I could not only write but navigate with the keyboard, the only thing slowing me down was typing speed. The difference between 60 and 90 words per minute here is unbelievable. I can now write 50% more code in a day. Scaling my productivity like that wasn't possible when the mouse was the bottleneck.

### 5. AI should work for you

Most new IDEs revolve around AI. Even the plugins for existing IDEs revolve around it. Neovim is no different. There's been an explosion of AI-focused plugins aiming to replicate the experience of products like Cursor. They use the same models, address the same problems, and appear to imitate modern IDEs. There's something different about the AI Neovim plugins, though.

For a while, I wasn't sure why I enjoyed using AI so much more in Neovim than I did in Cursor. Then, after prompting one AI assistant to update the configuration of a second AI assistant, it hit me. I was in control, and I could do anything. There were no limits or assumptions to where agents fit into my workflow. I could tune existing assistants, install a dozen at once, and decide when and how they're used.

Contrast this to Cursor where they've built (quite successfully) a single way to use agents. Yes there are different features within one product, but the UX is the same for everyone. It's not my product, its theirs. Its especially important for me to control my workflow when another intelligence is modifying my code.

### 6. Hobbyists create the cutting edge

The nature of Neovim plugins is different from VS Code's or other IDEs. Hobbyists create most plugins in the Neovim ecosystem, rather than startups or corporations. Their restrictions are fundamentally different. While VS Code or Cursor have to trend towards "one size fits all" solutions, most hobbyists are building something because they think its cool. They can get far more radical in the UX, because they're not invested in mass adoption.

This also means most plugins will have bugs, janky UX, and unexpected hiccups. This is part of the experience (see #3). It's a tradeoff that allows me to see the cutting edge and experience ideas that no VC-backed company would ever build. 

### 7. Great programmers are craftsmen

I've met more great programmers through Neovim than anything else. There's something about the mindset it puts you in that attracts fantastic engineers. Their attitude towards it always reminds me of someone who loves cars. They want to show theirs off, work on it every weekend, and see how far they can push it. They're craftsmen that are so obsessed with their art they've become obsessed with the tools that make it possible.

### 8. Understand one level deeper

When things break, and they often do, no one is coming to save me. This means I need to understand one level deeper than what I'm building or using. I can't take dependencies or tools at face value. I have to understand their intricacies and why they work the way they do. I have both a right and a duty to understand the tools I use.

### 9. Be opinionated

When I'm responsible for your own editor, I make decisions about how things work. I can't take the experience I'm given and accept it for what it is. The ability to change things makes me consider alternatives. I've developed a give and take relationship with the tools I use and a disdain for behaviors I dislike. These opinions provide an opportunity for self-reflection. I understand what works for me, and what I'd rather chew glass than use.

### 10. Take the high road

Many days it would be easier to use a more polished IDE. Features might get shipped faster and bugs fixed sooner in the short term. But looking back over the past 12 months, I've grown more as a developer than in the previous 12 years combined. I enjoy it more and take pride in both the tools I use and the code I write. Many times (but not all times), the more difficult path is the one that shapes you into the best person you can be.

### 11. Explore

None of this would have happened had I not tried something new. Your outputs are a manifestation of all inputs you've accumulated over the years. The more things you've tried and skills you've mastered, the more informed your outputs are. So explore new things. Try anything that interests you. Make time for learning and cherish experimentation. Don't let momentum push you down the same road your whole life.

Long live `init.lua`
