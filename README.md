# Advice-to-me
just an advice for myself

# 1. should use ProfileService for database
Why?
## Built for massive scalability
  low resource footprint, no excessive type checking. Great for 100+ player servers. ProfileService automatically spreads the DataStore API calls evenly within the auto-save loop timeframe.
## Auto-Saving and Backup Handling
  ProfileService supports auto-saving, manual save triggers, and even recovery from corrupted or missing data.
  You can set up data backups and default templates easily.
## Easier Multi-Server Handling
  If a player joins two servers at once, ProfileService automatically prevents duplicate sessions and ensures only one session is active.
## Built-in Events and Hooks
ProfileService has hooks like .ListenToRelease() and .ListenToProfileLoad().
Makes it easier to respond to data loading, saving, or errors.
