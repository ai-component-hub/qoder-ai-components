---
name: 'azure-prices'
description: 'Look up and compare Azure service pricing using the Azure Retail Prices'
adopted: 2026-05-16
API. Use this skill whenever the user asks about Azure costs, pricing, rates, or
wants to compare prices across regions or servi
source: awesome-copilot-agents
tier: 1
---

# azure-prices

Look up and compare Azure service pricing using the Azure Retail Prices API. Use this skill whenever the user asks about Azure costs, pricing, rates, or wants to compare prices across regions or servi

## When to Use

- Use this skill when working on tasks related to azure prices
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot-agents

## Workflow

The npm commands below are the preferred execution path for this skill and should be used instead of direct API calls whenever command execution is available.

### Single region lookup

Run the script with the service name and region. Present results in a readable table.

### Cross-region comparison

To compare prices across regions, run the script multiple times — once per region — then combine the results into a comparison table. For example, to compare Virtual Machines prices across three regions:

```bash
npm run --prefix ./scripts get-prices -- "Virtual Machines" eastus
npm run --prefix ./scripts get-prices -- "Virtual Machines" westus2
npm run --prefix ./scripts get-prices -- "Virtual Machines" westeurope
```

Then join the results by SKU name to show a side-by-side comparison table with columns for each region.

### Finding the cheapest region

Run prices for the target service across several common regions and sort by price. Common Azure regions to compare:

- `eastus`, `eastus2`, `westus2`, `centralus` (US)
- `westeurope`, `northeurope`, `uksouth` (Europe)
- `southeastasia`, `eastasia`, `japaneast` (Asia-Pacific)

### Service discovery

If the user isn't sure of the exact service name, run the script with no arguments first to get a sample of available names, then use the closest match.

## Source

This skill was adopted from open-source repository: awesome-copilot-agents
Original path: azure-prices
