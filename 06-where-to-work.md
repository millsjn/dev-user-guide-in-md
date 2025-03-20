# 6 Where to Do Your Work
The sensitive data that you have been approved to access will either be stored in the ADRF's structured or unstructured stroage locations (see How to Access Data](05-access-data.md).

## Topics
- [Eligible locations to do your work](#eligible-locations-to-do-your-work)
- [Ineligible locations to do your work](#ineligible-locations-to-do-your-work)
- [Storage Size Restrictions and Best Practices](#storage-size-restrictions-and-best-practices)


## Eligible locations to do your work
You can perform your approved project work in one of the following locations in the ADRF:
- [User Drive](#user-drive)
- [Project Drive](#project-drive)
- [PR schema](#pr-schema)

### User Drive
The U: drive is your user drive; it’s where you will store any files you are working on. Only the user will have access to the U: drive. For example, if user A wants to share information with user B who is on the same project, user A will need to save files to a P: drive folder and not folders in their U: drive since user B will not be able to access user A’s U: drive.

### Project Drive
The P: drive also allows permanent storage. This drive is accessible by anyone on the same project, but not across projects. This is the only drive outside of the user drive where saved files will not be erased after logging out of the ADRF.

### PR Schema
Each project will have a project-specific database created. All members of the project will have read and write permissions for data and may also create their own objects (tables, etc.). The project databases are prefixed with pr-.

## Ineligible locations to do your work
The G: drive (data), the L: drive (Libs), and the desktop are not eligible for long-term file storing. You won’t have permissions to write to either the G: drive or the L: drive. The desktop will function only as temporary storage—as soon as a user is logged out of the ADRF, your desktop will be cleared. Additionally, since Wi-Fi connectivity can be imperfect, desktop storage for any amount of time is not recommended.

## Storage Size Restrictions and Best Practices
**Storage size** varies by project, but is capped at a predetermined amount. Additional storage costs may vary depending on the resource requirements.

**Best Practices**: 
- To save storage space, **avoid saving copies of raw data tables**. Instead, write code to **access data**. For detailed instructions on how to access data in structed data storage, please see the ADRF's [Redshift Querying Guide](11-querying-guide.md)
- Organize folders in a way that makes sense for your particular project. For example, you might have folders for a particular analysis or sub-projects. Dates on file names can be helpful for version control.
- Keep tabs on how much storage you are using compared to the allocated amount of storage.

---
[⬅️ Previous: How to Access Data](05-access-data.md) | [Back to Home](0-cover.md) | [Next: How to Work Collaboratively in the ADRF ➡️](07-collaborate.md)
