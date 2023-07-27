# Children's Story Creator AI

Children's Story Creator AI is an advanced app that harnesses AI to create unique, high-quality kids stories based on the parameters you set. Tailor your plot, introduce characters, and specify conflicts and resolutions to construct a narrative that educates and entertains. This tailored approach guarantees bespoke stories that help children understand important world concepts. With a child-friendly language, the app focuses on fostering enjoyable learning experiences.

To run this app online: [Children's Story Creator AI Online](https://hero.page/app/children's-story-creator-ai-ai-powered-custom-kid's-stories/iUibhfNq53JUwiwDF7o1)

[![Run Children's Story Creator AI Online](/assets/run.svg)](https://hero.page/app/children's-story-creator-ai-ai-powered-custom-kid's-stories/iUibhfNq53JUwiwDF7o1)

To learn more about AI Apps for Author use-cases in the Children's Literature Writing industry, read [How to Enhance Children's Story Creation with AI Apps](https://hero.page/blog/ai/children's-literature-writing/how-to-enhance-children's-story-creation-with-ai-apps/170783)

### What is HeroML?
HeroML is an AI Prompt Chain/Workflow interpreter for Apps built on https://hero.page 

To see other apps, visit the [Hero Apps](https://hero.page/apps) page or explore [AI Apps for all industries](https://hero.page/blog) in the blog section

For more documentation, visit [Hero docs, and learn about AI App Workflows](https://hero.page/tutorials/introduction-to-heroml)

Download [VSCode Syntax Highlighter Ext. here](https://marketplace.visualstudio.com/items?itemName=hero-page.heroml)

## Run with HeroCLI (Requires OpenAI Token)

#### Installation

To install the HeroML CLI tool, you need to have Node.js and npm (comes with Node.js) installed on your machine. If you don't have these, please install them first. 

Then, run the following command in your terminal:

```bash
npm install -g heroml
```

This will install the HeroML CLI tool globally on your system, allowing you to use the `hero` command from any directory.

If you don't want to install it globally, you can run:

```bash
npm install heroml
```

and use it like:

```bash
npx hero run ./childrens_story_creator_ai.heroml
```

We'll be using `hero run ...` in this tutorial for simplicity.

#### Configuration

Before using the HeroML CLI tool, you need to configure your OpenAI API key. 

Create a `heroconfig.json` file in your home directory with the following content:

```json
{
  "openaiApiKey": "your-openai-api-key"
}
```

Replace `"your-openai-api-key"` with your actual OpenAI API key.

#### Usage

To run a HeroML script, use the `run` command followed by the path to your script:

```bash
hero run ./childrens_story_creator_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./childrens_story_creator_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./childrens_story_creator_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./childrens_story_creator_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Children's Story Creator AI
```
Your task is to write a "Children's Story" for the "Children's Literature Writing" industry, specifically for an "Author". Let's start by creating an engaging introduction for the story where we set up the scene or setting where {{main_character}} lives and a brief introduction about {{main_character}}.

Here's some more context about the Children's Story:
Main Character: {{main_character}}

->>>>

We have a story introduction that sets the stage and introduces our main character:

Story Introduction:
{{step_1}}

Now, create a problem or conflict for the {{main_character}} that they need to resolve. This conflict is the basis for an engaging plot for children.

->>>>

Our story has an introduction and a central conflict for the main character:

Story Introduction:
{{step_1}}

Central Conflict:
{{step_2}}

Next, introduce the other key characters in the story. They can be friends, family, an antagonist, or anyone who contributes significantly to the story plot.

->>>>

Our story's cast has now expanded, we have our main character, central conflict, and additional key characters:

Central Conflict:
{{step_2}}

Additional Characters:
{{step_3}}

Moving on, develop the plot of the story detailing how the {{main_character}} encounters and begins dealing with their problem or conflict.

->>>>

We have a plot where our main character starts dealing with the problem:

Additional Characters:
{{step_3}}

Plot:
{{step_4}}

Make sure to 'show' the story through the character's actions rather than merely 'telling' it. For example, if {{main_character}} is courageous, demonstrate their courage through their actions.

->>>>

The story is shaping up with clear plot points and its actions. Let's see what we have:

Plot:
{{step_4}}

Actions 'Shown': 
{{step_5}}

Now, build the tension in the story up towards the climax. This is the point in the story where the {{main_character}} is closest to solving the problem but encounters a significant setback.

->>>>

Our story's tension is building up nicely towards a climax:

Actions 'Shown': 
{{step_5}}

Climax:
{{step_6}}

At this stage, we need to have the {{main_character}} address their conflict and eventually solve it or learn something crucial. This is the resolution of the story.

->>>>

The story has a climax and a resolution, and the main character has learned something important:

Climax:
{{step_6}}

Resolution:
{{step_7}}

Compose a conclusion for the story illustrating the aftermath of the problem's resolution and showing how the experience changed {{main_character}} or what they learned from it.

->>>>

Our story concludes with a meaningful reflection based on the story's resolution:

Resolution:
{{step_7}}

Conclusion:
{{step_8}}

Perform a language check. Ensure the language used in the story is easy to understand and appropriate for children in terms of complexity and content.

->>>>

The language in our story is appropriate for children and readily understandable:

Language Checked Story:
{{step_9}}

Now, finalise the story by including a moral or takeaway point. This needs to be relevant to the problem {{main_character}} encountered and how they managed to resolve or deal with it.


```

