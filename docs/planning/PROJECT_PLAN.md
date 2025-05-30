# Land Steward Farming Best Practices Site - Project Plan

## Project Overview

**Goal**: Create an informational WordPress website focused on land steward farming best practices, with future WooCommerce integration planned.

**Technical Approach**: Custom theme development using Advanced Custom Fields (ACF) for content management, avoiding page builder plugins.

**Team**: Front-end developer with strong CSS/HTML skills, seeking technical leadership for initial setup and architecture.

## Initial Requirements Gathering

### Content Strategy (To Be Determined)
- [ ] **Content Types**: Define primary content categories (articles, guides, case studies, resources, etc.)
- [ ] **Target Audience**: Specify primary users (farmers, land managers, students, researchers)
- [ ] **Content Organization**: Determine taxonomy structure (by crop, region, practice type, difficulty)
- [ ] **User Interaction**: Define if accounts/login needed initially
- [ ] **Search/Filtering**: Identify content discovery needs

### Future WooCommerce Scope (To Be Planned)
- [ ] **Product Types**: Determine what will be sold (courses, tools, consulting, physical products)
- [ ] **Timeline**: Establish when e-commerce features will be needed
- [ ] **Integration Points**: Plan how informational content connects to future products

### Technical Considerations
- [ ] **Hosting Requirements**: Determine hosting needs and budget
- [ ] **Performance Goals**: Define expected traffic and performance targets
- [ ] **Content Management**: Establish who will manage content and their technical level
- [ ] **Budget Constraints**: Identify limitations on premium plugins/themes/hosting

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
1. **Custom Post Types** (Examples to refine)
   - Articles/Blog Posts
   - Best Practice Guides
   - Case Studies
   - Resource Libraries
   - Expert Profiles

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