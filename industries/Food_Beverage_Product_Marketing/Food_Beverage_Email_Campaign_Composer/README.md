# Food & Beverage Email Campaign Composer

Make your food and beverage email marketing more effective and tailored with the Food & Beverage Email Campaign Composer. This innovative app utilizes AI technology to create high-quality, customized email content suitable for different seasons. Users can specify variables for personalized, engaging messages that include catchy subject lines, product details, usage suggestions, company updates, strong call-to-actions, and thank-you notes with occasional promo codes. It can also add a postscript for extra information. The app's unique factor lies in its focused approach to the food & beverage industry, incorporating industry-standard terminologies and seasonal references for maximum context and relevance. Its propelled understanding of this sector makes every campaign effective, industry-specific, and timely, catering precisely to your subscribers.

To run this app online: [Food & Beverage Email Campaign Composer Online](https://hero.page/app/food-and-beverage-email-campaign-composer-customized-seasonal-food-and-beverage-marketing/mm87GRvrAL4zK8dAUl4Q)

[![Run Food & Beverage Email Campaign Composer Online](/assets/run.svg)](https://hero.page/app/food-and-beverage-email-campaign-composer-customized-seasonal-food-and-beverage-marketing/mm87GRvrAL4zK8dAUl4Q)

To learn more about AI Apps for Product Marketer use-cases in the Food & Beverage Product Marketing industry, read [How to Revamp Food & Beverage Marketing with AI Tools](https://hero.page/blog/ai/food-and-beverage-product-marketing/how-to-revamp-food-and-beverage-marketing-with-ai-tools/170882)

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
npx hero run ./food_and_beverage_email_campaign_composer.heroml
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
hero run ./food_and_beverage_email_campaign_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./food_and_beverage_email_campaign_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./food_and_beverage_email_campaign_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./food_and_beverage_email_campaign_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

