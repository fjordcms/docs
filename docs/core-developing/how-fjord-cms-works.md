# How FjordCMS works

FjordCMS as complex modular web-system is made up of several parts (hierarchy below):
- Core system (default functionality, basement)
  - Global SEO settings
  - E-Mail management
  - Private in-administration data/record management system
  - Authorization/Authentication using relational role system
  - Version management
  - System permissions
      - Admin panel actions
      - For template settings (only global, template permissions per page are in Templates)
  - History and action log
    - History of changes (in system/in modules/in templates)
    - Access log
- Templates (design of website, UI functionality)
    - Template
      - **Admin view**
        - Template settings
        - Pages and routing mechanism
            - Settings of page variables
        - Module dependencies
        - Custom permission nodes (related to page)
      - **Client view**
        - Rendering of pages
- Modules (backend functionality and data management)
  - Module
    - **Admin view**
      - Menu/pages structuring
      - Forms
      - Individual database
      - Custom permission nodes
    - **Client view**
      - Forms
      - In-module template complexes

