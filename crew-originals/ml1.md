# Prompting GenAI for data visualization

## Connecting business questions to data visualizations

Every impactful data visualization starts with a meaningful business question. Identifying the right question ensures your visualization is not just displaying information, but guiding decisions.

Consider a common scenario for data professionals working in different organizations, such as a regional operations team, a global product manager, or a finance analyst examining quarterly data.

Suppose you manage sales data for several regions:

> **Business question:**  
> How have monthly sales trends changed across different regions in the past year?

From this question, it is clear that you are interested in comparing sales over time and across geographical areas. Highlighting these data dimensions helps guide the choice of chart and the type of prompt you will use with your AI assistant.

tktk asset: Diagram illustrating how a business question maps to data columns and potential chart types.

### Choosing the right chart type: Making it relatable

Selecting the appropriate chart type is crucial for clarity. Here is a simple guide that maps common business needs to chart types:

- **Trends over time:** Line or area charts
- **Comparing categories:** Bar or column charts
- **Part-to-whole relationships:** Pie or stacked bar charts
- **Analyzing relationships between variables:** Scatter plots
- **Exploring distributions:** Histogram or box plots

> 💡 Think of each chart type as a tool in a toolkit. Just as you would not use a hammer to turn a screw, choosing the wrong chart can make your insights less clear. For example, you would not use a pie chart to show changes over time.

tktk asset: Visual examples of different chart types, each labeled with common use cases.

If you want to show monthly sales for each region, a multi-line chart works well, where every line represents a region across the same timescale.

- **Discussion prompt:**  
What kinds of business questions do you encounter in your work that could be explored or communicated with the help of a chart?

## Crafting effective prompts for GenAI

AI assistants can be powerful partners in creating data visualizations—that is, when you provide clear and structured prompts. A high-quality prompt helps the AI generate output you can use in a business setting.

### What goes into a strong prompt?

To get the visualization you need, include these elements:

1. **Data context:** Briefly describe what is in your dataset. 
2. **Visualization request:** Specify the chart type and how it connects to your business question.
3. **Desired format:** Explain how you want to receive the result. 

Let’s look at these steps with a relatable example.

#### 1. Providing data context

When sharing your dataset, mention details such as the columns included and what they represent.

> For example:  
> “I have a CSV file with sales records. Columns: Date (YYYY-MM-DD), Region, Product, Sales Amount (USD). Each row is a sale.”

This prepares the AI assistant to interpret the data before generating a visualization.

#### 2. Stating the visualization request

Tell the AI assistant exactly what you want it to create.

> For example:  
> “Create a line chart showing total monthly sales per region over the last year.”

#### 3. Defining the output format

Decide how you want to receive the end result. Options may include:

- Rendered chart in the AI interface
- Code (often Python or Plotly) used to generate the chart
- Downloadable image (if supported)

> For example:  
> “Please return a rendered plot here and the Python code used to create the visualization.”

### Complete prompt example

Putting it together:

> “I have uploaded a CSV file with columns: 'Date' (YYYY-MM-DD), 'Region', 'Product', and 'Sales Amount' (USD). Please generate a line chart that shows the total sales amount per month for each region over the last year. Show the chart here, and provide the Python code you used.”

This prompt tells the AI assistant what you want, why you want it, and how you want to use it.

> 🏆 Best practice: If you are uncertain about the best chart type, ask the AI assistant for recommendations before generating the chart. For example:  
> “Based on this dataset, what types of charts would help me compare monthly sales across regions?”

tktk asset: Annotated screenshot of a clearly structured AI prompt and resulting chart.

- **Discussion prompt:**  
Have you tried creating a visualization from a verbose versus a brief prompt? How did the level of detail impact the output?

## Guided practice: Generating your first visualization with GenAI

Now, let’s connect these skills to your workflow. Imagine you are working for a retail company and want to understand recent revenue performance.

Suppose your dataset contains the following columns: Order Date, Country, Customer Segment, Revenue.

> **Business question example:**  
> Which customer segment generated the highest total revenue last quarter?

Following our steps:

1. **Data context:**  
   “I have a CSV file of retail transactions: Order Date, Country, Customer Segment, Revenue (USD).”
2. **Chart type:**  
   Bar chart (great for category comparisons).
3. **Output format:**  
   “Display the bar chart here.”

Full prompt:

> “I have uploaded a CSV file of retail transactions with columns: Order Date, Country, Customer Segment, and Revenue (USD). Please create a bar chart showing total revenue by customer segment for the most recent quarter. Display the chart here.”

- **Interaction point:**  
After running your prompt, review the visualization the AI assistant generates.

Consider these reflection questions:

- Does the chart answer your business question?
- Are the filters and labels correct?
- Is the visual easy to interpret?

tktk asset: Example output showing before-and-after code and chart for a basic prompt.

## Iterating your prompts to refine visualizations

Sometimes, your first visualization may not fully meet your needs. Fortunately, refining your prompt is quick and flexible.

Here are some common ways you might iterate:

- **Change the chart type:**  
  If viewing data as a bar chart is helpful but you want another perspective, try:  
  “Now, show this as a pie chart instead of a bar chart.”

- **Adjust chart labels or titles:**  
  Clarity matters for business communication. You might prompt:  
  “Update the chart title to ‘Total Revenue by Customer Segment (Q4),’ and label the y-axis as ‘Total Revenue (USD).’ ”

- **Add or change data filters:**  
  To narrow in on relevant insights:  
  “Only include customer segments with revenue above 10,000 and focus on India.”

- **Request code or exportable output:**  
  To reuse or share the visualization in presentations or reports:  
  “Export this chart as a PNG. Also, provide the Python code used to create it.”

> ♻️ Iterating on prompts is similar to refining a search or editing a report: each interaction brings you closer to a visualization that clearly communicates your insights.

- **Chat prompt:**  
List one change you might make to your initial chart to improve its clarity for stakeholders.

## Activity: Prompt, generate, and refine your own visualization

**Purpose:**  
Use an AI assistant to go from a business question to a refined, actionable chart. This practical exercise will help you experience the real-world workflow of generating and improving data visualizations with GenAI.

### Instructions

- **Download the sample CSV dataset** from your module resources.
- **Review the data** and note the columns and types of problems you could explore.
- **Write a business question**. For example:  
  “How did sales vary by product category last year?”
- **Select a chart type** that would help answer your question.
- **Draft a prompt** for the AI assistant, including:
    - Description of dataset columns and context
    - The chart type you want
    - How you want to receive the result (rendered, code, or image)
- **Upload your CSV** to the AI assistant and submit your prompt.
- **Review the generated visualization.**  
  Does it answer your business question? Are the labels, axes, and titles clear?
- **Iterate on your prompt** at least once. Try changing chart type, adding filters, or refining chart labels.
- **Save your final results**, including any code or images the AI provides.

- **Mini-challenge:**  
  In addition to your primary business question, try generating a second chart that looks at the data from a new angle. For instance, after visualizing total sales by category, you might visualize sales by country or quarter.

> ❓ Knowledge check:  
> In your own words, how does including details about your dataset in your prompt affect the visualization the AI assistant creates? What happens if you omit key context?

- **Discussion prompt:**  
After completing the activity, discuss with your peers or in the discussion forum:
    - How did the specificity of your prompt affect GenAI’s visualization?
    - What refinements made the biggest difference?
    - How might you tailor your approach when collaborating with different stakeholders?

tktk asset: Template for drafting and refining AI prompts for data visualization, with sections for dataset context, business question, chart type, and output request.

---

## Instructor guide

### Delivery tips

- Encourage learners to articulate their business questions before opening the AI assistant. This keeps the workflow focused on solving real problems.
- Model the process by showing both a strong, detailed prompt and a weaker, vague prompt, to help learners observe the difference in output.
- When learners iterate, prompt them to describe their reasoning (for example, “I added this filter to make the chart focus on the highest-value segments, which matters for our business case”).
- Allow time for participants to discuss how the process of refining prompts mirrors the feedback loop seen in business environments: quickly moving from draft visualization to stakeholder-ready chart.

### Knowledge check answer

Including detailed context (such as data columns, units, and relevant filters) in your prompt helps the AI assistant correctly interpret the data and generate a visualization that meets your needs. Omitting context often results in inaccurate or ambiguous charts.

### Suggested activity solution

Example:

- Dataset columns: Date (YYYY-MM-DD), Region, Product, Sales Amount (USD), Customer Segment
- Business question: Which region saw the highest sales growth over the year?
- Initial prompt:  
  “I have uploaded a CSV file with columns: Date, Region, Product, Sales Amount (USD), and Customer Segment. Please generate a line chart showing monthly sales for each region. Display the chart here and provide the Python code used.”
- Refinement: Add a focus on top regions, adjust chart title, or change chart type to bar chart for a different perspective.

---

tktk asset: Example of a refined data visualization, showing before-and-after changes resulting from iterative prompting.

> 🧠 Encourage learners to save and compare their prompts and results. This reflection can help them recognize effective patterns and improve future workflows.