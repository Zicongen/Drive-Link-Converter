# Drive-Link-Converter


## 📅 Create Follow-up Meeting
**Double click** to edit me. [Docs](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.googlecalendar/)
 
Books a **30-minute follow-up call** in Google Calendar for the next day at 10:00 AM.
 
**Setup:**
1. Connect your account → **Credentials → Google Calendar OAuth2**
2. Calendar is set to `primary` — change if you use a dedicated sales calendar
3. To change the meeting time, update:
```
Start: $now.plus(1,'day').set({ hour: 10, minute: 0 })
End:   $now.plus(1,'day').set({ hour: 10, minute: 30 })
```
4. `Send Updates` is set to `all` — the lead **receives a calendar invite automatically**
 
> ⚠ Set `Send Updates` to `none` if you are not ready to contact the lead yet.
 
