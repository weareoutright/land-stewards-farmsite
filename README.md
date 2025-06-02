# Land Steward Farming Best Practices

A WordPress website focused on land steward farming best practices, built for scalability and future WooCommerce integration.

## Project Overview

This site serves as an informational resource for land stewards, farmers, and agricultural professionals seeking evidence-based farming practices. The architecture is designed to support future e-commerce functionality while maintaining optimal performance and user experience.

## Technical Stack

- **WordPress** - Latest version with custom theme development
- **Advanced Custom Fields Pro** - Custom post types and field management
- **Pantheon Hosting** - Dev/Test/Live workflow with Cloudflare CDN
- **Lando** - Local development environment

## Getting Started

### Local Development Setup

1. **Prerequisites**: Install [Lando](https://lando.dev/) for local development
2. **Clone Repository**: `git clone [repository-url]`
3. **Start Environment**: `lando start`
4. **Pull Database**: `lando pull pantheon`

See `/docs/setup/` for detailed environment configuration.

### Development Workflow

- **Dev Environment**: Local development with Lando
- **Test Environment**: Pantheon test site for staging
- **Live Environment**: Production site on Pantheon

## Project Documentation

Comprehensive project documentation is organized in the `/docs/` directory:

- **`/docs/planning/`** - Project planning documents and requirements
  - `PROJECT_PLAN.md` - Complete project roadmap and technical approach
- **`/docs/setup/`** - Environment and technical setup documentation
- **`/docs/development/`** - Development guidelines and specifications
- **`/docs/content/`** - Content strategy and structure documentation

## Architecture

### Theme Strategy
Custom child theme approach using modern WordPress standards for maximum flexibility and future WooCommerce compatibility.

### Content Management
- Custom post types for articles, guides, case studies, and resources
- Advanced Custom Fields for structured content input
- Custom taxonomies for content organization (regions, crops, practices)

### Performance
- Cloudflare CDN integration
- Image optimization
- Pantheon's high-performance hosting stack

## Contributing

This project follows standard WordPress development practices with custom theme development. See `/docs/development/` for coding standards and contribution guidelines.

## License

[License information - to be determined]

## Support

For technical questions or project planning, refer to the documentation in `/docs/planning/PROJECT_PLAN.md`.