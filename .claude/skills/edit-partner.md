# Edit Partner

Help manage partner data in /src/data/partners.json

## Usage
/edit-partner [action] [partner-name]

## Actions
- add: Add new partner
- edit: Modify existing partner
- archive: Set is_archived to true
- reorder: Change display_order

## Partner Fields
- name: Partner company name
- logo_url: URL to partner logo image
- website_url: Partner website (optional)
- display_order: Numeric order for display (0, 1, 2, etc.)
- logo_height: "small", "medium", or "large"
- is_archived: boolean, false to display

## When editing partners:
1. Read current partners.json file
2. Make requested changes with proper validation
3. Ensure display_order is unique
4. Write updated file
5. Suggest running npm run build to test

## Example Partner Structure:
```json
{
  "name": "TechCorp",
  "logo_url": "https://example.com/logo.png",
  "website_url": "https://techcorp.com",
  "display_order": 3,
  "logo_height": "large",
  "is_archived": false
}
```