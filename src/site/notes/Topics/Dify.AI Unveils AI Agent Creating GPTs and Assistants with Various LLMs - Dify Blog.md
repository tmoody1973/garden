---
{"dg-publish":true,"permalink":"/topics/dify-ai-unveils-ai-agent-creating-gp-ts-and-assistants-with-various-ll-ms-dify-blog/"}
---


Humans are capable of solving complex problems. This process involves understanding information, figuring out what steps to take, making choices, using tools, and then seeing what happens and deciding what to do next. Now we know LLMs are really good at understanding and processing language, which makes us pretty excited about how they could be used to help people tackle real-world problems.

Previously, OpenAI came up with something called GPTs and Assistants API, which let us play around with AI assistants using OpenAI's models. It really got our creative juices flowing. **Now, Dify is taking it a step further by letting you use just about any of the big-name LLMs out there, along with a variety of tools to create these smart AI Agents.**

## What Sets It Apart from OpenAI Assistants API?

OpenAI Assistants API lets developers create advanced AI Assistants using OpenAI's models. Meanwhile, Dify, an LLM app development platform that's big on openness, supports all sorts of LLMs, including those that are open-source. This means you're not just stuck with OpenAI's models; you've got a wider range to choose from for different AI Agents.

What's cool about Dify being open-source is that you can set it up right in your workplace. This makes adding AI smarts to your current business stuff super straightforward, even turning your own APIs into handy tools you can use in real-time. This is a big deal for businesses that really need to keep their data under wraps. We go into this in more detail in our article "[Dify.AI: Open-source Assistants API based on any LLM](https://dify.ai/blog/openai-assistants-api-vs-dify-self-hosting-flexible-ai-solutions)."

![](https://framerusercontent.com/images/5C4Rq4DKkZWXSxnrA38SxAYQs9w.png)

## What is an AI Agent?

We're excited about the idea of AI Agent emulating how we humans think and solve problems, step by step, to come up with a final solution. **In Dify, the AI Agent using a '**[**Chain-of-Thought**](https://arxiv.org/pdf/2201.11903.pdf)**' reasoning method. It means these agents can think things through gradually to solve problems. And the cool part? You can create one quickly using a user-friendly visual interface.**

For example, let's say we ask, "How old is Trump's wife now?" Currently, an LLM doesn't have the ability to give her current age from its own database. But don't worry, we have a couple of effective tools to help: 'Wikipedia\_search' and 'current\_time'. Here's the step-by-step breakdown of how it tackles the question:

1. First up, it uses 'Wikipedia\_search' to dig up Melania Trump's birth year. She was born on April 26, 1970.
2. Then, it uses 'current\_time' to pin down today's date, which is January 21, 2024.
3. And finally, it crunches the numbers to figure out Melania Trump's age right now: 53 years old.

![](https://framerusercontent.com/images/KwrZrvWne3LVNASdYxUGQlK9M4.png)

## How to Achieve Agent Reasoning with Various LLMs?

To make these AI Agents smart, you need a solid base model for reasoning. That's where LLMs come in, with CoT (Chain of Thought) reasoning capabilities. Different model providers support different ways of making these models think, like '[Function calling](https://platform.openai.com/docs/guides/function-calling/function-calling)' and 'ReAct.' Those that use Function Calling usually work better.

Right now, models from OpenAI, ChatGLM, Tongyi, MiniMax, and ERNIE Bot support this Function calling feature.For model series that do not yet support Function Calling, we provide a universal ReAct method for invocation.

![](https://framerusercontent.com/images/ahVwoFUGXRCMxseyTSUtpkPw.png)

## What Tools are Available to AI Agents Now?

For an AI agent, having the right set of tools is crucial. These tools aren't just bells and whistles; they provide extra knowledge and skills, which are essential for the AI to think things through.

In this version, we're not just relying on the usual knowledge base that the AI can call upon. We've also got 11 super handy tools lined up:

1. Google Search: This is like AI's gateway to Google. It lets the AI perform searches and pull out bits of info and web pages.
2. DALL·E: This is an artistic aid from OpenAI. The AI can use it to create images from your text descriptions.
3. Vectorizer.AI: A quick fix for turning PNG and JPG images into SVG vector graphics.
4. Chart Generator: Perfect for when the AI needs to whip up visual charts - be it bar, line, or pie charts.
5. Web Scraper: It's a tool that makes it easy to automatically grab text, images, and links from websites.
6. Wolfram Alpha: Think of this as the AI's go-to for solving tricky math, analyzing data, or digging up historical info.
7. Youtube: For when the AI needs the scoop on YouTube video stats.
8. Stable Diffusion: Another creative tool for the AI to turn text descriptions into images.
9. Yahoo Finance: The AI's resource for real-time finance and stock news.
10. Wikipedia: The AI's way of diving into Wikipedia for quick snippets and info.
11. Current Time: A simple tool for the AI to check the current time.

When using Agent mode, you've got the power to switch on a bunch of cool tools for your AI Agent. This lets the LLM pick and use them as needed. We've made sure these tools play nice together. All tools can leverage a shared variable pool to easily access outputs of other tools. For instance, if you make a picture using DALL·E, another tool that makes videos could use that picture in its videos.

In the video demo we've set up, tools like DALL·E and Vectorizer.AI are included. This means your AI Agent can draw a logo for you, then turn it into a vector graphic.

<video autoplay="" class="framer-text framer-image" data-framer-asset="data:framer/asset-reference,Y5C7PlWBa8lEeMSMpLeeFyqbiBQ.mp4" loop="" muted="" playsinline="" src="https://framerusercontent.com/assets/Y5C7PlWBa8lEeMSMpLeeFyqbiBQ.mp4"></video>

Here's how it works: the AI Agent chats with you, asking questions to get what you're after - your style, the vibe you want, and what you like. Once it's got a clear picture, it uses **DALL·E** to craft your design just how you want it. You can offer your ideas for adjustments, and the AI Agent will fine-tune it based on what you say. Then, it hands it off to **Vectorizer.AI** to transform your logo into an SVG format. That way, you can use your new logo whenever you're ready.

## Customize Tools for AI Agents Usage

In the world of business, imagine AI Agents that can securely fetch your company's data or tap into other tools to solve problems in real-time. So, not only do we have some cool built-in tools, but we're also helping developers connect their own custom tools via APIs. Right now, this includes using extensions like [OpenAPI/Swagger](https://swagger.io/docs/specification/about/) and [OpenAI Plugin](https://platform.openai.com/docs/plugins/introduction) standards. What this means is you can bring outside tools into Dify just by tweaking their APIs to match these standards. Once you've got your own tool set up, your whole team can start using it.

<video autoplay="" class="framer-text framer-image" data-framer-asset="data:framer/asset-reference,JCwa3wPXbAcxSQgrvjL7UPvbWJs.mp4" loop="" muted="" playsinline="" src="https://framerusercontent.com/assets/JCwa3wPXbAcxSQgrvjL7UPvbWJs.mp4"></video>

Plus, we're super excited to get developers involved in making new, handy tools by coding them themselves. This is going to make AI Agents even smarter. If this sounds like your kind of thing, take a peek at our [guide](https://github.com/langgenius/dify/blob/48d5628fd4e4045ce39e978d4fd4c522c34f8ec1/api/core/tools/README.md) on how to contribute.

## Updates You Should Know About

We've improved our interface to align with our big upgrades and better reflect Dify's design ethos. Don't worry, your current app won't be impacted:

1. We've rebranded the 'Build Apps' section as 'Studio', and what used to be 'Chat APP' is now simply 'Assistant'. Under this new setup, you can create either a 'Basic Assistant' or an 'Agent Assistant', both harnessing the power of LLM.
2. The 'API Extension' feature, which was part of our 'Chat App' before, has found a new home in the 'Variables' section now. It'll show up as a variable in your prompts. And if you've set up 'API Extension' before, they'll keep working as usual.

![](https://framerusercontent.com/images/qLqZg4tfBq6fq77RrP3ZNbRWI.png)

3. To better organize the wide range of tools for your AI Agent, the 'Tools' option has been moved to the main menu. Here, you can manage everything tool-related, like customizing tools, handling permissions, and other tasks.

## Get Started

Ever thought about creating your own AI Agent? With Dify, you can start from build a new Assistant, opting for the Agent Assistant mode. Or, take an existing Chat App and switch it to Agent Assistant type right from its prompt setup page. Our [docs](https://docs.dify.ai/user-guide/creating-dify-apps/prompt-engineering/agent-assistant) are a great starting point for your adventure.

We're all for you exploring Dify to turn your one-of-a-kind ideas into reality. Whether you're building your own AI Agent or contributing new tools to us, we can't wait to see your creations.

Don’t forget to join our [Discord community](https://discord.com/invite/FngNHpbcY7) to share your thoughts and questions. We’re all ears!