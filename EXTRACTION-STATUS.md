# Angle One Capital - Squarespace Extraction Status

## ⚠️ REPOSITORY IS INCOMPLETE

This repository is in progress. The full Squarespace site has NOT been completely extracted yet.

---

## ✅ What's Been Completed

### Core Configuration Files
- ✅ `.gitignore` - Git ignore rules
- - ✅ `README.md` - Project overview
  - - ✅ `site-config.json` - Global styling, colors, typography, spacing
    - - ✅ `components.json` - Reusable UI patterns (buttons, hero sections, etc.)
      - - ✅ `navigation.json` - Site structure and menu hierarchy
       
        - ### Pages Extracted (3 of ~50 pages)
        - - ✅ `pages/main-navigation/home-new-3.json` - Landing page
          - - ✅ `pages/main-navigation/the-problem.json` - Problem statement page
            - - ✅ `pages/main-navigation/our-solutions.json` - Parent page (placeholder only)
             
              - ---

              ## ❌ What's Still Missing

              ### Main Navigation Pages (5 pages missing)
              - ❌ `pages/main-navigation/nexus.json`
              - - ❌ `pages/main-navigation/our-team.json`
                - - ❌ `pages/main-navigation/contact.json`
                 
                  - ### Our Solutions Subpages (4 pages missing)
                  - Need to be created in: `pages/main-navigation/our-solutions/`
                  - - ❌ `who-we-serve.json`
                    - - ❌ `advisory.json`
                      - - ❌ `strategies.json`
                        - - ⚠️ `what-we-do.json` - Partially extracted earlier, needs full content
                         
                          - ### Not Linked Pages (~40 pages missing)
                          - Need to be created in: `pages/not-linked/`
                         
                          - **Draft/Test Pages:**
                          - - Thought Leadership (Copy)
                            - - The Problem (Copy)
                              - - Our Team (Copy)
                                - - New Dropdown (empty container)
                                  - - Our Team FOR FUTURE EDITING
                                    - - Nexus (Copy)
                                      - - Nexus (duplicate)
                                        - - Our Solutions (Copy) (appears twice)
                                          - - Home New 3 (Copy)
                                            - - Home New 3
                                              - - Home New
                                                - - The Sorcerer's Apprentice
                                                  - - Enter Multiflation
                                                    - - The Monkey's Paw
                                                      - - Home (appears multiple times)
                                                        - - Thought Leadership
                                                          - - White Papers
                                                            - - What We Do (Copy)
                                                              - - What We Do
                                                                - - The Problem
                                                                  - - Our Solutions (with subpages: Advisory, Strategies)
                                                                    - - Philosophy
                                                                      - - Strategy
                                                                        - - Home (Original)
                                                                          - - Home (Original) (Copy)
                                                                            - - New Page
                                                                              - - Contact
                                                                                - - Team
                                                                                  - - Plus more...
                                                                                   
                                                                                    - ---

                                                                                    ## 📋 What Needs to Be Done

                                                                                    ### Immediate Action Items:

                                                                                    1. **Extract Main Navigation Pages**
                                                                                    2.    - Visit each page in Squarespace
                                                                                          -    - Scroll through entire page to capture all sections
                                                                                               -    - Document:
                                                                                                    -      - Hero sections with video backgrounds
                                                                                                    -       - Text content (headings, body copy, accent words)
                                                                                                    -        - Layout structure (split layouts, grids, etc.)
                                                                                                    -         - CTA buttons
                                                                                                    -          - Footer text
                                                                                                
                                                                                                    -      2. **Extract Our Solutions Subpages**
                                                                                                    -     - Same process as above for each of the 4 subpages
                                                                                                    -    - Pay special attention to the "What We Do" page which has already been partially extracted
                                                                                                     
                                                                                                         - 3. **Document Not Linked Pages**
                                                                                                           4.    - These are draft/archive pages
                                                                                                                 -    - May contain important content variations
                                                                                                                      -    - Create JSON files for each in `pages/not-linked/` folder
                                                                                                                       
                                                                                                                           - 4. **Create Additional Documentation**
                                                                                                                             5.    - `REBUILD-GUIDE.md` - Detailed instructions for Claude AI
                                                                                                                                   -    - `media/assets-mapping.json` - Complete video/image file references
                                                                                                                                        -    - `pages/templates/` - Reusable page templates
                                                                                                                                         
                                                                                                                                             - ---
                                                                                                                                             
                                                                                                                                             ## 🔍 How to Continue Extraction
                                                                                                                                             
                                                                                                                                             ### For Each Page:
                                                                                                                                             1. Navigate to page in Squarespace admin
                                                                                                                                             2. 2. Scroll through ENTIRE page (all sections, top to bottom)
                                                                                                                                                3. 3. Document these elements:
                                                                                                                                                   4.    - Page title and URL
                                                                                                                                                         -    - All hero sections
                                                                                                                                                              -    - All text content (preserve accent word styling)
                                                                                                                                                                   -    - Background videos/images
                                                                                                                                                                        -    - Layout patterns
                                                                                                                                                                             -    - Buttons and CTAs
                                                                                                                                                                                  -    - Special styling notes
                                                                                                                                                                                   
                                                                                                                                                                                       - ### JSON Format:
                                                                                                                                                                                       - ```json
                                                                                                                                                                                         {
                                                                                                                                                                                           "pageId": "page-name",
                                                                                                                                                                                           "title": "Page Title",
                                                                                                                                                                                           "url": "/page-url",
                                                                                                                                                                                           "published": true/false,
                                                                                                                                                                                           "template": "hero-section" | "split-layout" | etc,
                                                                                                                                                                                           "sections": [
                                                                                                                                                                                             {
                                                                                                                                                                                               "id": "section-1",
                                                                                                                                                                                               "type": "hero-section",
                                                                                                                                                                                               "backgroundVideo": "filename.mp4",
                                                                                                                                                                                               "content": {
                                                                                                                                                                                                 "heading": "Main heading text",
                                                                                                                                                                                                 "accentWords": ["word1", "word2"],
                                                                                                                                                                                                 "bodyText": "Optional body paragraph"
                                                                                                                                                                                               }
                                                                                                                                                                                             }
                                                                                                                                                                                           ]
                                                                                                                                                                                         }
                                                                                                                                                                                         ```
                                                                                                                                                                                         
                                                                                                                                                                                         ---
                                                                                                                                                                                         
                                                                                                                                                                                         ## 📊 Progress Summary
                                                                                                                                                                                         
                                                                                                                                                                                         | Category | Completed | Total | Status |
                                                                                                                                                                                         |----------|-----------|-------|--------|
                                                                                                                                                                                         | Core Config Files | 5 | 5 | ✅ 100% |
                                                                                                                                                                                         | Main Nav Pages | 3 | 8 | ⚠️ 37.5% |
                                                                                                                                                                                         | Our Solutions Subpages | 0 | 4 | ❌ 0% |
                                                                                                                                                                                         | Not Linked Pages | 0 | ~40 | ❌ 0% |
                                                                                                                                                                                         | **OVERALL** | **8** | **~57** | **❌ 14%** |
                                                                                                                                                                                         
                                                                                                                                                                                         ---
                                                                                                                                                                                         
                                                                                                                                                                                         ## 🚀 Next Steps
                                                                                                                                                                                         
                                                                                                                                                                                         1. Continue extracting pages one-by-one from Squarespace
                                                                                                                                                                                         2. Create JSON files for each page
                                                                                                                                                                                         3. 3. Upload to GitHub in proper folder structure
                                                                                                                                                                                         4. Update this STATUS file as pages are completed
                                                                                                                                                                                         5. 5. Once complete, Claude AI can use this repo to rebuild the entire site
                                                                                                                                                                                           
                                                                                                                                                                                            6. ---
                                                                                                                                                                                           
                                                                                                                                                                                            7. ## 📝 Notes
                                                                                                                                                                                           
                                                                                                                                                                                            8. - The landing page appears to be "Home New 3" (marked with home icon in Squarespace)
                                                                                                                                                                                               - - Many pages are duplicates or test versions (indicated by "(Copy)" suffix)
                                                                                                                                                                                                 - - All styling is dark-themed with orange (#FF9D00) and cyan (#00D9FF) accents
                                                                                                                                                                                                 - Video backgrounds are critical to the design aesthetic
                                                                                                                                                                                                 - - Site uses Brandon Grotesque for headings, Nunito for body text
                                                                                                                                                                                                  
                                                                                                                                                                                                   - ---
                                                                                                                                                                                                   
                                                                                                                                                                                                   **Last Updated:** [Current date/time]
                                                                                                                                                                                                   **Status:** 🔴 IN PROGRESS - INCOMPLETE
