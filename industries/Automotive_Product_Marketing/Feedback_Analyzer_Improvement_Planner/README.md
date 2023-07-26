# Feedback Analyzer & Improvement Planner

Feedback Analyzer & Improvement Planner is an advanced AI-driven application that enhances your feedback strategy optimization. Customize your inputs to analyze insightful generated content specific to your needs. Expect a detailed analysis report on product user feedback, emphasizing both positive and negative key features, using specialized data collection and analysis methods, segmented themes, and the provision of improvement suggestions. Notable is our unique feature of actionable data application for product enhancement strategies. It also bears an additional notes section highlighting sporadic, significant user comments for a comprehensive feedback assessment.

To run this app online: [Feedback Analyzer & Improvement Planner Online](https://hero.page/app/feedback-analyzer-and-improvement-planner-ai-driven-feedback-strategy-optimizer/FuMFJShoCsfO1nJaIZnU)

[![Run Feedback Analyzer & Improvement Planner Online](/assets/run.svg)](https://hero.page/app/feedback-analyzer-and-improvement-planner-ai-driven-feedback-strategy-optimizer/FuMFJShoCsfO1nJaIZnU)

To learn more about AI Apps for Product Manager use-cases in the Automotive Product Marketing industry, read [How to Refine Automotive Product Marketing with AI Tools](https://hero.page/blog/ai/automotive-product-marketing/how-to-refine-automotive-product-marketing-with-ai-tools/170747)

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
npx hero run ./feedback_analyzer_and_improvement_planner.heroml
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
hero run ./feedback_analyzer_and_improvement_planner.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./feedback_analyzer_and_improvement_planner.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./feedback_analyzer_and_improvement_planner.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./feedback_analyzer_and_improvement_planner.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Feedback Analyzer & Improvement Planner
```
Your task is to write a "Customer Feedback Report" for the "Automotive Product Marketing" industry, specifically for a "Product Manager". 
Let's initialize this report by preparing the first part: an executive summary, which gives an overall impression about the feedback based on {{feedback_overview}}.

Here's some more context about the Customer Feedback Report:
Feedback Overview: {{feedback_overview}}
Product Focus: {{product_focus}}
Feedback Themes: {{feedback_themes}}
Positive Features: {{positive_features}}
Negative Features: {{negative_features}}
Improvement Areas: {{improvement_areas}}

->>>>

With the generation of our executive summary:

Executive Summary:
{{step_1}}

We'll continue by articulating an introduction that emphasizes the need for this report, identifying its relevance in enhancing product offerings with reference to {{product_focus}}.

->>>>

Our "Customer Feedback Report" currently holds an executive summary and introduction as follows:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Now, it is crucial to detail our data collection and analysis methodology for understanding the authenticity and comprehensibility of the feedback received.

->>>>

For our report, we now have:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Methodology:
{{step_3}}

We can proceed to the main body of the report, where we will analyse and address the major themes or categories emerging from the customer feedback with reference to {{feedback_themes}}.

->>>>

In the main body of the report, we have analyzed feedback themes:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Methodology:
{{step_3}}

Feedback Themes:
{{step_4}}

Next, delve into discussing the specific product features that received positive feedback based on {{positive_features}}. Also, provide context from automotive car-related aspects that customers found appealing.

->>>>

We have evaluated the positive product features:

Feedback Themes:
{{step_4}}

Positive Features:
{{step_5}}

Now, elaborate on the product features that received negative or constructive feedback with a focus on {{negative_features}}. Discuss specific aspects that automotive customers felt were lacking in detail.

->>>>

The detailed report includes a section on negative product features:

Feedback Themes:
{{step_4}}

Positive Features:
{{step_5}}

Negative Features:
{{step_6}}

According to the insights obtained from feedback, draft specific recommendations to enhance product offerings or marketing strategies. This should focus on {{improvement_areas}}.

->>>>

The compiled report now carries recommendations for improvement:

Positive Features:
{{step_5}}

Negative Features:
{{step_6}}

Improvement Recommendations:
{{step_7}}

Conclude the report now by summarizing the main points and reiterating the vital role of customer feedback within automotive product marketing.

->>>>

We now have a conclusion added to our report:

Improvement Recommendations:
{{step_7}}

Conclusion:
{{step_8}}

The final touch requires adding a section for 'Additional Notes'. This section will encapsulate less frequent but equally relevant comments from customers about {{product_focus}}.


```

