+++
widget = "pages"
headless = true  # This file represents a page section.

active = true  # Activate this widget? true/false
weight = 23  # Order that this section will appear.

title = "Posts"
#subtitle = "Lab News"

[content]
  # Page type to display. E.g. post, talk, or publication.
  page_type = "post"
  # Choose how much pages you would like to display (0 = all pages)
  count = 5
  # Choose how many pages you would like to offset by
  offset = 0
  # Page order. Descending (desc) or ascending (asc) date.
  order = "desc"
  # Optionally filter posts by a taxonomy term.
  
 [content.filters]
   tag = ''
   category = ''
   publication_type = ''
   exclude_featured = false
   exclude_past = false
   exclude_future = false
    
[design]
  # Toggle between the various page layout types.
  #   1 = List
  #   2 = Compact
  #   3 = Card
  #   4 = Citation (publication only)  
  view = 3
  
  [advanced]
 # Custom CSS.
 css_style = ""

 # CSS class.
 css_class = ""
+++
