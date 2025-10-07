# TD AI Threat Models

![td-ai](assets/td-ai-part3.png)

A comprehensive collection of Threat Dragon threat models enhanced with AI-generated threat analysis from multiple leading AI providers. Whether you're exploring AI-assisted security analysis or looking for practical threat modeling examples, this repository has you covered.

## Overview

Here you'll find threat models created using [Threat Dragon](https://owasp.org/www-project-threat-dragon/) - the popular open-source threat modeling tool - but with a twist: we've enhanced each model with AI-generated threat analysis from top AI providers including Anthropic, OpenAI, Google, xAI, and Novita. These models span various system architectures, showing you firsthand how AI can revolutionize traditional threat modeling practices.

## AI Threat Generation Tool

**Every single threat model you see here was created using the [td-ai-modeler](https://github.com/InfosecOTB/td-ai-modeler) - a powerful tool that leverages Large Language Models (LLMs) to automatically analyze your system components and generate comprehensive security threats with mitigation strategies for Threat Dragon models.**

### What makes td-ai-modeler special:

- **AI-Powered Threat Generation**: Harnesses cutting-edge LLMs to dive deep into your system components and uncover security threats you might have missed
- **Flexible Threat Framework Support**: Built for STRIDE, but easily adaptable to other threat modeling frameworks
- **Multi-LLM Support**: Works with all the major players - OpenAI, Anthropic, Google, xAI, and even local Ollama setups thanks to the LiteLLM library
- **Seamless Threat Dragon Integration**: Plays perfectly with Threat Dragon JSON models - no compatibility headaches
- **Smart Filtering**: Automatically knows which components to focus on and which to skip
- **Rock-Solid Data Validation**: Built-in Pydantic validation ensures your threat data is always clean and consistent
- **Thorough Response Validation**: Double-checks AI responses against your original models to catch any discrepancies
- **Detailed Validation Logging**: Timestamped logs with comprehensive coverage reports so you know exactly what happened
- **Visual Indicators**: Automatically highlights components with threats using red strokes - no manual work needed

### AI Providers we've tested with:
- **OpenAI**: GPT-5, GPT-5 Mini
- **Anthropic**: Claude Opus 4.1, Claude Sonnet 4.5
- **Google**: Gemini 2.5 Pro
- **xAI**: Grok-4 (latest and fast-reasoning variants)
- **Novita**: DeepSeek R1, DeepSeek V3.1 Terminus, Qwen3 Coder
- **Ollama**: Gemma 3 27B (perfect for local deployments)

Want to try it yourself? Check out the [official repository](https://github.com/InfosecOTB/td-ai-modeler) for detailed setup instructions and documentation.

## Repository Structure

We've organized this repository into three distinct threat model categories, each showcasing different types of systems:

### 1. InfoSecOTB (Infosecotb.com)
**Location:** `1_infosecotb/`

This one's a real-world example: a cybersecurity blog platform running on WordPress with an integrated AI-powered chatbot. Perfect for understanding threats in content management systems with AI integration.

**What's inside:**
- WordPress CMS hosted on BlueHost
- vMeNext AI chatbot powered by OpenAI GPT
- Blog content management and user engagement features
- Social media integration and search functionality

### 2. Husky AI
**Location:** `2_husky-ai/`

Here's something fun but educational: a machine learning system that can tell the difference between huskies and other dogs. This model is great for understanding threats in ML/AI systems with proper security practices.

**The tech stack:**
- Convolutional Neural Network (CNN) for image classification
- Azure Cognitive Services for image retrieval
- Azure Blob Storage with RBAC/ABAC access controls
- Jupyter Notebook development environment
- Production deployment with API Gateway

### 3. Online Payments Processing Platform
**Location:** `3_online-payments-processing-platform/`

Based on the OWASP Threat Model Cookbook example, this one tackles the critical world of e-commerce payment processing. It's a must-see for anyone dealing with payment security.

**What you'll learn about:**
- Customer-merchant interaction flows
- Stripe payment integration
- OAuth authentication
- Secure payment processing workflows

## AI Provider Analysis

Each threat model comes with AI-generated threat analysis from multiple providers, so you can see how different AI models approach the same security challenges:

- **Anthropic**: Claude Opus 4.1 and Claude Sonnet 4.5
- **OpenAI**: GPT-5 and GPT-5 Mini
- **Google**: Gemini 2.5 Pro
- **xAI**: Grok-4 (latest and fast-reasoning variants)
- **Novita**: DeepSeek R1, DeepSeek V3.1 Terminus, and Qwen3 Coder
- **Ollama**: Gemma 3 27B (for Husky AI)

## File Formats

You'll find each AI-generated threat model in two handy formats:
- **JSON**: Raw Threat Dragon format - perfect for importing directly into Threat Dragon
- **PDF**: Human-readable reports - great for sharing with your team or stakeholders

## Getting Started

### What you'll need

- [Threat Dragon](https://owasp.org/www-project-threat-dragon/) (web or desktop version)
- A web browser for viewing PDF reports

### How to explore the models

**JSON Files**: Import these directly into Threat Dragon for interactive viewing and editing - you can even modify the threats and see how the AI analysis looks

**PDF Files**: Open these in any PDF viewer for clean, static documentation that's perfect for presentations

### Getting started with Threat Dragon

1. Head over to [Threat Dragon](https://www.threatdragon.com/#/)
2. Create a new model or open an existing one
3. Use the import feature to load any `.json` file from this repository
4. Dive in and explore the AI-generated threat analysis and diagrams

### Reproducing These Results

Want to create your own AI-enhanced threat models? The [td-ai-modeler tool](https://github.com/InfosecOTB/td-ai-modeler) makes it surprisingly straightforward.

For step-by-step setup instructions and detailed documentation, check out the [td-ai-modeler repository](https://github.com/InfosecOTB/td-ai-modeler).

## AI-Enhanced Threat Modeling

Here's how the [td-ai-modeler](https://github.com/InfosecOTB/td-ai-modeler) tool transforms traditional threat modeling:

- **Automated Threat Generation**: Let AI models dive deep into your system components and generate comprehensive threats using the STRIDE framework - no more manual brainstorming sessions
- **Comprehensive Threat Identification**: AI models catch threats that even experienced security professionals might overlook during manual analysis
- **Consistent Analysis**: Get standardized threat analysis across different system types and AI providers - no more inconsistencies
- **Multiple Perspectives**: See how different AI models approach the same system architecture - it's like having multiple security experts review your system
- **Automated Documentation**: AI generates detailed threat descriptions, mitigations, and visual indicators - your documentation practically writes itself
- **Quality Assurance**: Built-in validation ensures all generated threats meet Threat Dragon standards - quality is guaranteed
- **Scalability**: Process multiple threat models efficiently with different AI providers - scale your security analysis without scaling your team

## Contributing

This repository serves as a practical reference for AI-enhanced threat modeling. While these models are based on real or realistic scenarios, they're designed to be educational and help you understand how AI can enhance your threat modeling process.

## License

This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) file for details.

## Related Resources

- [Threat Dragon Official Documentation](https://www.threatdragon.com/docs/)
- [OWASP Threat Model Cookbook](https://github.com/wunderwuzzi23/threat-model-cookbook)
- [STRIDE Threat Modeling Framework](https://docs.microsoft.com/en-us/azure/security/develop/threat-modeling-tool-threats)

## Disclaimer

These threat models are designed for educational and demonstration purposes. While they provide valuable insights into AI-enhanced threat modeling, they shouldn't be used as the sole basis for security decisions in production systems. Always conduct thorough security assessments tailored to your specific use cases and environments.
