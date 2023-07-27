# Pranayama Journey Content Creator

Pranayama Journey Content Creator, your personalized Pranayama Instructor narratives guide. This app allows you to craft detailed story prompts and uses AI to generate high-quality, customized content. It produces an authentic narrative spotlighting the instructor's journey, from initial interest to professional teaching, highlighting personal challenges, breakthroughs, and ambitions intertwined with core Pranayama principles. The content offers a unique, in-depth exploration of the Pranayama instruction world.

To run this app online: [Pranayama Journey Content Creator Online](https://hero.page/app/pranayama-journey-content-creator-personalized-pranayama-instructor-narratives/5uPZ7DLMdNf3UaoD16IE)

[![Run Pranayama Journey Content Creator Online](/assets/run.svg)](https://hero.page/app/pranayama-journey-content-creator-personalized-pranayama-instructor-narratives/5uPZ7DLMdNf3UaoD16IE)

To learn more about AI Apps for Pranayama Instructor use-cases in the Breathwork & Pranayama industry, read [How to Elevate Pranayama Instruction with AI Tools](https://hero.page/blog/ai/breathwork-and-pranayama/how-to-elevate-pranayama-instruction-with-ai-tools/170767)

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
npx hero run ./pranayama_journey_content_creator.heroml
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
hero run ./pranayama_journey_content_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./pranayama_journey_content_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./pranayama_journey_content_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./pranayama_journey_content_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Pranayama Journey Content Creator
```
Your task is to write a "Personal Experience" for the "Breathwork & Pranayama" industry, particularly as a "Pranayama Instructor". 

Let's start with an introduction to this personal experience, providing some background as to your interest in Pranayama. This could be your personal story detailing how you became interested in breathwork and any motivational factors that led you to become an instructor.

Here's some more context about the Personal Experience:
Interest In Pranayama: {{Interest_In_Pranayama}}
Initial Learning Experience: {{Initial_Learning_Experience}}
Professional Journey: {{Professional_Journey}}
Present Teaching Experience: {{Present_Teaching_Experience}}
Reflection And Aspirations: {{Reflection_and_Aspirations}}

->>>>

We have an introduction for the personal experience of a Pranayama Instructor:

Introduction:
{{step_1}}

Next, let's elaborate on your initial learning experience in Pranayama and the hurdles you overcame. This should include the various techniques you learned, your experiences with each, influences of your teachers, and any personal challenges you've vanquished during this stage.

->>>>

We now have an introduction and the details about your initial learning experience:

Introduction:
{{step_1}}

Initial Learning Experience:
{{step_2}}

Moving forward, let's share your journey of evolving from a student to a professional Pranayama Instructor. Discuss the training specifics, certification processes, emotional transformations, and your early experiences in the professional realm.

->>>>

So far, we have details of your initial learning experience, and your journey to a professional instructor:

Initial Learning Experience:
{{step_2}}

Professional Journey:
{{step_3}}

Now, describe your present Pranayama teaching experience emphasising on student interaction, class dynamics, common problems faced by students and how you help resolve them. Speak about the expertise you've gained over time.

->>>>

With the professional journey and current teaching experience detailed:

Professional Journey:
{{step_3}}

Present Teaching Experience:
{{step_4}}

Lastly, let's reflect on your entire journey. Summarize your personal experiences with Pranayama: the value it has added to your life, and your aspirations as a Pranayama Instructor. Your reflection should exemplify the essence of Pranayama practice as per your understanding, manifesting its relevance and value.


```

