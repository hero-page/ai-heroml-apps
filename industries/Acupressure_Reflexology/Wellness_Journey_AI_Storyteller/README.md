# Wellness Journey AI Storyteller

Wellness Journey AI Storyteller app offers a new approach to wellness storytelling. Leveraging AI, it generates personalized narratives that simulate a wellness blogger's experiences on your chosen wellness practices. Enjoy engaging, custom content reflecting evolving sessions, conclusive assessment, and recommendations. With its unique perspective, expect detailed accounts on techniques like acupressure or reflexology, making the experience relatable and enriching. An immersive wellness narrative designed just for you.

To run this app online: [Wellness Journey AI Storyteller Online](https://hero.page/app/wellness-journey-ai-storyteller-personalized-wellness-journey-narratives/y8BmmTk3DP7CTbgK5IQk)

[![Run Wellness Journey AI Storyteller Online](/assets/run.svg)](https://hero.page/app/wellness-journey-ai-storyteller-personalized-wellness-journey-narratives/y8BmmTk3DP7CTbgK5IQk)

To learn more about AI Apps for Wellness Blogger use-cases in the Acupressure & Reflexology industry, read [How to Elevate Acupressure Blogging with AI Assisted Journeys & Reviews](https://hero.page/blog/ai/acupressure-and-reflexology/how-to-elevate-acupressure-blogging-with-ai-assisted-journeys-and-reviews/170715)

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
npx hero run ./wellness_journey_ai_storyteller.heroml
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
hero run ./wellness_journey_ai_storyteller.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./wellness_journey_ai_storyteller.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./wellness_journey_ai_storyteller.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./wellness_journey_ai_storyteller.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Wellness Journey AI Storyteller
```
Your task is to write a "Personal Experience" for the "Acupressure & Reflexology" industry, specifically for a "Wellness Blogger". 

Start by introducing the specific acupressure or reflexology technique being explored.

Here's some more context about the Personal Experience:
Technique: {{technique}}
Finding Practitioner: {{finding_practitioner}}
First Experience: {{first_experience}}
Progress: {{progress}}
Conclusion: {{conclusion}}

->>>>

Now, the blog post for our "Wellness Blogger" has an introduction about the specific technique:

Introduction about the Technique:
{{step_1}}

Next, let's detail the process of finding a suitable practitioner or learning how to perform the technique. This can include steps taken to research and locate a practitioner, making an appointment, or studying the methods if self-administered.

->>>>

The blog post now has an introduction and details about how the suitable practitioner was found or how the technique was learned:

Technique Introduction:
{{step_1}}

Process of Learning or Finding a Practitioner:
{{step_2}}

Now, provide a comprehensive account of your first experience with this technique. This should describe both the physical and emotional journey.

->>>>

The blog post about the "Personal Experience" now includes the technique introduction, the learning process, and the first interaction with the technique:

Technique Introduction:
{{step_1}}

Process of Learning or Finding a Practitioner:
{{step_2}}

First Experience with Technique:
{{step_3}}

Moving on, describe your progress and any changes you noticed over several sessions of the technique or over a sufficient period of self-practice. This could include physical benefits, emotional improvements, any changes in habit or lifestyle, and a reflection on the difference between expectation and reality.


```

