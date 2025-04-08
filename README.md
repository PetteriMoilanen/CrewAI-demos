# CrewAI-demos

This repo is for demoing CrewAI applications. The notebooks are mainly (currently entirely) modified copies of notebooks from two DeepLearning.AI courses: [Multi AI Agent Systems with crewAI](https://learn.deeplearning.ai/courses/multi-ai-agent-systems-with-crewai) and
[Practical Multi AI Agents and Advanced Use Cases with crewAI](https://learn.deeplearning.ai/courses/practical-multi-ai-agents-and-advanced-use-cases-with-crewai).

If you're unfamiliar with CrewAI, here's a good place to start: https://docs.crewai.com/introduction

I'd originally intented to run these notebooks in Colab, but as they have very specific dependencies, I ran into problems with Colab's Torch versions etc.

**Note!** CrewAI (or Chroma to be exact) seems to require sqlite version >= 3.35.0. When running this on a GitHub Codespace default container, importing CrewAI classes produced this error message:
>RuntimeError: Your system has an unsupported version of sqlite3. Chroma                     requires sqlite3 >= 3.35.0.

and I had to update sqlite3 with
```
sudo apt update
sudo apt install -y sqlite3 libsqlite3-dev
```
