## Strategy

* Always call a specialized agent if they can help in a task.

## Agent Usage Guidelines

Call specialized agents during planning and implementation when:

### Streamlit UX Architect Agent

* UI/UX design decisions and layout optimization
* Component selection and user flow design
* Dashboard structure and interface architecture
* User experience improvements and workflow design
* Multi-step process design and navigation

### Streamlit Data Visualization Expert Agent

* Advanced chart design with Plotly, Altair, and matplotlib
* Interactive visualization patterns and user engagement
* Data storytelling through visual hierarchy and flow
* Color theory, accessibility, and visual best practices
* Custom visualization components and animation techniques

### Streamlit Docs Analyzer Agent

* Understanding Streamlit features and capabilities
* Performance optimization and best practices
* Memory management and large dataset handling
* Component functionality and API usage
* Troubleshooting Streamlit-specific issues

**IMPORTANT**: When invoked, this agent should use `gemini -p "Analyze llms-full.txt and focus on [SPECIFIC_TOPIC] - provide detailed information about [USER_QUESTION]"` to get targeted insights from the comprehensive Streamlit documentation before providing guidance.

### Streamlit Performance Optimizer Agent

* Memory usage optimization and session state efficiency
* Caching strategies (st.cache_data, st.cache_resource)
* Large dataset handling and data chunking
* Component rendering speed and bundle size reduction
* Concurrent user session optimization

### Streamlit Deployment Specialist Agent

* Cloud deployment strategies (Streamlit Cloud, AWS, Azure, GCP)
* Docker containerization and orchestration setup
* CI/CD pipeline configuration and automation
* Environment management and secrets handling
* Scaling and load balancing for production apps

### Streamlit Security Auditor Agent

* Authentication and authorization implementation
* Secrets management and environment variable security
* Input validation and data sanitization practices
* HTTPS configuration and secure communication
* Compliance requirements and audit trail implementation

### Streamlit Testing Engineer Agent

* Unit testing strategies for Streamlit components
* Integration testing and end-to-end test automation
* Mock data generation and test fixture management
* Performance testing and load simulation
* Quality assurance workflows and regression testing

### Streamlit Data Pipeline Architect Agent

* ETL workflow design and real-time data integration
* Database connection optimization and query performance
* API integration and external data source management
* Data validation, transformation, and cleaning processes
* Streaming data handling and live dashboard updates

### Streamlit Multi-App Orchestrator Agent

* Multi-page application architecture and navigation
* Cross-page state management and data persistence
* App modularity and code organization patterns
* Dynamic routing and conditional page rendering
* User session management across application flows

### Streamlit Monitoring Specialist Agent

* User behavior tracking and engagement analytics
* Performance monitoring and error tracking integration
* A/B testing framework implementation
* Usage metrics collection and dashboard reporting
* Business intelligence integration and KPI tracking

### Streamlit AI Integration Specialist Agent

* LLM integration and prompt engineering strategies
* AI agent orchestration within Streamlit workflows
* Context window and memory management optimization
* Streaming responses, token counting, and latency mitigation
* Chat and Q&A interface implementation patterns

### Streamlit UI Customization Expert Agent

* Custom CSS and advanced theme configuration
* Brand identity implementation (logos, colors, fonts)
* Dark/light theme switching and accessibility compliance
* Corporate branding guidelines enforcement
* Responsive design optimization across devices

### Streamlit API Integration Architect Agent

* Third-party API connections and OAuth implementation
* Payment gateway integration (Stripe, PayPal, etc.)
* SaaS platform integrations (Google Workspace, Slack, Zapier)
* Webhook processing and external event handling
* Real-time data synchronization with external services

### Streamlit Report Generator Specialist Agent

* PDF generation via reportlab, weasyprint, or pdfkit
* Downloadable Excel, CSV, and HTML report creation
* Component screenshot and snapshot rendering
* Branded report templates and automated export workflows
* Multi-format document generation and delivery systems

### Streamlit State Management Specialist Agent

* Advanced session state patterns and cross-page synchronization
* Widget state management and data persistence strategies
* Complex workflow state machines and navigation control
* Multi-user session coordination patterns
* State preservation across app restarts and updates

### Streamlit Accessibility Compliance Expert Agent

* WCAG 2.1/2.2 compliance and 508 accessibility standards
* Screen reader compatibility and keyboard navigation optimization
* Mobile responsiveness and touch interface design
* Color contrast and visual accessibility auditing
* Assistive technology integration and testing

### Streamlit Component Builder Agent

* Custom React component development and packaging
* Frontend framework integration (Vue, Angular, etc.)
* Component lifecycle management and state handling
* Advanced widget creation and iframe communication
* Third-party library integration and wrapper creation

### Streamlit Enterprise Governance Specialist Agent

* Multi-tenant architecture and role-based access control
* Audit trails, compliance workflows, and governance policies
* Enterprise SSO integration and user management systems
* Regulatory compliance tracking and reporting
* Corporate policy enforcement and security governance

### Streamlit Realtime Streaming Architect Agent

* WebSocket integration and high-frequency data updates
* Message queue integration (Kafka, Redis Streams, RabbitMQ)
* Real-time dashboard optimization and performance tuning
* Asynchronous data processing and background task management
* Live data synchronization and conflict resolution

### General Purpose Agent

* Complex multi-step research tasks
* Code searching across large codebases
* File system exploration and pattern matching
* Cross-technology integration research

**CRITICAL**: Always consult the appropriate specialized agent during the planning phase for any task that falls within their expertise area, not just during implementation.

### WebSearch

When performing web searches, limit the number of queries to what is strictly necessary. Stop searching once sufficient context has been gathered to complete the task effectively.

## Gemini Assistant Integration

The `gemini` command is available as a powerful assistant tool with 1M token context size. Use it for:

- **Large file analysis**: When files are too large for efficient processing
- **Code generation**: Complex code generation tasks
- **File system operations**: Recursive file operations and analysis  
- **Content summarization**: Analyzing and summarizing large documents
- **Research tasks**: When you need an "intern" to process extensive content

### Usage Examples:
```bash
# Analyze files
gemini -p "Analyze this large file and summarize its key points"

# Generate code
gemini -p "Create a Python function that does X"

# File operations
gemini -p "Count all markdown files recursively and show their sizes"

# Get help
gemini help
```

### When to Use Gemini:
- Processing files > 50KB 
- Complex multi-file analysis
- When you need a second opinion on code
- Large codebase exploration
- Content generation tasks

Remember: Gemini has 1M token context, making it ideal for handling large files that would be impractical to process directly.

## Use Gemini as Your Intern

Treat gemini as a capable intern that can handle tasks requiring extensive context or processing:

- **Delegate large file analysis** instead of reading huge files yourself
- **Offload research tasks** that require processing multiple files
- **Use for initial code exploration** in unfamiliar codebases
- **Handle repetitive analysis** across many files
- **Process user-provided large documents** or datasets
- **Generate boilerplate code** for complex requirements

Think of gemini as extending your capabilities - use it proactively when you encounter tasks that would benefit from its large context window or when you need to process more information than is practical to handle directly.

