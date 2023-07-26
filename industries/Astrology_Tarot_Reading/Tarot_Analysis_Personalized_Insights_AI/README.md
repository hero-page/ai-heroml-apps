# Tarot Analysis & Personalized Insights AI

Explore the mysteries of tarot with AI-Powered Tarot Analysis. Employing advanced AI intelligence, this app garners customized, high-grade tarot card readings. Detailing cosmic alignments, defining card spreads, signifying each card in its placement, analyzing cards' intermingling narratives, and mapping the reading to personal life or situations, the app provides holistic, personalized insights. The in-depth, specialized tarot interpretation integrates astrology for a unique, tailored tarot experience.

To run this app online: [Tarot Analysis & Personalized Insights AI Online](https://hero.page/app/tarot-analysis-and-personalized-insights-ai-ai-powered-personalized-tarot-analysis/9SXRFm4lvIjSPdGIKwxJ)

[![Run Tarot Analysis & Personalized Insights AI Online](/assets/run.svg)](https://hero.page/app/tarot-analysis-and-personalized-insights-ai-ai-powered-personalized-tarot-analysis/9SXRFm4lvIjSPdGIKwxJ)

To learn more about AI Apps for Tarot Reader use-cases in the Astrology & Tarot Reading industry, read [How to Enhance Tarot Reading with AI-Assisted Card Analysis](https://hero.page/blog/ai/astrology-and-tarot-reading/how-to-enhance-tarot-reading-with-ai-assisted-card-analysis/170743)

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
npx hero run ./tarot_analysis_and_personalized_insights_ai.heroml
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
hero run ./tarot_analysis_and_personalized_insights_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./tarot_analysis_and_personalized_insights_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./tarot_analysis_and_personalized_insights_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./tarot_analysis_and_personalized_insights_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Tarot Analysis & Personalized Insights AI
```
Your task is to write a "Card Analysis" for the "Astrology & Tarot Reading" industry, specifically designed for a "Tarot Reader".

The first thing we need to do is provide an introduction detailing the overall context of the reading, taking into account aspects such as the intention behind the reading, the reader’s persona, and the current cosmic alignments. Make use of the dynamic variable {{reading_context}} for this purpose.

Here's some more context about the Card Analysis:
Reading Context: {{reading_context}}
Spread Description: {{spread_description}}
Card Symbolism: {{card_symbolism}}
Card Position: {{card_position}}
Specific Card Context: {{specific_card_context}}
Combined Card Meanings: {{combined_card_meanings}}
Applicable Life Aspects: {{applicable_life_aspects}}

->>>>

Now, we have an introduction for our card analysis:

Introduction:
{{step_1}}

Next, provide a description of the spread that was used during the reading. Remember to make use of the dynamic variable {{spread_description}} for this step.

->>>>

We have an introduction and a description of the spread used in the reading:

Introduction:
{{step_1}}

Spread Description:
{{step_2}}

Next, we need to delve into the analysis of each card in its position within the spread. For each card, discuss the following:
- The card symbolism, making use of the variable {{card_symbolism}}.
- The implications of the card's upright or reversed position, using the variable {{card_position}}.
- How the card's specific meaning is tied into the broader context of the reading, using the variable {{specific_card_context}}.

->>>>

Thus far in our card analysis, we have:

Introduction:
{{step_1}}

Spread Description:
{{step_2}}

Individual Card Analysis:
{{step_3}}

Next, discuss how the cards interact within the spread and explain the combined meanings they form. Use the dynamic variable {{combined_card_meanings}} for this.

->>>>

So far, our card analysis has:

Introduction:
{{step_1}}

Spread Description:
{{step_2}}

Individual Card Analysis:
{{step_3}}

Combined Card Meanings:
{{step_4}}

Now, we need to dedicate a portion of the analysis to the application of this Tarot reading to the querent's life or situation, taking into account the astrological correlations or metaphysical aspects of each card. Use the dynamic variable {{applicable_life_aspects}} for this.

->>>>

So far in the card analysis, we have:

Introduction:
{{step_1}}

Spread Description:
{{step_2}}

Individual Card Analysis:
{{step_3}}

Combined Card Meanings:
{{step_4}}

Applicable Life Aspects:
{{step_5}}

Finally, conclude the analysis by recapping the overall message of the Tarot reading, keeping in mind the context in which the reading was done, which is detailed in the variable {{reading_context}} from step 1. Make sure to link the concluding message with all the aspects discussed in the previous steps.


```

