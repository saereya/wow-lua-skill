# GMTicketInfo

Namespace `C_GMTicketInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/gmticketinfodocumentation.lua` (FileDataID 4637097)

## Events

### GM_PLAYER_INFO

```lua
GM_PLAYER_INFO(name: cstring, info: cstring)
```

`SynchronousEvent`

### ITEM_RESTORATION_BUTTON_STATUS

```lua
ITEM_RESTORATION_BUTTON_STATUS()
```

`SynchronousEvent`

### PETITION_CLOSED

```lua
PETITION_CLOSED()
```

`SynchronousEvent`

### PETITION_SHOW

```lua
PETITION_SHOW()
```

`SynchronousEvent`

### PLAYER_REPORT_SUBMITTED

```lua
PLAYER_REPORT_SUBMITTED(invitedByGUID: WOWGUID)
```

`SynchronousEvent`

### QUICK_TICKET_SYSTEM_STATUS

```lua
QUICK_TICKET_SYSTEM_STATUS()
```

`SynchronousEvent`

### QUICK_TICKET_THROTTLE_CHANGED

```lua
QUICK_TICKET_THROTTLE_CHANGED()
```

`SynchronousEvent`

### UPDATE_WEB_TICKET

```lua
UPDATE_WEB_TICKET(hasTicket: bool, numTickets: number?, ticketStatus: number?, caseIndex: number?, waitTimeMinutes: number?, waitMessage: cstring?, caseTitle: cstring?, caseDescription: cstring?)
```

`SynchronousEvent`
