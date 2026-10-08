# Future Work

## Contact Email Setup

- [ ] Finish setting up and activating `coach@annleahy.ca` (John is working on email setup).
- [x] Replace the homepage placeholder with `coach@annleahy.ca` and a working email link, as provided in Ann’s October 8 feedback.
- [ ] Connect the consultation form to the approved email or scheduling service so requests actually reach Ann.
- [ ] Verify mailbox delivery and booking delivery before marking booking requests as received.

## Google Calendar Integration

### Overview
The booking form currently displays a confirmation message but does not create actual calendar events. A future enhancement should integrate with Google Calendar to:

1. **Automatically create calendar events** when a user submits the booking form
2. **Check availability** in real-time to show only open time slots
3. **Send calendar invitations** to both Ann and the client
4. **Handle time zone differences** appropriately

### Implementation Options

#### Option A: Google Calendar API (Recommended)
- Use Google Calendar API with OAuth 2.0
- Requires backend service (Node.js, Python, etc.)
- Provides full control over event creation and availability checking
- Documentation: https://developers.google.com/calendar/api

#### Option B: Calendly or Cal.com Embed
- Embed a third-party scheduling tool
- Simpler implementation, no backend required
- Less customization but handles all scheduling logic
- Monthly subscription may be required

### Tasks
- [ ] Choose integration approach
- [ ] Set up Google Cloud project (if using API directly)
- [ ] Create backend service for calendar operations
- [ ] Update booking form to call backend API
- [ ] Implement email notifications
- [ ] Test end-to-end booking flow
