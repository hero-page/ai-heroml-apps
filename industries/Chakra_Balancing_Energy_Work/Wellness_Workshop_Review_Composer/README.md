# Wellness Workshop Review Composer

Wellness Workshop Review Composer is a unique app designed for writing high-quality reviews on wellness workshops personalized to your journey. The app uses AI technology to create customizable content, focusing on your experience with various aspects like facilitator's teaching style, workshop materials, and overall participation. It also evaluates the impact of the workshop on your wellness journey, from how you felt during the session to the changes it initiated in your lifestyle. Most importantly, the app captures the unique experiences that make your review a potential guide for others interested in similar workshops.

To run this app online: [Wellness Workshop Review Composer Online](https://hero.page/app/wellness-workshop-review-composer-personalizing-your-wellness-journey-reviews/JRivOQVvM3RyCsWod1E6)

[![Run Wellness Workshop Review Composer Online](/assets/run.svg)](https://hero.page/app/wellness-workshop-review-composer-personalizing-your-wellness-journey-reviews/JRivOQVvM3RyCsWod1E6)

To learn more about AI Apps for Wellness Blogger use-cases in the Chakra Balancing & Energy Work industry, read [How to Amplify Your Wellness Journey with AI in Chakra Balancing & Energy Work](https://hero.page/blog/ai/chakra-balancing-and-energy-work/how-to-amplify-your-wellness-journey-with-ai-in-chakra-balancing-and-energy-work/170773)

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
npx hero run ./wellness_workshop_review_composer.heroml
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
hero run ./wellness_workshop_review_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./wellness_workshop_review_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./wellness_workshop_review_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./wellness_workshop_review_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Wellness Workshop Review Composer
```
Your task is to write a "Workshop Review" for the "Chakra Balancing & Energy Work" industry, specifically for a "Wellness Blogger". Let's start with an introduction detailing the name of the workshop: {{workshop_name}}, the facilitator: {{facilitator}}, and the location and date: {{location_and_date}}.

Here's some more context about the Workshop Review:
Workshop Name: {{workshop_name}}
Facilitator: {{facilitator}}
Location And Date: {{location_and_date}}
Materials Provided: {{materials_provided}}
Active Participation: {{active_participation}}
Impact: {{impact}}

->>>>

Currently, we have the introductory section for our workshop review:

Introduction:
{{step_1}}

Next, provide a brief overview of the workshop's purpose and the key elements of chakra balancing and energy work it focused on.

->>>>

We now have an introduction and an overview of our workshop:

Introduction:
{{step_1}}

Workshop Overview:
{{step_2}}

Following this, describe your initial impressions of the workshop setting and the materials provided: {{materials_provided}}.

->>>>

So far for our review, we have an introduction, workshop overview, and initial impressions:

Introduction:
{{step_1}}

Workshop Overview:
{{step_2}}

Initial Impressions:
{{step_3}}

Now, detail the techniques taught in the workshop for chakra balancing and energy work. Compare these to other methods you are aware of.

->>>>

We have now documented details about the taught techniques:

Introduction:
{{step_1}}

Techniques Taught:
{{step_4}}

Next, we need to discuss the facilitator's teaching style, their effective communication, understanding of the subject, and their command over the techniques.

->>>>

Here's what we have so far for our review, including the new section on the facilitator's teaching quality:

Introduction:
{{step_1}}

Techniques Taught:
{{step_4}}

Facilitator's Teaching Quality:
{{step_5}}

Following on, share your experience of active participation, the exercises conducted: {{active_participation}}, and explain how they helped in the process of chakra balancing and energy work.

->>>>

Now, we need to discuss your active participation during the workshop:

Introduction:
{{step_1}}

Techniques Taught:
{{step_4}}

Active Participation:
{{step_6}}

As the next step, share about the impact of the workshop on your personal wellness journey: {{impact}}. Discuss emotional and mental transformations, and how the understanding of the subject matter was improved.

->>>>

We have accumulated substantial content for our review, and now, we have a section dedicated to the impact of the workshop:

Introduction:
{{step_1}}

Techniques Taught:
{{step_4}}

Wellness Impact:
{{step_7}}

Next, reflect on the workshop’s contributions to the wellness community.

->>>>

Our review is filling out nicely, let's see what we've achieved:

Introduction:
{{step_1}}

Techniques Taught:
{{step_4}}

Contribution to Wellness Community:
{{step_8}}

Finally, wrap up the review with an overall assessment of the workshop. Suggest who will benefit most from this kind of workshop and whether you'd consider attending again.


```

