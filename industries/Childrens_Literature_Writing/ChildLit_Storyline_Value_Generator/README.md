# ChildLit Storyline & Value Generator

ChildLit Storyline & Value Generator lets you generate tailor-made children's stories using AI technology. Specify your preferred variables and watch as the app creates high-quality narratives featuring engaging premises, main characters, settings, narrative arcs. But unlike others, the stories also integrate common themes or moral lessons. As they imbue young minds with values, these narratives also meet the strict standards of children's literature editors, making them perfect for professional publications.

To run this app online: [ChildLit Storyline & Value Generator Online](https://hero.page/app/childlit-storyline-and-value-generator-creating-valued-kids'-storylines/4sNChDf9JPfYmHUqRIVB)

[![Run ChildLit Storyline & Value Generator Online](/assets/run.svg)](https://hero.page/app/childlit-storyline-and-value-generator-creating-valued-kids'-storylines/4sNChDf9JPfYmHUqRIVB)

To learn more about AI Apps for Editor use-cases in the Children's Literature Writing industry, read [How to Enhance Children's Book Editing with AI Tools](https://hero.page/blog/ai/children's-literature-writing/how-to-enhance-children's-book-editing-with-ai-tools/170784)

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
npx hero run ./childlit_storyline_and_value_generator.heroml
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
hero run ./childlit_storyline_and_value_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./childlit_storyline_and_value_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./childlit_storyline_and_value_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./childlit_storyline_and_value_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for ChildLit Storyline & Value Generator
```
Your task is to write "Storyline Suggestions" for the "Children's Literature Writing" industry, specifically for an "Editor". Let's start by generating an engaging premise that highlights the main conflict or adventure around which the story revolves:

Here's some more context about the Storyline Suggestions:
Story Premise: {{story_premise}}
Main Characters: {{main_characters}}
Main Settings: {{main_settings}}
Narrative Arc: {{narrative_arc}}
Themes Values: {{themes_values}}
Lessons Morals: {{lessons_morals}}

->>>>

We have the premise for our children's story:

Story Premise:
{{step_1}}

Next, introduce the main characters, describing their personalities and roles within the story:

->>>>

Now, with an engaging premise and main characters for our storyline:

Story Premise:
{{step_1}}

Main Characters:
{{step_2}}

Let's describe the main settings or locations where the story takes place:

->>>>

For our engaging children's story, we have the premise, main characters, and the main settings:

Story Premise:
{{step_1}}

Main Characters:
{{step_2}}

Main Settings:
{{step_3}}

Now, let's map out the narrative arc, which includes the setup, conflict, climax, and resolution:

->>>>

So far, we've created the premise, main characters, settings and narrative arc for our children's story:

Story Premise:
{{step_1}}

Main Characters:
{{step_2}}

Main Settings:
{{step_3}}

Narrative Arc:
{{step_4}}

Let's enrich the story by incorporating common themes and values relevant to children's literature such as friendship, kindness, courage, and learning:

->>>>

Our storyline now has an engaging premise, main characters, settings, and narrative arc, along with relevant themes for children's literature:

Story Premise:
{{step_1}}

Main Characters:
{{step_2}}

Main Settings:
{{step_3}}

Narrative Arc:
{{step_4}}

Themes & Values:
{{step_5}}

To conclude, let's propose potential lessons or morals that children can learn from this storyline. The lessons should be simple and practical for children to understand and apply in their own lives.


```

