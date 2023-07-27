# Childlit Blogger Review Creator

Delve into the world of KidLit with the Childlit Blogger Review Creator. This intuitive app uses advanced AI technology to generate customised and engaging reviews for children's literature, specifically for blogs. Simply specify your input, and the app crafts a detailed and conversational review, complete with book introduction, personal opinion, theme analysis, audience recommendation, and comparative analysis. Going beyond mere plot recounting, it provides a deep literary critique, showcasing the book's quality and relevance within the children's literary context.

To run this app online: [Childlit Blogger Review Creator Online](https://hero.page/app/childlit-blogger-review-creator-intelligent-kidlit-blog-reviewer/LFdFdq7MHaMtPi6vGg4h)

[![Run Childlit Blogger Review Creator Online](/assets/run.svg)](https://hero.page/app/childlit-blogger-review-creator-intelligent-kidlit-blog-reviewer/LFdFdq7MHaMtPi6vGg4h)

To learn more about AI Apps for Blogger use-cases in the Children's Literature Writing industry, read [How to Elevate your Children's Literature Blog with AI Apps](https://hero.page/blog/ai/children's-literature-writing/how-to-elevate-your-children's-literature-blog-with-ai-apps/170785)

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
npx hero run ./childlit_blogger_review_creator.heroml
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
hero run ./childlit_blogger_review_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./childlit_blogger_review_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./childlit_blogger_review_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./childlit_blogger_review_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Childlit Blogger Review Creator
```
To write a "Book Review" for the "Children's Literature Writing" industry, for a "Blogger", follow these instructions:

Start by writing an engaging introduction that includes the title of the book, the name of the author, and a brief outline of what the book is about. Remember to mention {{book_title}}, {{author_name}}, and provide a brief {{book_summary}}.

Here's some more context about the Book Review:
Book Title: {{book_title}}
Author Name: {{author_name}}
Book Summary: {{book_summary}}
Book Characters: {{book_characters}}
Book Plot: {{book_plot}}
Book Setting: {{book_setting}}
Personal Opinion: {{personal_opinion}}
Book Themes: {{book_themes}}
Intended Audience: {{intended_audience}}
Comparative Analysis: {{comparative_analysis}}

->>>>

For our book review, we now have an engaging introduction about:

Book Title:
{{step_1}}

For the next step, let's focus on the book's main elements. Write an overview of the main characters, plot, and setting without revealing too much detail or any spoilers. Make sure you mention {{book_characters}}, {{book_plot}}, and {{book_setting}}.

->>>>

Our book review now has an introduction and an overview of the story:

Introduction:
{{step_1}}

Overview:
{{step_2}}

Now, it's time to share your thoughts on the book. In the "Personal Opinion" section, comment on the language style, pacing, and the emotional connection you felt with the characters. Express what you liked or didn’t like about the book and include examples to back up your opinions. Please keep your {{personal_opinion}} professional and respectful.

->>>>

In our book review so far, we have:

Introduction:
{{step_1}}

Story Overview:
{{step_2}}

Personal Opinion:
{{step_3}}

Next, let's delve into the book's core themes or messages and their relevance to children. Use examples from the book to emphasize these themes. Please provide your insight on {{book_themes}}.

->>>>

At this point, our book review has:

Introduction:
{{step_1}}

Story Overview:
{{step_2}}

Personal Opinion:
{{step_3}}

Book Themes:
{{step_4}}

For the "Recommendation" section, discuss who you think would most enjoy the book and why. Mention age groups, interests, etc. in your recommendation. Your review can also compare how the book stacks up against other books of the same genre or by the same author. So please include, {{intended_audience}} and {{comparative_analysis}}.

->>>>

Our book review now includes:

Introduction:
{{step_1}}

Story Overview:
{{step_2}}

Personal Opinion:
{{step_3}}

Book Themes:
{{step_4}}

Recommendation:
{{step_5}}

Next, put together a thought-provoking conclusion to wrap up the review. This conclusion should restate your personal opinion, the relevance of the themes, and reader recommendations.


```

