# TLDR

Tips for implementing the Airtable Base. The answers are in the video too. You can copy what you see.
    
- Create 3 tables
  - `Composition Prompts` Table
    - Prompt (Long text)
    - Post Type (Single select)
      - Image
      - Video
      - Text
      - Image Carousel
    - Created Date (Date)
    - Note (Short text)
  - `Content` Table
    - ID (Autonumber)
    - Prompt (Long text) [TIP: Make it hidden]
    - Post Type (Single select)
      - Image
      - Video
      - Text
      - Image Carousel
    - Instagram Caption (Long text)
    - LinkedIn Post (Long text)
    - X.com Post (Long text)
    - YouTube Title + Description (Long text)
    - TikTok Post (Long text)
    - Facebook Post (Long text)
    - Creation Date (Date)
    - Distribution Date (Date) [Optional]
    - Media (Attachment)
    - Approved (Checkbox)
  - `Distribution Prompts` Table
    - Prompt (Long text)
    - Post Type (Single select)
        - Image
        - Video
        - Text
        - Image Carousel
    - Created Date (Date)
    - Note (Short text)
