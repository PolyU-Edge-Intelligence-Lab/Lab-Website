---
# An instance of the Portfolio widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: portfolio

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 10

#title: Projects
#subtitle: ''



content:
  # Page type to display. E.g. project.
  page_type: project

  # Filter toolbar (optional).
  # Add or remove as many filters (`filter_button` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove the toolbar, delete the entire `filter_button` block.
    # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
  filter_default: 0
  filter_button:

  - name: AI Computing Cyberinfrastructure
    tag: AI Computing Cyberinfrastructure
  # - name: TinyML
  #  tag: TinyML
  #- name: Federated Learning
  #  tag: Federated Learning
  #- name: Blockchain
  #  tag: Blockchain
  #- name: Smart City
  #  tag: Smart City
  #- name: Smart Healthcare
  #  tag: Smart Healthcare
  - name: Cloud-Edge Collaborative Large Models
    tag: Foundation Model
  - name: Trustworthy AI Governance & AIGC
    tag: Trustworthy AI
  - name: AI4Science
    tag: AI for Science
  # - name: Edge AI Application
  #   tag: Edge AI Application
  # - name: Federated Learning
  #   tag: FL
  - name: Others (FL, Tiny ML, Blockchain etc.)
    tag: Others

design:
  # Choose how many columns the section has. Valid values: '1' or '2'.
  columns: '1'

  # Toggle between the various page layout types.
  #   1 = List
  #   2 = Compact
  #   3 = Card
  #   5 = Showcase
  view: 5

  # For Showcase view, flip alternate rows?
  flip_alt_rows: true
---