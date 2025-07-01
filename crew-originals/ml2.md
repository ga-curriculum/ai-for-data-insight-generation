# Evaluating and refining AI-generated charts

## Why evaluating GenAI charts matters

Generating charts with an AI assistant can accelerate your workflow and unlock creative ways to explore data. However, speed alone does not guarantee clear, accurate, or actionable visuals. As data professionals, we must ensure that every chart we share truly reflects our data and communicates insights effectively.

Imagine that an AI assistant is like a co-pilot—it can create an initial draft, but it will not always know the full business context or the best way to answer your question. Your expertise brings that final level of precision and business relevance.

> 💡 Even the most sophisticated automation cannot replace your understanding of your company's goals, your stakeholders' needs, and the critical “so what?” behind every chart.

tktk asset: Illustration showing a "human plus AI" collaboration at a desk—one person reviewing a generated chart.

## A practical rubric for reviewing AI-generated charts

To assess charts efficiently and systematically, use a three-part rubric: accuracy, clarity, and insight value. This framework helps you quickly spot issues and guide improvements.

### 1. Accuracy: Are the data and details correct?

Accuracy is the foundation of any effective chart. If key numbers, timeframes, or categories are wrong, any insights may be misleading.

- Does the chart show the correct subset of the data (date range, filters, grouping)?
- Are calculations (such as sums, averages) performed as intended?
- Are axis and legend labels precise, including units?
- Did the AI assistant follow your prompt, or did it make assumptions?

> ⚠ A chart showing annual sales totals instead of “Q4 only,” when you specifically asked for Q4, could lead to incorrect business decisions.

*Real-world example:*  
A product manager asks for a chart of "active users by month for Asia Pacific in the latest quarter." The AI assistant instead shows data for all regions. This could cause the team to miss trends relevant to their market.

### 2. Clarity: Is the chart understandable at a glance?

Clarity ensures your stakeholders can interpret the visualization without confusion.

- Does the title reflect the specific question or focus?
- Are labels and legends clear, using plain language and appropriate units?
- Is the chart free of visual clutter, such as overlapping lines or colors that are difficult to distinguish?
- Is the formatting accessible for all audiences (font size, color contrast)?

> 💡 Think of clarity like signs in an airport. If you have to stop and puzzle over the directions, you might end up lost.

*Analogy:*  
A well-labeled chart is like a clearly marked map—any reader should be able to find the "destination" insight quickly.

### 3. Insight value: Does the chart answer the business question?

A chart should not only display information—it should help drive a decision.

- Does the visualization directly address your or your stakeholders' needs?
- Can a viewer easily identify trends, differences, or outliers?
- Is it obvious what action or conclusion should follow from viewing the chart?

*Practical example:*  
If you present a pie chart with many small, similar slices for regional sales, it may technically display all values but fail to reveal which region is leading. Instead, a sorted bar chart could highlight the highest-performing area.

> 🏆 High-impact charts make the key insight “pop,” so anyone—from senior leaders to frontline teams—can act on it.

tktk asset: Side-by-side example of an overloaded pie chart and a clear, sorted bar chart with annotations.

## Spotting issues: A sample GenAI chart in action

Let’s apply the rubric with an example scenario relevant to your daily tasks.

You prompt your AI assistant:  
"Create a bar chart showing total revenue by customer segment for the latest quarter using the uploaded CSV."

The AI assistant generates a chart with these features:

- Title: "Revenue by Segment"
- Bars labeled as “A,” “B,” and “C”
- No date range noted anywhere
- Y-axis labeled only as "Revenue"
- No legend

Let’s break down what stands out:

- **Accuracy:** Are "A," "B," and "C" correct codes for customer segments, or should these be descriptive names? Did the chart use the right time period (the latest quarter), or is it displaying data from the whole year?
- **Clarity:** The title is generic; it would be clearer as "Total Revenue by Customer Segment – Q4." The Y-axis needs a unit, such as “Revenue (USD).”
- **Insight value:** If "C" is much taller than the other bars, that's valuable—unless the segments are not properly labeled and the viewer cannot tell which is which.

> 💡 Ask yourself: If I presented this chart during a business meeting, would my colleagues know what to do next and trust the results?

## How to refine GenAI charts for better results

Once you spot opportunities for improvement, the next step is to communicate specific refinements to your AI assistant or adjust the chart directly.

### Write focused follow-up prompts

You do not need to start from scratch. Point out what should change and build on the existing output.

Prompt examples:

- “Update the chart to show only data for the latest quarter.”
- “Replace the labels ‘A’, ‘B’, and ‘C’ with the full customer segment names: ‘Enterprise’, ‘Small Business’, ‘Consumer’.”
- “Add a chart title: ‘Total Revenue by Customer Segment – Q4’. Label the y-axis as ‘Revenue (USD)’.”

### Adjust formatting for clarity and accessibility

You can address readability and presentation by specifying details in your prompt.

- “Increase the size of the labels for better readability.”
- “If any category names are long, rotate the x-axis labels for clarity.”
- “Limit the chart to show only the top five customer segments by revenue, grouping others as ‘Other’.”

### Request annotations and summaries

Help your audience quickly notice key takeaways.

- “Highlight the segment with the highest revenue.”
- “Add a brief summary below the chart explaining which segment performed best and by how much.”

> 🧠 Many AI assistants can provide the code behind the chart, allowing skilled users to make direct changes for even greater customization.

*Example with code context:*

Suppose you need to modify labels or customize formatting in Python using matplotlib.

my/path/to/script.py

python
import matplotlib.pyplot as plt

# Example lists of names and revenues
segment_names = ['Enterprise', 'Small Business', 'Consumer']
revenues = [42000, 25000, 17000]

plt.bar(segment_names, revenues)
plt.title('Total Revenue by Customer Segment – Q4')
plt.xlabel('Customer Segment')
plt.ylabel('Revenue (USD)')
plt.xticks(rotation=45)
plt.show()

> 💡 Making small code changes gives you extra control—especially if you plan to reuse or share charts across projects.

tktk asset: Annotated screenshot showing before-and-after versions of a GenAI-generated chart with prompt refinements.

## Guided practice: Evaluate and enhance an AI-generated chart

**Purpose:**  
Apply the rubric to a GenAI-generated chart and practice refining it to boost accuracy, clarity, and business insight.

### Instructions

1. **Download the provided sample CSV dataset** from your course resources.

2. **Review the dataset** to get familiar with available columns (such as dates, regions, customer segments, and revenue).

3. **Use your AI assistant** to upload the dataset and prompt it to create a chart.
    - For example:  
      “I have uploaded a CSV with sales data. Please create a bar chart showing total revenue by region for the latest month. Show the chart and provide the code you used.”

4. **Examine the chart output.** Use the quick-check rubric:
    - *Accuracy*: Are the data, filters, and labels correct?
    - *Clarity*: Are titles, labels, and formatting informative and readable?
    - *Insight value*: Does the chart directly answer your business question?

5. **Identify at least two areas to improve.** Examples might include missing date ranges, unclear category names, or lack of units.

6. **Write and submit follow-up prompts** to address these areas.
    - Examples:  
      “Update the title to: ‘Total Revenue by Region – May’. Label the y-axis as ‘Revenue (USD)’. Clarify region names if needed.”

7. **Iterate as needed.** If you want to make direct changes, request the Python or Plotly code and apply a small customization—such as adjusting colors or sorting the regions.

8. **Save both the initial and improved charts** for comparison.

9. **Summarize your final insight** in one or two sentences. For example:  
   "In May, the Asia-Pacific region generated the highest revenue, nearly double that of other regions."

- **Mini-challenge:**  
  Try applying the rubric to a different chart type (such as a line chart or pie chart) with your dataset. What new adjustments or prompts do you find are required?

tktk asset: Worksheet for chart evaluation, including a prompt refinement template and sample dataset snippet.

### Chat prompt:  
After making refinements, discuss in your learning group or add your reply to the discussion board:

- What was the most impactful change you made? How did it improve the chart?
- Did your refinements reveal a new insight or correct a misunderstanding from the original chart?
- How could you use this structured review and feedback approach in your everyday work with AI-powered data visualization tools?

tktk asset: Example learner submission—before-and-after chart images with insight summary.

---

## Instructor guide

### Delivery tips

- Model the evaluation process by walking through a GenAI-generated chart, thinking aloud as you apply the rubric.
- Encourage learners to focus on real-world context—prompt them to consider a stakeholder or business scenario as they review and refine charts.
- Support all learners in formulating clear follow-up prompts. Where possible, demonstrate both prompt-based and code-based refinements.
- Reinforce that the goal is not to criticize the AI assistant, but to bring charts to a business-ready standard with human judgment.

### Knowledge check discussion—suggested points

- Strong refinements usually clarify chart titles, labels, and ensure the visualization truly reflects the filtered data of interest.
- Encouraging learners to use the rubric repeatedly often uncovers subtle issues in dataset grouping, labeling, or presentation that could impact business interpretations.

### Suggested activity solution

**Example:**

- Initial chart: Bar chart titled "Revenue by Segment". Axes are missing units, and labels use codes "A", "B", "C". No date range.
- Issues: Lack of clarity on time frame; ambiguous segment labels; insufficient insight for decision-making.
- Refinements:
    - Update title to "Total Revenue by Customer Segment – Q4".
    - Replace labels with descriptive names ("Enterprise", "Small Business", "Consumer").
    - Add unit to the y-axis ("Revenue (USD)").
    - Prompt to highlight the highest segment.

- Sample insight summary: "In Q4, the Enterprise segment accounted for the highest revenue, suggesting a focus area for the next quarter."

tktk asset: Instructor slide deck including sample rubric, example charts at each refinement step, and discussion facilitation prompts.

---