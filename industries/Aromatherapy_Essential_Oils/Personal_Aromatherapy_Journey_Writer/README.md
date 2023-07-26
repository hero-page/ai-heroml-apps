# Personal Aromatherapy Journey Writer

Explore the world of aromatherapy with Personal Aromatherapy Journey Writer app! Add your personal inputs and let the app create high-quality content about your essential oil experiences. The app combines user inputs with AI technology to generate personalized aromatherapy narratives, covering historical and scientific background, detailed essential oil descriptions, benefits, DIY recipes, buying guidance and wellness impact. What sets us apart is that our insights include your personal anecdotes making the content unique, engaging, and highly relatable. With insights from reputable sources, this app serves as an informative guide for both novice and experienced aromatherapy enthusiasts.

To run this app online: [Personal Aromatherapy Journey Writer Online](https://hero.page/app/personal-aromatherapy-journey-writer-custom-aromatherapy-narratives-and-insights/q4EqyUOf9j0s7pG0Fkh1)

[![Run Personal Aromatherapy Journey Writer Online](/assets/run.svg)](https://hero.page/app/personal-aromatherapy-journey-writer-custom-aromatherapy-narratives-and-insights/q4EqyUOf9j0s7pG0Fkh1)

To learn more about AI Apps for Wellness Blogger use-cases in the Aromatherapy & Essential Oils industry, read [How to Enrich Your Aromatherapy Journey with AI Solutions](https://hero.page/blog/ai/aromatherapy-and-essential-oils/how-to-enrich-your-aromatherapy-journey-with-ai-solutions/170730)

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
npx hero run ./personal_aromatherapy_journey_writer.heroml
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
hero run ./personal_aromatherapy_journey_writer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./personal_aromatherapy_journey_writer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./personal_aromatherapy_journey_writer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./personal_aromatherapy_journey_writer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Personal Aromatherapy Journey Writer
```
Your task is to write a "Personal Experience" for the "Aromatherapy & Essential Oils" industry, specifically for a "Wellness Blogger". Let's start with an introduction that conveys a personal narrative about your introduction to aromatherapy and essential oils.

Here's some more context about the Personal Experience:
Initial Experience: {{initial_experience}}
Essential Oils Background: {{essential_oils_background}}
Personal Experiences: {{personal_experiences}}
Favorite Oils: {{favorite_oils}}
DIY Recipes: {{DIY_recipes}}
Oil Sources: {{oil_sources}}
Overall Experience: {{overall_experience}}

->>>>

You've shared a personal narrative about the introduction to aromatherapy and essential oils:

Introduction:
{{step_1}}

Next, let's discuss the history and science behind aromatherapy and essential oils. Be sure to justify your points with reliable sources.

->>>>

The history and science behind aromatherapy and essential oils have been discussed:

Introduction:
{{step_1}}

Essential Oils Background:
{{step_2}}

Now, share your personal journey and experiences with different oils, focusing on specific instances where they helped improve your well-being. Include both the positive and negative experiences for a well-rounded account.

->>>>

Personal experiences with different oils have been discussed:

Essential Oils Background:
{{step_2}}

Personal Experiences:
{{step_3}}

The next task is to describe in detail the specific aromatherapy oils you personally use the most. Break this section into subsections for each oil, describing their unique properties, benefits, how to use them, and any safety precautions needed.

->>>>

The favorite oils and their specific details are explored:

Personal Experiences:
{{step_3}}

Favorite Oils:
{{step_4}}

Let's proceed to discuss any do-it-yourself (DIY) recipes or experiments you've tried using essential oils. Think about their efficiency, their smell, their feel, and any notable changes you observed.

->>>>

The exploration of DIY recipes and experiments has been done:

Favorite Oils:
{{step_4}}

DIY Recipes:
{{step_5}}

Now, provide information about any local or online stores where you usually source your essential oils.

->>>>

Information about sourcing essential oils has been discussed:

DIY Recipes:
{{step_5}}

Oil Sources:
{{step_6}}

Following that, share tips and recommendations on how potential newbies should introduce themselves to aromatherapy and essential oils.

->>>>

You have shared tips and recommendations for newcomers:

Oil Sources:
{{step_6}}

Tips and Recommendations:
{{step_7}}

To culminate, let's write about the overall impact that incorporating aromatherapy and essential oils has had on your wellness routine and life. This should be both personal and informative.


```

