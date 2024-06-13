# Conference Notes

## 9:30 AM: Space Force Analytics

### Summary:
- Represented the experiences of a single person and not the whole of org.

### Key Requirements:
- He wants NiFi
- He has Databricks, AWS, PalantirFoundry

### Foundry Features:
- Quick metrics
- Includes RDBMS
- Main development platform
- DAG implementation
- Cleaned datasets

### Projects & Tools:
- PM tool: Jira
- Reporting/Workflow management
- Total Force Awareness tools
- Rapid prototyping

## 10:30 AM: Unleashing AI on Your Data (MicroStrategy)

### Summary:
- This was very much an advertisement for MicroStrategy but it was well done
- Discussion about their new MicroStrategy AI Suite, specifically about the conversation of raw data to dashboards.

### Presenters:
- Aaron Ehrlich
- Christopher Seven

### Key Topics:
- Business Intelligence (BI)
- AutoSQL, Dashboard, Answer, Bot, Bot on Mobile
- AI/ML Challenges and Tools for Data Quality

### Highlights:
- “Information is like water”: How to turn it into a utility?
- Showed a graph relating AI and BI: Y axis = smart, X = precise. AI is high on Y, BI is high on X. Combined, they are more than their sums.
- Not good enough to be right 95% of the time.
- Uses Azure on backend.
- Dashboards creation from datasets.

### Key Questions:
- How to use PCA to determine important features?
- PCA = feature reduction. Not aware how to use it in this way.
- Use case for Metro: Forecasting ridership using standard time series components.
- Comparison: OAI Data Studio vs. MicroStrategy Auto?

### Resources:
- MicroStrategy Express

## Writing an AI Data Strategy

### Summary:
- Boss tells you to write a three year AI strategy, how do you proceed?
- Overall model: Ginormous datasets -> AI Model -> Domain data -> Prompts
- Minimize the amount of time leadership needs to operate on faith.
- “Strategy without a timeline is a dream.”
- Find allies. When you think of “we” and “them”, your allies are in the “we” group.

### Key Points:

#### Strategy Development:
- Business strategies should be in place; create if they don't exist.
- Focus on data with the fastest payback to drive growth.
- Costs are often front loaded (talent, IT, data prep).
- Benefits are often ethereal.
- Decision maker turnover is a risk.
- Incremental delivery for learning and financial gain.
- Strategies have a temporal component. Right strategy for right time.
- “Your proposed partner is under indictment…” = ☹

#### Quotes:
- "Victorious strategist only seeks battle after victory is assured."
- "Strategy without a timeline is a dream."

#### Frameworks:
- Porter's 5 Forces
- Diffusion of Innovation
- Blue Ocean Strategy
- R/W/W - Real/Win/Worth It
- Three Horizons Model
- 2x2 Matrix and derivatives

#### Data Strategy Components:
- Domain expertise, friction (governance/policies), reputation, and value.
- AI experts are good, domain experts are good.
- If it’s the same individual? You are on the fast track.
- Often easier to teach AI to domain expert than vice versa.
- Does data have a reputation with executives? Real vs perceived veracity.
- Focus on cost reduction, mundane tasks, process improvements.
- Hint: Look at your BI processes.
- Avoid blindly automating processes. Focus on what you start and end with.

#### Execution Challenges:
- Your competition is sometimes the “next best idea.”
- Be aware of this and ensure you can speak to them.
- Data cleaning is subjective and variable.
- Do not focus on this in initial stages.
- Consider multiple sources and governance issues.
- Focus where Human Intelligence (HI) is limited.
- Identify “learning targets”. Where can you pivot, how long will it take to pivot?
- Product management is important, keep it in mind, but don’t fixate on it.

#### Conclusion:
- Business strategy guides impact.
- Early, frequent delivery drives learning and funding.

## LLM’s: Good, Bad and the Ugly

### Summary:
Justin Grammens: Founder/CEO Lab651

#### LLM Positive Use Cases:
- Content generation
- Language translation
- Learning and Research
- Role Playing

#### LLM Challenges:
- Fixed Knowledge Base
- Understanding context
- Conversation continuity (ie “next work generation”)
- Dependence on user input: How do you ask the right question?

#### What Makes Something Open Source?
- Sharing code and weights
- Permissive license
- Community driven
- Transparency

#### Benefits of Open Source:
- Control and customization
- Cost effectiveness (generally free/low cost)
- Transparency and trust

#### Challenges of Open Source:
- Computational intensity
- Consider focusing on narrow slice of domain to help counter this
- Lack of critical support (or erratic support)
- Integration challenges

#### The “Ugly” of Open Source:
- Security risks (i.e. malicious contributions)
- Ethical/legal considerations (what will be the output?)
- Licensing (understanding the terms)

#### Methods to optimize LLM’s:
- Fine tuning (i.e. Lora): Train the model
- Prompt tuning (creating soft prompts): Train the prompt, not the model
- Prompt Engineering: Train the user, not the model or prompt
- RAG: Model + external retrieval system

Example: RagFlow

#### Use cases:
- Need up to date info (law, medicine)
- Task specific (understand legal document, generating marketing copy)
- Need deterministic output

#### Benefits:
- Optimize based on authoritative KB’s
- Attribute sources more easily

## Hugging Face

### Summary:
- One click deploys (related: HF Spaces)
- Easy to bring into Notebook

#### Links:
- Blog.n8n.io
- AppliedAI.mn

## Streamlining Support Ticket Management with Generative AI

### Summary:
Wissal Jawad @ Element

- Topic was classifying incident tickets into predefined categories. Used llama 2 with the appropriate prompting to automate this process. Dataset was a public domain set of about 26 incidents. The slides were presented in quick succession which made it difficult to take notes, so at some point I took pictures – which are included below.
- ![Slide 1](image1.jpg)
- ![Slide 2](image2.jpg)
- ![Slide 3](image3.jpg)
- ![Slide 4](image4.jpg)

## Bridging the Gap - Meghan Miller

### Summary:
- Intelligent communication increases efficiency, engagement, job satisfaction. Importance of research before conversations and practical outcomes. Different communication styles and levels needed for various audiences (execs, managers, general).

#### Common Communication Pitfalls:
- Too detailed or high-level
- Lack of tangible milestones and clear objectives
- Inadequate presentation skills

#### Best Practices:
- Start with impact and takeaway
- Avoid acronyms
- Tailor messages to leadership levels

#### Conclusion:
- Empathy and understanding are crucial. Know your audience and avoid technical jargon.

## MLOPS - Justin Leighton

### Summary:
- Train, deploy, monitor models in production. High failure rate for models reaching production.

#### DS vs. Analytics Differences:
- Organizational structure and specialization.
- Domain skills are critical for engineers.

#### Steps to Production:
- Modularize code
- Standardize file structures
- Write tests and apply linting
- Containerize with Docker
- CI/CD pipeline integration

#### Deployment:
- Use FastAPI, Flask, Airflow, or cron for tasks.
- Deploy to Kubernetes clusters or platform services.

#### Monitoring:
- Uptime and log monitoring for engineering.
- Model performance (drift) for data science.

#### Recommended Books:
- Effective Python
- Building Intelligent Systems
- ArjanCodes (resource)

## References:

MicroStrategy AI Suite vs OpenAI Data Studio

When comparing dashboard creation between MicroStrategy and OpenAI Data Studio, several key differences emerge based on their respective design philosophies, user experiences, and capabilities:

### MicroStrategy

#### Advanced Customization and Flexibility:
- Complex Visualizations: MicroStrategy supports highly customizable dashboards with a wide range of built-in and third-party visualizations. Users can create sophisticated reports and data visualizations, including maps, graphs, and grids, tailored to specific business needs​.
- Detailed Data Integration: It allows for complex data integrations and multi-source data blending, making it suitable for organizations that need to handle large and diverse data sets​.
- Intuitive Interface: The platform provides an intuitive drag-and-drop interface for dashboard creation, but it is also equipped to handle more technical requirements, such as OLAP (Online Analytical Processing) and advanced SQL queries​.
- Enterprise Features: MicroStrategy excels in offering enterprise-level features, such as role-based access control, mobile access, and extensive collaboration tools, which are critical for large organizations​.

#### AI Integration:
- AI-Enhanced Analytics: MicroStrategy integrates AI capabilities to enhance its BI functionalities, including automated insights, predictive analytics, and natural language processing for easier data querying and report generation​.

### OpenAI Data Studio

#### Simplicity and Ease of Use:
- User-Friendly Design: OpenAI Data Studio emphasizes ease of use with a focus on democratizing data access. Its interface is designed to be intuitive, allowing users with minimal technical expertise to create and customize dashboards effectively​.
- No-Code/Low-Code Approach: The platform supports a no-code/low-code environment, making it accessible for users to generate dashboards without deep technical knowledge. This approach is beneficial for organizations looking to enable more team members to engage with data without extensive training​.

#### AI and Natural Language Processing:
- Generative AI: OpenAI Data Studio leverages generative AI to simplify dashboard creation. Users can interact with the platform using natural language prompts, making it easy to generate and modify reports and visualizations based on conversational inputs​.
- Real-Time Data Insights: The integration of AI capabilities allows for real-time data analysis and insights, helping users quickly understand and visualize data trends and patterns without extensive manual intervention​.

### Key Differences in Dashboard Creation
- Customization vs. Simplicity: MicroStrategy offers deep customization and is well-suited for complex, enterprise-level dashboard needs. It provides advanced features that require a certain level of technical expertise. In contrast, OpenAI Data Studio focuses on simplicity and ease of use, leveraging AI to make dashboard creation more accessible to non-technical users.
- Integration and Data Handling: MicroStrategy's robust data integration capabilities make it ideal for organizations with diverse and complex data environments. OpenAI Data Studio, while capable of integrating various data sources, emphasizes ease of use and rapid deployment of AI-driven insights.
- User Experience: MicroStrategy provides a feature-rich, flexible environment that can cater to detailed and specific business requirements, whereas OpenAI Data Studio aims to simplify the process with an intuitive, AI-powered interface that lowers the barrier to entry for data analysis and visualization.

In conclusion, for organizations requiring highly customized, enterprise-grade dashboards with extensive data integration, MicroStrategy is the preferred choice. On the other hand, for those seeking a more user-friendly, AI-driven solution for quick and easy dashboard creation, OpenAI Data Studio offers a compelling alternative.
