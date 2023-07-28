# Product Manager Feature Announcement Creator

Combat feature announcement fatigue with Product Manager Feature Announcement Creator. Our AI-powered tool crafts remarkable, easy-to-understand releases for new features in the Customer Service & Support Tools industry. Tailored for Product Managers, just specify variables and let AI furnish detailed info about the new feature, highlighting headline, overview, benefits, impact on user workflows or pricing, and available training. Unique to our app is its in-depth industry focus - delivering jargon-free, comprehensive content in a positive tone for maximum clarity and appeal.

To run this app online: [Product Manager Feature Announcement Creator Online](https://hero.page/app/product-manager-feature-announcement-creator-ai-powered-feature-announcement-expert/qApCofaqzKUmGApVQWik)

[![Run Product Manager Feature Announcement Creator Online](/assets/run.svg)](https://hero.page/app/product-manager-feature-announcement-creator-ai-powered-feature-announcement-expert/qApCofaqzKUmGApVQWik)

To learn more about AI Apps for Product Manager use-cases in the Customer Service & Support Tools industry, read [How to Streamline Customer Support with AI-Based Documentation Tools](https://hero.page/blog/ai/customer-service-and-support-tools/how-to-streamline-customer-support-with-ai-based-documentation-tools/170836)

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
npx hero run ./product_manager_feature_announcement_creator.heroml
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
hero run ./product_manager_feature_announcement_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./product_manager_feature_announcement_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./product_manager_feature_announcement_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./product_manager_feature_announcement_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

