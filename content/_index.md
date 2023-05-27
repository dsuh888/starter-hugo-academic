---
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: collection
    id: job-market-paper
    content:
      title: Job Market Paper
      filters:
        folders:
          - working-papers
        tag: job-market
      count: 1
      offset: 0
      order: desc
      item_layout: vertical
      show_abstract: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: working-papers
    content:
      title: Working Papers
      text: >-
        <details>
          <summary>Abstract</summary>
          <p>This is an abstract</p>
        </details>
      filters:
        folders:
          - working-papers
        tag: wp
      count: 5
      offset: 0
      order: desc
    design:
      columns: '2'
      view: citation
  - block: collection
    id: publications
    content:
      title: Publications
      text: ''
      filters:
        folders:
          - publication
        exclude_featured: true
      count: 5
      offset: 0
      order: desc
    design:
      columns: '2'
      view: citation
---
