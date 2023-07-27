# Illustration Description Storyliner

Illustration Description Storyliner is an AI-powered children's book analyst. It allows users to provide variables in prompts, and produces high-quality custom content. It provides a detailed analysis of kids' book illustrations, including scene, characters, actions, and vital objects. Unique to this app is its ability to intertwine the art analysis with the story's larger theme and progression, offering a narrative analysis that's specific to children's literature.

To run this app online: [Illustration Description Storyliner Online](https://hero.page/app/illustration-description-storyliner-ai-powered-children's-book-analyst/tILOZGomtpLCTDTs8GdW)

[![Run Illustration Description Storyliner Online](/assets/run.svg)](https://hero.page/app/illustration-description-storyliner-ai-powered-children's-book-analyst/tILOZGomtpLCTDTs8GdW)

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
npx hero run ./illustration_description_storyliner.heroml
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
hero run ./illustration_description_storyliner.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./illustration_description_storyliner.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./illustration_description_storyliner.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./illustration_description_storyliner.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Illustration Description Storyliner
```
Start by setting the scene. Describe the overall context and environment for the "Illustration Description" in the "Children's Literature Writing" industry. This description should specifically cater to a "Author". 

Here's some more context about the Illustration Description:
Setting: {{setting}}
Character Description: {{character_description}}
Action Description: {{action_description}}
Object Description: {{object_description}}
Relation To Plot: {{relation_to_plot}}

->>>>

With the following scene set:

Scene Description: 
{{step_1}}

Now, elaborate on the characters present in this scene. Focus on their appearances, special features, or expressions.

->>>>

In our "Illustration Description", we now have a detailed scene and character descriptions:

Scene Description: 
{{step_1}}

Character Description: 
{{step_2}}

Now, emphasize the action taking place in the scene. It could be a significant event, a character's movement, or anything of importance related to the plot of your story.

->>>>

In our "Illustration Description", we have a scene, character descriptions, and the action unfolding:

Scene Description: 
{{step_1}}

Character Description: 
{{step_2}}

Action Description: 
{{step_3}}

Next, give a detailed description of any important objects or elements present in your scene. Explain their significance to the storyline.

->>>>

In our "Illustration Description", we have the scene, characters, actions and now, the important objects or elements:

Scene Description: 
{{step_1}}

Character Description: 
{{step_2}}

Action Description: 
{{step_3}}

Object/Element Description:
{{step_4}}

Now, conclude the description by relating it back to the plot of the story. This helps give the illustration a sense of continuity and relevance.


```

