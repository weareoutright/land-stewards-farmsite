# Land Steward Farming Site - Project Plan

## Project Overview

**Goal**: Create a WordPress website focused on marketing livestock breeding practices with future expansion to crop content and e-commerce capabilities.

**Relationship to Main Land Stewards Site**: This will be a separate marketing-focused site for livestock breeding and land management services. Design should complement the main LS website using similar styling but with less detail and complexity.

**Technical Approach**: Custom WordPress theme development using Advanced Custom Fields (ACF) for content management, avoiding page builder plugins.

## Target Audiences & User Goals

1. **Other Breeders/Stewards**
   - Share genetics information, parasite resistance data, genome information
   - Promote best practices in livestock breeding
   - Facilitate breeding stock sales (relationship building, offline transactions)

2. **Large Landowners/Land Managers**
   - Lease goats for invasive species management
   - Lease sheep for alternative mowing solutions (solar farms, large properties)
   - Access education on land management through livestock

3. **Pet Owners**
   - Submit inquiries for goat purchases (inquiry-only, not direct sales)

## Content Strategy

### Primary Content Areas
- **Green Program** - Sustainable practices and environmental initiatives
- **Livestock Management** - Sheep and goats breeding, genetics, parasite resistance
- **Grazing Practices** - Land management techniques and case studies
- **Breeding Information** - Genetics data, genome information, breeding stock profiles
- **Educational Resources** - Guides for land managers on invasive species control and alternative mowing
- **Regional Showcase** - Northeast region expertise and success stories (competitive advantage)
- **Future Expansion** - Crop/produce content planned for later phases

### Required Functionality
- **Content Management System** - Easy updates for non-technical users
- **Submission Forms** - Various request forms for different inquiries and services
- **Inquiry System** - Pet goat purchase inquiries and land management consultations
- **Search & Filtering** - Advanced filtering by genetics, region, practice type, animal type

### Content Organization
- **Custom Post Types**: Livestock Profiles, Green Program Posts, Grazing Case Studies, Educational Resources, Regional Showcases, Breeding Stock Listings, Service Inquiries
- **Taxonomies**: Animal type, practice type, region, difficulty level, genetics data
- **Custom Fields**: Breeding information, genetics data, parasite resistance metrics, contact forms

## Future Integration Planning

### E-commerce Development (Phase 2+)
**Timeline**: Not needed for initial launch, planned for future implementation

**Planned Features**:
- Online breeding stock catalog
- Service booking system
- Educational content sales
- Regional networking capabilities

**Sector Development**: Comprehensive list of e-commerce sectors to be developed based on initial site performance and user feedback

### CRM Integration (Phase 2+)
**Decision Required**: Salesforce vs. Raisers Edge (Salesforce likely choice)

**Goal**: Consolidate multiple databases/spreadsheets under unified CRM system

**Integration Requirements**:
- Lead capture from all website forms
- Automated data flow from website interactions to CRM
- Customer data synchronization
- Future e-commerce integration with CRM system

## Architecture Decision Framework

### CRITICAL DECISION: NextJS Integration Strategy

**Context**: Recently completed NextJS front-end website exists. This new site serves different audiences with different goals - NOT an enhancement to existing NextJS site.

### Option 1: Separate WordPress Installation (RECOMMENDED)
**Development Time**: 125-175 hours
**Approach**: Completely independent WordPress site

**Pros**:
- Fastest development timeline
- Full access to WordPress/WooCommerce/Salesforce plugin ecosystem
- Independent scaling and customization
- No dependency on existing NextJS site
- Easier implementation of forms and CRM integrations
- Lower risk, proven approach

**Cons**:
- Potential duplicate efforts for shared functionality
- Separate maintenance overhead

### Option 2: Traditional WordPress CMS (with Integration Planning)
**Development Time**: 150-200 hours
**Approach**: WordPress site with architecture planning for eventual NextJS coordination

**Pros**:
- Keeps door open for future integration
- Native WooCommerce integration
- Proven ecosystem for complex integrations
- Planning for coordinated design systems

**Cons**:
- Additional 25-50 hours for integration planning
- More complex decision-making process
- Dependencies on existing NextJS architecture

### Option 3: WordPress Multisite Network
**Development Time**: 225-300 hours
**Not Recommended Due To**:
- WooCommerce multisite complexity
- Increased e-commerce integration challenges
- Higher maintenance overhead
- Medium-high risk level

### Option 4: Headless WordPress + NextJS
**Development Time**: 250-350 hours
**Not Recommended Due To**:
- Custom e-commerce integration required
- Complex Salesforce connectivity
- Higher development overhead
- High risk with less experienced developer resources

### **RECOMMENDATION: Option 1 - Separate WordPress Installation**

**Rationale**:
- Fastest time to market (125-175 hours)
- Lowest risk approach
- Full ecosystem access for CRM/e-commerce
- Independence allows for rapid iteration
- Future integration can be evaluated after both sites are established

## Technical Stack

### Core WordPress Setup
- **WordPress**: Latest version with regular updates
- **Hosting**: Pantheon with Dev/Test/Live workflow
- **Development Environment**: Lando for local development
- **Content Management**: Advanced Custom Fields Pro for custom post types and field groups
- **SEO**: RankMath SEO optimization
- **Performance**: Cloudflare CDN integration

### Theme Strategy
**Options**:

**GeneratePress + Custom Child Theme**
- Performance-focused and highly customizable
- Excellent WooCommerce compatibility for future e-commerce
- Developer-friendly with strong community support
- Proven track record for custom implementations

**Custom Theme Development**
- Complete design control and unique branding
- Optimized specifically for project requirements
- No third-party dependencies or licensing
- Full ownership of codebase

### Form & CRM Integration
- **Forms**: Gravity Forms Pro (excellent Salesforce integration)
- **CRM Integration**: Gravity Forms Salesforce Add-on or dedicated Salesforce plugin
- **Lead Management**: Automated data flow to chosen CRM system

## Development Phases

### Phase 1: Foundation (4-6 weeks)
1. **Environment Setup**
   - Pantheon site creation and Lando local setup
   - GeneratePress child theme implementation
   - Basic site architecture and navigation

2. **Content Structure**
   - ACF field groups for all content types
   - Custom post type creation
   - Taxonomy structure implementation

3. **Core Functionality**
   - Basic submission forms
   - Content templates for all post types

### Phase 2: Content & Design (3-4 weeks)
1. **Design Implementation**
   - Visual design aligned with main LS site
   - Responsive design across all devices
   - Agricultural aesthetic with natural color palette

2. **Advanced Features**
   - Search and filtering functionality
   - Content recommendations
   - Performance optimization

### Phase 3: Integration & Testing (2-3 weeks)
1. **CRM Integration**
   - Salesforce connection setup
   - Form automation testing
   - Data flow verification

2. **Launch Preparation**
   - Performance testing
   - SEO optimization
   - Content migration and testing

### Phase 4: Future Enhancement Planning
1. **E-commerce Preparation**
   - WooCommerce architecture planning
   - Product integration strategy
   - Payment system evaluation

2. **Performance Monitoring**
   - Analytics implementation
   - User behavior tracking
   - Conversion optimization

## Design Direction

### Reference Aesthetics
**Target Style**: Clean, sophisticated agricultural aesthetic
- **[Blackberry Farm Shop](https://shop.blackberryfarm.com)**: Elegant rustic design, muted natural colors, high-quality photography
- **[Hudson Valley Foie Gras](https://www.hudsonvalleyfoiegras.com)**: Minimalist e-commerce layout, premium positioning
- **[Esri StoryMaps](https://storymaps.arcgis.com)**: Interactive educational content delivery

### Design Principles
- Natural color palettes reflecting farming/environmental themes
- High-quality photography and visual storytelling
- Premium positioning while maintaining authenticity
- Mobile-responsive, user-friendly layouts
- Interactive educational content delivery

## Immediate Action Items

### 1. FINALIZE ARCHITECTURE DECISION
**Owner**: Technical Lead
**Timeline**: This week
- [ ] Confirm Separate WordPress Installation approach
- [ ] Document decision rationale
- [ ] Plan development environment setup

### 2. CRM INTEGRATION PLANNING
**Owner**: Business Lead + Technical Lead
**Timeline**: Next week
- [ ] Finalize Salesforce vs. Raisers Edge decision
- [ ] Define lead capture requirements
- [ ] Map data flow from website to CRM

### 3. DEVELOPMENT SETUP
**Owner**: Technical Lead
**Timeline**: Week 2
- [ ] Set up Pantheon hosting environment
- [ ] Configure Lando local development
- [ ] Install and configure GeneratePress + child theme

### 4. CONTENT STRUCTURE FINALIZATION
**Owner**: Content Lead + Technical Lead
**Timeline**: Week 2-3
- [ ] Finalize ACF field groups for livestock data
- [ ] Complete taxonomy structure for animal types, regions, practices
- [ ] Create content templates and style guide

## Success Metrics

- **Performance**: Fast, responsive site (< 3 second load times)
- **Usability**: Easy content management for non-technical users
- **Scalability**: Architecture supports future WooCommerce integration
- **SEO**: Optimized content structure for search visibility
- **Mobile**: Mobile-first responsive design
- **Integration**: Seamless CRM data flow and lead capture

## Project Timeline

**Total Estimated Development**: 125-175 hours (3-4 months part-time)

**Phase 1 Completion**: 6-8 weeks
**Beta Launch**: 10-12 weeks
**Full Launch**: 12-16 weeks

---

**Next Meeting**: Architecture decision confirmation and development kickoff planning

**Project Status**: Planning Complete - Ready for Development Phase