---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:

  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  
   - block: publications
    id: featured
    content:
      title: Publications
      text: A complete list of my publications can be obtained from my '[Google Scholar](https://scholar.google.com/citations?user=8KIsYXkAAAAJ&hl=en)' profile. Please do not hesistate to contact me for full-text or associated data.
      
  - block: collection
    id: posts
    content:
      title: Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 2
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
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Comments, Criticism or Questions? Please get in touch! 
      # Contact (add or remove contact options as necessary)    
      address:
        street: Mechanical Engineering, Indian Institute of Science
        city: Bangalore
        region: Karnataka
        postcode: '560012'
        country: India
        country_code: IN   
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: 
          link: 'https://twitter.com/strayologist'
          
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
