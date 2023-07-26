# Angel Card Reading Guide Creator

Explore the spiritual realm with Angel Card Reading Guide Creator. This comprehensive app lets users modify variables for personalized prompts, utilizing advanced AI to generate holistic, in-depth guides on Angel Card readings. Experience a step-by-step walkthrough from mood setting to interpreting cards and post-session reflections. Plus, discover how to foster connections with celestial beings and harness intuition for a profound spiritual journey. Unveil unique, actionable advice based on your readings, creating an immersive and personalized experience for the reader and client.

To run this app online: [Angel Card Reading Guide Creator Online](https://hero.page/app/angel-card-reading-guide-creator-comprehensive-custom-angel-card-guide/JdZFFZDVbjIrZHIaQgZF)

[![Run Angel Card Reading Guide Creator Online](/assets/run.svg)](https://hero.page/app/angel-card-reading-guide-creator-comprehensive-custom-angel-card-guide/JdZFFZDVbjIrZHIaQgZF)

To learn more about AI Apps for Angel Card Reader use-cases in the Angel Card Reading industry, read [How to Elevate Angel Card Readings with AI Insights](https://hero.page/blog/ai/angel-card-reading/how-to-elevate-angel-card-readings-with-ai-insights/170725)

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
npx hero run ./angel_card_reading_guide_creator.heroml
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
hero run ./angel_card_reading_guide_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./angel_card_reading_guide_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./angel_card_reading_guide_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./angel_card_reading_guide_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Angel Card Reading Guide Creator
```
Your task is to write a "Reading Experience" for the "Angel Card Reading" industry, specifically for an "Angel Card Reader". 
Start by crafting an introduction that sets the mood for the reading session. This might include the reason for the reading: {{reason_for_reading}}.

Here's some more context about the Reading Experience:
Reason For Reading: {{reason_for_reading}}
Chosen Spread: {{chosen_spread}}
Question Or Focus: {{question_or_focus}}
Querent State: {{querent_state}}

->>>>

Your task is to provide a reading experience. Till now we have:

Introduction:
{{step_1}}

Now, describe the process of how to select and spread the Angel Cards, which is the central task of an Angel Card Reading. In this section, ensure to explain how the reader shuffles and cuts the deck, then spreads the cards in the {{chosen_spread}}.

->>>>

We have: 

Introduction:
{{step_1}}

Selection & Spreading Angel Cards:
{{step_2}}

Now, provide a guide for interpreting each card's symbolism and messages. Illustrate how their meanings can be influenced by the position of cards in {{chosen_spread}} and their relation to the {{question_or_focus}}.

->>>>

We have: 

Introduction:
{{step_1}}

Selection & Spreading Angel Cards:
{{step_2}}

Interpreting Angels Cards:
{{step_3}}

Now dedicates a section to address the key points associated with the {{question_or_focus}}. Let the angel card reader interpret these cards considering the individual's emotional, physical, and mental status: {{querent_state}}. After this, help the reader to lead the querent through a discussion on how these cards answer or give insights into the {{question_or_focus}}.

->>>>

We now have detailed the process of selecting and spreading the cards and interpreting them:

Introduction:
{{step_1}}

Selection & Spreading Angel Cards:
{{step_2}}

Interpreting Angels Cards:
{{step_3}}

Addressing Key Points:
{{step_4}}

Next, detail the importance of connecting with the angels during the reading. Try to emphasise the role of intuition in angel card reading, guiding the user to feel and understand energy and possible messages from angels related to the {{querent_state}} and {{question_or_focus}}.

->>>>

Currently, we have:

Introduction:
{{step_1}}

Selection & Spreading Angel Cards:
{{step_2}}

Interpreting Angels Cards:
{{step_3}}

Addressing Key Points:
{{step_4}}

Connecting with Angels:
{{step_5}}

Now, wrap up the reading experience by summarising the essential points. Provide guidance on integrating the insights from the reading into real-life scenarios based on the {{question_or_focus}} and the individual's state of being: {{querent_state}}.

->>>>

We have developed so far:

Introduction:
{{step_1}}

Selection & Spreading Angel Cards:
{{step_2}}

Interpreting Angels Cards:
{{step_3}}

Addressing Key Points:
{{step_4}}

Connecting with Angels:
{{step_5}}

Wrapping up the Reading:
{{step_6}}

Next, close the reading session by encouraging the querent to express their thoughts on the experience, any insights they gained and how they are feeling post-reading about the {{question_or_focus}}. 


```

