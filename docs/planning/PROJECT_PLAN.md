# Land Steward Farming Best Practices Site - Project Plan

## Project Overview

**Goal**: Create a WordPress website focused on marketing livestock breeding practices and later crops, with future WooCommerce integration planned.

**Relationship to Main Land Stewards Site**: This site will be more marketing-focused for livestock breeding practices and crops, different from the main Land Stewards site. **Design should complement the main LS website using same styling but won't go into as much detail.**

**Technical Approach**: Custom theme development using Advanced Custom Fields (ACF) for content management, avoiding page builder plugins.

**MAJOR ARCHITECTURE CONSIDERATION**: Recently completed NextJS front-end only website may be included in this build. WordPress Multisite architecture should be evaluated for managing multiple sites under one installation.

**Team**: Front-end developer with strong CSS/HTML skills, seeking technical leadership for initial setup and architecture.

## Initial Requirements Gathering

### Target Audience & Goals
**Primary Audiences:**

1. **Other Breeders/Stewards**
   - Goal: Share genetics information, parasite resistance data, genome information
   - Goal: Promote best practices
   - Goal: Sell breeding stock (relationship building, offline sales)

2. **Large Landowners/Land Managers**
   - Goal: Lease goats for invasive species management
   - Goal: Lease sheep for alternative mowing solutions (solar farms, etc.)
   - Goal: Education on land management through livestock

3. **Pet Owners**
   - Goal: Goat inquiries (not direct sales, inquiry-based only)

### Content Strategy & Functional Requirements

**Primary Content Areas Identified**:
- **Green Program** - Sustainable practices and environmental initiatives
- **Livestock** - Sheep and goats breeding, genetics, parasite resistance
- **Grazing Practices** - Land management through livestock
- **Breeding** - Genetics information, genome data, breeding stock
- **Education** - Resources for land managers on invasive species control and alternative mowing
- **Produce** - Future expansion to crop/produce content
- **Regional Focus** - Showcase Northeast region expertise (limited competition in area)

**Required Functionality**:
- **CMS** - Content management system for regular updates
- **Submission Forms** - Various request forms for different inquiries and services
- **Inquiry System** - For pet goat inquiries (not direct sales)

**E-commerce Planning**:
- [ ] **Sector Development**: Build comprehensive list of possible e-commerce sectors
- [ ] **Integration Planning**: Connect content areas to future sales channels

**Content Organization**:
- [ ] **Taxonomy Structure**: By animal type, practice type, region, difficulty
- [ ] **User Interaction**: Define accounts/login needs for different user types
- [ ] **Search/Filtering**: Advanced filtering by genetics, region, practice type

### Future E-commerce & CRM Integration
**E-commerce Timeline**: Not initially needed, but will be added eventually

**CRM Integration Planning**:
- **Primary Options**: Salesforce vs. Raisers Edge (most likely Salesforce)
- **Goal**: Consolidate multiple databases/spreadsheets under one roof
- Website architecture must accommodate future CRM connectivity
- Consider API integration points for lead capture and customer data sync
- Future e-commerce must integrate with chosen CRM system

**Integration Considerations**:
- [ ] **Lead Capture**: Design forms and contact points for CRM integration
- [ ] **Customer Data Flow**: Plan how website interactions feed into CRM
- [ ] **Product Integration**: Plan how informational content connects to future e-commerce
- [ ] **Timeline**: Establish when e-commerce features will be needed

### Technical Considerations
- [ ] **Hosting Requirements**: Determine hosting needs and budget
- [ ] **Performance Goals**: Define expected traffic and performance targets
- [ ] **Content Management**: Establish who will manage content and their technical level
- [ ] **Budget Constraints**: Identify limitations on premium plugins/themes/hosting

### Architecture Decision: NextJS Integration & Multisite Evaluation
**Critical Decision Required**: Evaluate integration of existing NextJS front-end website

**Options to Consider**:
1. **WordPress Multisite Network**
   - Manage multiple sites under one WordPress installation
   - Shared user base, plugins, and themes across sites
   - Centralized administration and updates
   - Potential for shared CRM integration across sites

2. **Headless WordPress + NextJS**
   - Use WordPress as content management backend
   - NextJS site consumes WordPress data via REST API/GraphQL
   - Maintain existing NextJS frontend architecture
   - More complex but potentially better performance

3. **Separate WordPress Installation**
   - Keep sites completely independent
   - Simpler initial setup but harder to maintain consistency
   - Duplicate efforts for CRM integration and user management

**Evaluation Criteria**:
- [ ] **Content Management**: How will content be managed across sites?
- [ ] **User Experience**: Do sites need shared user accounts/login?
- [ ] **CRM Integration**: Single CRM integration vs. multiple integrations
- [ ] **Maintenance**: Administrative overhead and update complexity
- [ ] **Performance**: Speed and scaling considerations
- [ ] **Development Resources**: Team capacity for different approaches

## Recommended Technical Stack

### Core WordPress Setup
- **WordPress**: Latest version with regular updates
- **Theme Strategy**: Custom child theme approach for maximum flexibility
- **Content Management**: Advanced Custom Fields Pro for custom post types and field groups
- **Development Environment**: Local development with staging/production workflow

### Suggested Parent Theme Options
1. **Twenty Twenty-Four (Block Theme)** - Modern, lightweight, future-proof
2. **GeneratePress** - Performance-focused, highly customizable, developer-friendly
3. **Astra** - Fast, flexible, good WooCommerce compatibility
4. **Custom Starter Theme** - Built from scratch using modern WordPress standards

### Essential Plugins (Recommended)
- **Advanced Custom Fields Pro** - Custom fields and post types
- **Custom Post Type UI** - Additional CPT management (if needed beyond ACF)
- **RankMath SEO** - Search engine optimization

## Development Approach

### Phase 1: Foundation Setup
1. **Environment Setup**
   - Create Pantheon sandbox site with default WordPress install
   - Use Lando to pull codebase and database locally for development
   - Standard Pantheon Dev/Test/Live workflow

2. **Theme Architecture**
   - Parent theme selection and evaluation
   - Child theme creation
   - Basic theme structure setup
   - CSS/SCSS architecture planning

3. **Content Structure Planning**
   - Custom post type identification
   - Field group design
   - Taxonomy structure
   - Template hierarchy planning

### Phase 2: Content Types & Fields
1. **Custom Post Types** (Based on content areas identified)
   - **Livestock Profiles** - Sheep and goat breeding information, genetics data
   - **Green Program** - Sustainable practices and environmental initiatives  
   - **Grazing Practices** - Land management techniques and case studies
   - **Educational Resources** - Guides for land managers on invasive species/mowing alternatives
   - **Regional Showcases** - Northeast region expertise and success stories
   - **Breeding Stock** - Available animals with genetics/parasite resistance data
   - **Service Inquiries** - Pet goat requests and land management consultations

2. **Custom Fields & Taxonomies**
   - Field groups for each post type
   - Category/tag taxonomies
   - Custom taxonomies (regions, crops, practices, difficulty levels)

3. **Template Development**
   - Archive templates
   - Single post templates
   - Search and filtering functionality
   - Responsive design implementation

### Phase 3: Advanced Features
1. **User Experience**
   - Advanced search/filtering
   - Content recommendations
   - User accounts (if needed)
   - Newsletter integration

2. **Performance & SEO**
   - Image optimization
   - Cloudflare CDN and performance optimization
   - Schema markup
   - Performance monitoring

### Phase 4: WooCommerce Preparation
1. **Architecture Review**
   - Ensure theme WooCommerce compatibility
   - Plan product integration with content
   - Design checkout/account flows

2. **Content Integration**
   - Connect informational content to products
   - Cross-selling strategies
   - Member/customer content areas

## Next Steps

### Immediate Actions Needed
1. **Requirements Gathering Session**
   - Define content types and structure
   - Identify target audience specifics
   - Establish timeline and budget parameters

2. **Technical Decisions**
   - Select parent theme approach
   - Choose hosting solution
   - Set up development environment

3. **Content Planning**
   - Create content inventory
   - Design field group structures
   - Plan template layouts

### Design Inspiration & Style Preferences

**Reference Websites Analyzed:**

1. **Blackberry Farm Shop** (blackberryfarmshop.com/farmstead/)
   - Elegant, rustic aesthetic reflecting agricultural heritage
   - Muted, natural color palette (beiges, grays)
   - High-quality product photography
   - Sophisticated typography mixing serif and sans-serif
   - Clean grid-based layout with intuitive navigation
   - Storytelling through product descriptions emphasizing farm origins

2. **Hudson Valley Foie Gras** (hudsonvalleyfoiegras.com/collections/duck)
   - Clean, minimalist e-commerce layout
   - Forest green and neutral color palette suggesting premium quality
   - Product-focused design with consistent image sizing
   - Descriptive content emphasizing artisanal quality
   - Mobile-friendly, responsive design

3. **Esri StoryMaps** (Environmental/Conservation Sites)
   - Interactive storytelling through visual narratives
   - Educational content delivery with engaging user experience
   - Clean, minimal design focusing on content
   - Visual storytelling to make complex information accessible

**Design Direction Insights:**
- Preference for clean, sophisticated agricultural aesthetics
- Natural color palettes that reflect farming/environmental themes
- High-quality photography and visual storytelling
- Premium positioning while maintaining authenticity
- Interactive, educational content delivery
- Mobile-responsive, user-friendly layouts

### Questions for Next Discussion
1. What specific farming practices/topics will be covered?
2. What's the rough timeline for launch and WooCommerce addition?
3. Do you have preferred hosting providers or budget constraints?
4. Will there be multiple content contributors?
5. Any existing branding/design requirements?

## Success Metrics
- [ ] Fast, responsive site performance
- [ ] Easy content management for non-technical users
- [ ] Scalable architecture for future WooCommerce integration
- [ ] SEO-optimized content structure
- [ ] Mobile-first responsive design

---

**Next Meeting**: Review requirements and begin technical setup phase.

**Project Status**: Planning Phase - Requirements Gathering