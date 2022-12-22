### <h2>Introduction</h2>
Event can have one of the following status:

1. Pending
2. Approved
3. Rejected
4. Archived

### <h2>Event Lifecycle</h2>
<br>
    <figure markdown>
        ![Image title](/assets/event_management/event_lifecycle.png){ width="200" }
        <figcaption>Event Lifecycle chart</figcaption>
    </figure>

### States

#### <h2>Pending</h2>
When a user reports an event it is available to view on the <a href="https://ageoplatform.eu"> Web Platform </a> in <i>Pending</i> state by default.

You can refer to <a href="http://127.0.0.1:8000/reporting/report_event/">Report an event</a> section for details about reporting an event.

???+ Note
    Events in <i>Pending</i> state are not verified by AGEO

For Example:

We report a Rockfall event
    <figure markdown>
        ![Image title](/assets/event_management/submit_link.png){ width="200" }
        <figcaption>Reporting an event</figcaption>
    </figure>
<br>
    <figure markdown>
        ![Image title](/assets/event_management/web_view.png){ width="800" }
        <figcaption>Event View on web platform</figcaption>
    </figure>

#### <h2>Rejected</h2>
An <strong>Admin</strong> or a <strong>Manager</strong> can choose to reject an event.

Rejected events are still viewable on the map and table view for anonymous users.
???+ Tip
    <i>Rejected</i> events can be archived to remove it from user view

???+ Note
    <i>Rejected</i> events can be verified again

Example: 
Manager rejecting a Rockfall event
    <figure markdown>
        ![Image title](/assets/event_management/reject_event.png){ width="800" }
        <figcaption>Event View on web platform</figcaption>
    </figure>
A reject event will be represented a red "Rejected" badge
    <figure markdown>
        ![Image title](/assets/event_management/event_rejected.png){ width="800" }
        <figcaption>Event View on web platform</figcaption>
    </figure>

#### <h2>Accepted</h2>
An <strong>Admin</strong> or a <strong>Manager</strong> can choose to approve an event.

???+ Note
    <i>Approved</i> events can be rejected later

Example:
We will approve an Earthquake event
    <figure markdown>
        ![Image title](/assets/event_management/approve_event.png){ width="800" }
        <figcaption>Event View on web platform</figcaption>
    </figure>

#### <h2>Archived</h2>
An <strong>Admin</strong> or a <strong>Manager</strong> can choose to archive an event. This feature can be used soft delete events from user view.

Archived events will not be viewable to anyone except Admin and Managers.
???+ Note
    <i>Archived</i> events can be unarchived later and will appear in <i>Approved</i> State.

