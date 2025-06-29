---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: hero
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: Hugo Academic Theme
      image:
        filename: hero-academic.png
      cta:
        label: '**Get Started**'
        url: https://hugoblox.com/templates/
      cta_alt:
        label: Ask a question
        url: https://discord.gg/z8wNYzb
      cta_note:
        label: >-
          <div style="text-shadow: none;"><a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star Hugo Blox Builder</a></div><div style="text-shadow: none;"><a class="github-button" href="https://github.com/HugoBlox/theme-academic-cv" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star the Academic template</a></div>
      text: |-
        **Generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 500,000+ sites.**

        **Easily build anything with blocks - no-code required!**

        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.

        <!--Custom spacing-->
        <div class="mb-3"></div>
        <!--GitHub Button JS-->
        <script async defer src="https://buttons.github.io/buttons.js"></script>
    design:
      background:
        gradient_end: '#dced82'
        gradient_start: '#a7c221'
        text_color_light: true
  
  - block: about.biography
    id: about
    content:
      title: Kia ora!
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      
  - block: collection
    id: publications
    content:
      title: Recent Publications
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation

  - block: experience
    id: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Postdoctoral Fellow
          company: University of Toronto Scarborough
          company_url: 'https://www.utsc.utoronto.ca/labs/microbiomemanipulationlab/'
          company_logo: uoft_shield_crop
          location: Toronto, Canada
          date_start: '2024-11-25'
          date_end: ''
          description: Evaluation and evolution of elite agricultural bioinoculants across production landscapes, as part of the [Genome Canada-funded BENEFIT project](https://www.queensu.ca/microbes-for-agriculture/).
        - title: PhD in Biological Sciences
          company: University of Auckland
          company_url: 'https://www.auckland.ac.nz/en.html'
          company_logo: uoa_logo_shield
          location: Auckland, New Zealand
          date_start: '2021-03-01'
          date_end: '2025-01-01'
          description: |2-
            * Examining effector requirements, redundancies, and repertoire refinement in the emergent kiwifruit pathogen *Pseudomonas syringae* pv. *actinidiae*.
            * Awarded a University of Auckland Doctoral Scholarship.    
        - title: MSc in Biological Sciences
          company: University of Auckland
          company_url: 'https://www.auckland.ac.nz/en.html'
          company_logo: uoa_logo_shield
          location: Auckland, New Zealand
          date_start: '2019-03-01'
          date_end: '2020-05-01'
          description: |2-
            * Identification of candidate *Pseudomonas syringae* pv. *actinidiae* effectors that trigger resistance in *Actinidia arguta*.
            * Awarded a Zespri Innovation Scholarship.
        - title: PGDipSci in Biological Sciences
          company: University of Auckland
          company_url: 'https://www.auckland.ac.nz/en.html'
          company_logo: uoa_logo_shield
          location: Auckland, New Zealand
          date_start: '2018-03-01'
          date_end: '2018-12-01'  
          description: |2-
            * Awarded the Senior Frances Briggs Memorial Prize in Plant Sciences.
            * Awarded the Janet Bain Mackay Memorial Prize.
        - title: BSc in Biological Sciences
          company: University of Auckland
          company_url: 'https://www.auckland.ac.nz/en.html'
          company_logo: uoa_logo_shield
          location: Auckland, New Zealand
          date_start: '2015-03-01'
          date_end: '2017-12-01' 
          description: |2-
            * First in Course for BIOSCI 321 - Plant Pathology.
            * Tuākana Certificate of Merit for excellent scholastic achievement in STATS 201.
    design:
      columns: '2'


  - block: accomplishments
    id: teaching
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Teaching'
      subtitle:
      # Date format: https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: 
          date_end: '2023-11-15'
          date_start: '2021-07-01'
          description: 'Graduate Teaching Assistant responsible for delivering online and in-person labs.'
          icon: uoa_logo_shield
          organization: University of Auckland
          organization_url: 
          title: 'BIOSCI 220: Quantitative Biology'
          url: ''
        - certificate_url: 
          date_end: '2023-07-01'
          date_start: '2023-01-25'
          description: 'Graduate Teaching Assistant responsible for lab design, delivery and marking.'
          icon: uoa_logo_shield
          organization: University of Auckland
          organization_url: 
          title: 'BIOSCI 324: Plant Pathology & Symbiosis'
          url: ''
    design:
      columns: '2'

  - block: portfolio
    id: projects
    content:
      title: Posters
      filters:
        folders:
          - project
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: compact
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  
  - block: markdown
    id: gallery
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="flickr" >}}
    design:
      columns: '1'
---