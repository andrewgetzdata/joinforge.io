# Edit Event

Help manage events in /src/data/events.json

## Usage
/edit-event [action] [event-title]

## Actions
- add: Add new event
- edit: Modify existing event
- archive: Set is_past to true

## Event Fields
- title: Event title
- type: "Lightning Session", "Workshop", "Ship Session", "Social", "Partner"
- description: Markdown formatted description
- speaker: Speaker or host name
- date: ISO datetime string (e.g., "2025-12-05T17:00:00.000Z")
- duration_in_minutes: Duration number
- location: Location string or "Virtual"
- meeting_url: URL for virtual events
- image_url: Event banner image URL
- max_attendees: Maximum attendee number (or null)
- tags: Array of topic tags
- is_past: boolean, false for future events

## When editing events:
1. Read current events.json file
2. Make requested changes with validation
3. Ensure proper ISO datetime formatting
4. Set appropriate event type with correct casing
5. Write updated file