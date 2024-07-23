---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: About me
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: people
    id: groups
    content:
      title: Meet the Team
      # Choose which groups/teams of users to display.
      #   Edit `user_groups` in each user's profile to add them to one or more of these groups.
      user_groups:
        - Phd Students
        - Researchers
        - Grad Students
        - Administration
        - Postdocs
      sort_by: Params.last_name
      sort_ascending: true
    design:
      # Show user's social networking links? (true/false)
      show_social: false
      # Show user's interests? (true/false)
      show_interests: false
      # Show user's role?
      show_role: true
      # Show user's organizations/affiliations?
      show_organizations: true

  - block: people
    id: alumni
    content:
      title: Former members (and where to find them)
      # Choose which groups/teams of users to display.
      #   Edit `user_groups` in each user's profile to add them to one or more of these groups.
      user_groups:
        - Alumni
      sort_by: Params.last_name
      sort_ascending: true
    design:
      # Show user's social networking links? (true/false)
      show_social: true
      # Show user's interests? (true/false)
      show_interests: false
      # Show user's role?
      show_role: true
      # Show user's organizations/affiliations?
      show_organizations: true

  - block: collection
    id: classes
    content:
      title: Recent classes
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
      view: showcase
      columns: '2'


  - block: collection
    id: books
    content:
      title: Books and reviews
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - books
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
      columns: '5'

  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'

  - block: slider
    id: projects
    content:
      slides:
        - title: 👋 Welcome to the group
          content: Take a look at what we're working on...
          align: center
          background:
            image:
              # Specify an image from `assets/media/`
              # or delete the image section to remove it
              filename: photo.jpeg
              filters:
                brightness: 0.7
            position: right
            color: '#666'
        - title: Learning Neural Nets (with Neural Nets)
          content: 'Invited talk in the Physics for Neural Network Conference in Princeton, April 2023'
          align: left
          background:
            image:
              # Specify an image from `assets/media/`
              # or delete the image section to remove it
              filename: Princeton.jpeg
              filters:
                brightness: 0.7
            position: center
            color: '#555'
          link:
            icon: graduation-cap
            icon_pack: fas
            text: See the talk
            url: https://www.kaltura.com/index.php/extwidget/preview/partner_id/1449362/uiconf_id/25928631/embed/dynamic?flashvars[playlistAPI.kpl0Id]=1_jg3ev20y
        - title: How do two-layer neural networks learn complex functions from data over time? 
          content: 'Invited talk at Mathematics of Modern Machine Learning in Neurips 2023'
          align: left
          background:
            image:
              # Specify an image from `assets/media/`
              # or delete the image section to remove it
              filename: neurips_no.jpeg
              filters:
                brightness: 0.7
            position: center
            color: '#555'
          link:   
            icon: graduation-cap
            icon_pack: fas
            text: See the talk
            url: https://neurips.cc/virtual/2023/workshop/66507#collapse83688
        - title: Are Gaussian Data All You Need?
          content: 'Invited talk in the GRAMSIA conference in Harvard, May 2023'
          align: left
          background:
            image:
              # Specify an image from `assets/media/`
              # or delete the image section to remove it
              filename: harvard.jpg
              filters:   
                brightness: 0.7
            position: center
            color: '#555'
          link:
            icon: graduation-cap
            icon_pack: fas
            text: See the talk
            url: https://www.youtube.com/watch?v=SevHEAo2MHg&ab_channel=HarvardCMSA
        - title: Comment fonctionne l'inteligence artificielle ?
          content: 'Conference grand public de vulgarisation a
          Cargese, Juillet 2024'
          align: left
          background:
            image:
              # Specify an image from `assets/media/`
              # or delete the image section to remove it
              filename: Cargese.jpg
              filters:
                brightness: 0.7
            position: center
            color: '#555'
          link:
            icon: graduation-cap
            icon_pack: fas
            text: Voir la conference
            url: https://www.youtube.com/watch?v=zBdHMIjrDEc&ab_channel=IESCARGESE
        - title: Statistical Physics and Learning 
          content: 'Invited talk in the Turing Institute in London, 2019'
          align: left
          background:
            image:
              # Specify an image from `assets/media/`
              # or delete the image section to remove it
              filename: alanturing.jpeg
              filters:
                brightness: 0.7
            position: center
            color: '#555'
          link:   
            icon: graduation-cap
            icon_pack: fas
            text: See the talk
            url: https://www.youtube.com/watch?v=k65KqtJsEVU&ab_channel=TheAlanTuringInstitute
        - title: Youtube Channel
          content: 'Videos of talks from Prof. Krzakala'
          align: right
          background:
            image:
              # Specify an image from `assets/media/`
              # or delete the image section to remove it
              filename: photo_talk_youtube.jpeg
              filters:
                brightness: 0.5
            position: center
            color: '#333'
          link:
            icon: graduation-cap
            icon_pack: fas
            text: Youtube Channel
            url: https://www.youtube.com/playlist?list=PLvKBgJ4p0p3yNIJfnNx0BA4EKAHg3eOT-
    design:
      # Slide height is automatic unless you force a specific height (e.g. '400px')
      slide_height: ''
      # Make the slides full screen within the browser window?
      is_fullscreen: true
      # Automatically transition through slides?
      loop: false
      # Duration of transition between slides (in ms)
      interval: 2000

  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
      # Contact (add or remove contact options as necessary)
      email: florent.krzakala@epfl.ch
      phone: +41 21 693 31 87
      address:
        street: EPFL, IdePHICS lab, ELD 239, Station 11
        city: Lausanne
        postcode: 1015
        country: Switzerland
        country_code: CH
      coordinates:
        latitude: '46.51917196603566'
        longitude: '6.564594732428433'
      # Automatically link email and phone or display as text?
      autolink: true

---

---
