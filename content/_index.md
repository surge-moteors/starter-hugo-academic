---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    id: home
    content:
      title: AIR-DI
      image:
        filename: hero-robot-head-s.png
        size: s
      text: |-
        **The description of our group.**

        Some introduction content.

        <!--Custom spacing-->
        <div class="mb-3"></div>
        <!--GitHub Button JS-->
        <script async defer src="https://buttons.github.io/buttons.js"></script>
    design:
      background:
        # gradient_end: '#1976d2'
        # gradient_start: '#004ba0'
        gradient_end: '#A9D0F5'
        gradient_start: '#01A9DB'
        gradient_angle: 90
        text_color_light: true
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: true
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  # - block: people
  #   id: people
  #   content:
  #     title: Meet the Team
  #     user_groups:
  #       - Researchers
  #     sort_by: last_name
  #     sort_ascending: true
  #   design:
  #     # Show user's social networking links? (true/false)
  #     show_social: false
  #     # Show user's interests? (true/false)
  #     show_interests: true
  #     # Show user's role?
  #     show_role: true
  #     # Show user's organizations/affiliations?
  #     show_organizations: true
  # - block: tag_cloud
  #   content:
  #     title: Popular Topics
  #   design:
  #     columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      # Contact (add or remove contact options as necessary)
      email: test@example.org
      phone: 888 888 88 88
      address:
        street: 
        city: Beijing
        region: 
        postcode: '100000'
        country: China
        country_code: 
      directions: 
      office_hours:
      contact_links:
        - icon: github
          icon_pack: fab
          name: Find us on GitHub
          link: 'https://github.com/AIR-DI'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      # form:
      #  provider: netlify
      #  formspree:
      #    id:
      #  netlify:
      #    # Enable CAPTCHA challenge to reduce spam?
      #    captcha: false
    design:
      columns: '2'
---
