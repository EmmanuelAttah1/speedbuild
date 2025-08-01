# SpeedBuild

**Stop rebuilding what already works.**

Reuse full-stack features with one command. No boilerplate. No bugs. No copy-paste.
SpeedBuild lets you extract full Django features (views, models, templates, configs, dependencies) from your own projects and redeploy them into new ones. Think of it as Copilot for reusable code features, not just single lines.

[![Alpha Launch](https://img.shields.io/badge/Status-Alpha%20Launch-orange)](https://speedbuild.dev)
[![Open Source](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Django](https://img.shields.io/badge/Framework-Django-092E20?logo=django)](https://djangoproject.com)


## How It Works

### 1. **Extract Complete Features**
Our AST-powered engine traces every dependency of a feature, from database models to middleware configurations—ensuring nothing is missed.

### 2. **Adapt with AI** 
Describe your requirements in plain English. SpeedBuild intelligently modifies the extracted code to fit your project's architecture.

### 3. **Deploy Production-Ready Code**
Get complete, working features with proper package installations, configurations, and framework integrations.

# Quick Start
1. Install SpeedBuild
```bash
pip install speedbuild
```

2. Setup your environment
```bash
speedbuild setup
```

Follow the prompts to authenticate and configure your workspace.

3. Extract a feature from your project
```bash
speedbuild extract shop/views.py CheckoutCart
```

This saves a reusable feature template from the CheckoutCart view and all its dependencies.

4. Deploy the feature in a new project
```bash
speedbuild deploy speed_build_InitiatePayment
```

SpeedBuild scans your current project structure and adapts the feature intelligently.

5. Undo the last deployment (if needed)
```bash
speedbuild undo
```

6. See all Extracted Features
```bash
speedbuild list
```

Your project is restored to its previous state.

## What is a SpeedBuild Feature?
A SpeedBuild feature is a reusable, production-ready implementation of a common app logic, such as:
- User authentication with Google or email/password


- Payment integration with Stripe or Paystack


- Custom checkout or dashboard logic


- Notifications system (emails, webhooks, etc.)

- Or custom logic


It includes logic, middleware, configs, templates, dependencies — everything wired up and deployable with one command.

### How Adaptation Works
SpeedBuild doesn't just copy files — it intelligently adapts features to your current project using AI:
It scans the current folder structure and settings.


It uses an LLM (you configure the key) to modify the feature code to match your environment.


It automatically adds packages, modifies settings, wires routes, and aligns file structure.


Example customization (plain English prompt):
>_ Register all models to the admin panel

SpeedBuild rewrites the feature to register every model using Django admin.
Your LLM key is stored locally. SpeedBuild respects your privacy.


## Supported Frameworks

- ✅ **Django** - Full support
- 🚧 **Flask** - Coming Q3 2025
- 🚧 **FastAPI** - Coming Q3 2025


## Coming Soon: SpeedBuild Cloud
Collaborate with other developers via:
Public & private template repositories


Semantic feature search ("Add Stripe subscriptions")


Team sharing, roles, and usage tracking


## Why SpeedBuild?

### vs. Copy-Paste Development
- **SpeedBuild**: Complete features with all dependencies
- **Copy-Paste**: Missing configs, broken imports, hours of debugging

### vs. AI Code Generation
- **SpeedBuild**: Battle-tested, production-proven features
- **AI Generation**: Untested code that breaks under load

### vs. Starting from Scratch
- **SpeedBuild**: Deploy in minutes with proven patterns
- **From Scratch**: Days of development, repeated mistakes


# Contributing
SpeedBuild is free and open source. Star us on GitHub and contribute to the growing feature hub!
[github logo] github.com/EmmanuelAttah1/speedbuild

### Development Setup

```bash
git clone https://github.com/EmmanuelAttah1/speedbuild.git
cd speedbuild
pip install -r requirements.txt

#run as package
python -m speedbuild.sb
```

## License

MIT License. See [LICENSE](LICENSE) for details.

## Support

- 📖 **Documentation**: [docs.speedbuild.dev](https://app.speedbuild.dev/doc)
- 🐛 **Issues**: [GitHub Issues](https://github.com/EmmanuelAttah1/speedbuild/issues)
- 📧 **Email**: hello@speedbuild.dev

## Alpha Launch

SpeedBuild is launching in alpha! [Sign up for early access](https://app.speedbuild.dev/register) and help us build the future of code reuse.

---

**Built by developers, for developers.** Stop rebuilding. Start reusing.

[Get Started](https://speedbuild.dev) • [Documentation](https://app.speedbuild.dev/doc)

