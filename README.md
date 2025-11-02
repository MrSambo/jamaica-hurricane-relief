# Jamaica Hurricane Relief

This repository contains product documentation and code for the Jamaica Hurricane Relief project, supporting two key platforms: **FieldTrack** and **Mana Relief**.

## Project Overview

This repository serves as the source of truth for product documentation, maintained as Markdown files, and will also contain the codebase for both relief platforms. Both projects are designed to address critical gaps in disaster response and recovery operations in Jamaica.

## Active Projects

### FieldTrack

**FieldTrack** is a bare-minimum mobile app that enables emergency response teams to track relief supply distribution to affected communities through an offline-first approach.

#### Platform Goals

* Eliminate critical relief supply misallocation and ensure accurate beneficiary service during field missions
* Establish foundation for scalable disaster relief distribution tooling
* Achieve 100% field team adoption within first distribution cycle
* Reduce distribution accountability overhead by 75% compared to manual processes

#### Key Features

* **Offline-First Operation**: Full functionality without internet connectivity using local device storage
* **Relief Supply Registry**: Create, edit, and track supply records with inventory management
* **Distribution Team Management**: Role-based access (Site Manager, Distribution Lead, Team Member) with batch distribution capabilities
* **Beneficiary Tracking**: Record individual or family unit service within distribution events
* **Data Export**: Comprehensive CSV export for accountability reporting and aid organization coordination

📖 **Documentation**: See [`product-docs/fieldtrack/prd-fieldtrack.md`](./product-docs/fieldtrack/prd-fieldtrack.md) for complete details.

---

### Mana Relief

**Mana Relief** is a digital marketplace empowering international and Jamaican supporters to fund urgent hurricane relief by buying real items from trusted local suppliers—or via Amazon as fallback.

#### Platform Goals

* Route >70% of funded goods through Jamaican suppliers, strengthening local recovery ecosystem
* Provide radical transparency: every donation is traceable with proof of fulfillment
* Ship MVP to support active relief operations
* Onboard reliable supplier partners and NGOs for sustainable local commerce integration
* Attach proof of fulfillment to every donation to build donor confidence

#### Key Features

* **Dynamic Relief Items Marketplace**: Filterable catalog of needed goods (water, food, hygiene, hardware) with urgency flags and progress tracking
* **Shop Local Priority**: Direct funding through vetted Jamaican suppliers with in-platform checkout
* **Amazon Fallback**: Alternative fulfillment route when local suppliers can't meet demand
* **Transparency Feed**: Public-facing log of fulfilled items with photos, timestamps, and impact tracking
* **Supplier Directory**: Simple onboarding process for local businesses with admin verification workflow

📖 **Documentation**: See [`product-docs/mana-relief/prd-mana-relief.md`](./product-docs/mana-relief/prd-mana-relief.md) for complete details.

---

## Repository Structure

```
product-docs/
  ├── fieldtrack/
  │   ├── prd-fieldtrack.md
  │   └── technical-one-pager-fieldtrack.md
  ├── mana-relief/
  │   ├── prd-mana-relief.md
  │   └── non-technical-one-pager-mana.md
  └── general-context/
      ├── constraints.md
      ├── hurricane-context.md
      └── ticket-creation.md
```

## Documentation

All product documentation is maintained in Markdown format within the `product-docs/` directory. Each project includes:
- **PRD (Product Requirements Document)**: Complete functional specifications, user stories, and technical considerations
- **One-Pager**: Quick reference documents for technical or non-technical overviews

## Contributing

Documentation and code changes should be committed with clear, descriptive commit messages. For project-specific contributions, reference the relevant PRD for context and requirements.

