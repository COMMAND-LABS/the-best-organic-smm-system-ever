# TASK

Generate copy for a multi-day marketing campaign to post once per day to LinkedIn & Instagram. You should generate about 8 to 9 days of posts in total. The last day of posting should be June 24th,  2025 (aka 30 days out from the event on July 24th, 2025).

Store the posts into Airtable.

## LINK TO EVENT PROMO IMAGE

{
  "url": "<PUBLIC_LINK_TO_YOUR_VIDEO_HERE>",
  "filename": "<FILENAME_HERE>"
}

## ABOUT THE IMAGE

Describe the image details that are important for the social media content here

## GENERAL REQUIREMENTS

- Make the output natural and impossible to detect as being A.I. generated
- Use spacing and new lines to make the marketing copy easy to read
- Use minimal emojis
- Do NOT bold any text when generating the copy for LinkedIn
- Avoid em-dashes
- Make the posts short and succinct
- CTA
- Date format is MM/DD/YYYY

## SCHEMA FOR LINK TO MEDIA

{
  "type": "array",
  "items": {
    "type": "object",
    "properties": {
      "url": {
        "type": "string"
      },
      "filename": {
        "type": "string"
      }
    }
  }
}

## TODAY'S DATE

MM/DD/YYYY

## SEO KEYWORDS

ai, course, masterclass, miami, south, florida, learn, network