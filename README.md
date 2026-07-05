# SuiteThrottle Pricing Data

This repository hosts the dynamic pricing configuration for SuiteThrottle, the cache-aware FinOps governor for AI coding assistants.

The pricing.json file dictates the multiplier ratios for usage-based billing (UBB) across various models (e.g., Anthropic, OpenAI). The SuiteThrottle VS Code extension fetches this file dynamically to ensure developers always have the most accurate, up-to-date cost estimates before executing a prompt.

# Why is this public?

Transparency. Developers shouldn't have to guess how their meter is calculated. By keeping the multipliers here, the community can verify the exact tier costs SuiteThrottle uses to calculate the 90% prompt-caching discounts and 81x model deltas.

# Custom Internal Pricing

If your Enterprise uses custom negotiated rates or private model endpoints, you do not need to fork this repository. You can override these public multipliers entirely using the suitethrottle.customModels setting directly inside your VS Code settings.json.
