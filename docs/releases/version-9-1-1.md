# Version 9.1.1

Version 9.1.1 is a BuddyPress maintenance and security release. It was released on August 18, 2021. 3 bugs were fixed and 3 security issues were addressed.

For version 9.1.1 the database version (bp_db_version in wp_options) was 12850, and the Trac revision was 13068.

## Fixes

- Activity: update the nonce used by the Activity Reply JS Fallback (#8545)
- Settings: do not try to validate a dismissed email change (#8538)
- Settings: make sure changing pwd from the General Screen encrypts it (#8539)
- Security: make sure the activation key is never included into responses of the BP REST API Signup endpoints
- Security: prevent potential SQL injections making sure the order by clause built inside the BP_Notifications_Notification::get_order_by_sql() only accepts an allowed list of column names
- Security: prevent potential SQL injections making sure the order by clause built inside the BP_Invitation::get_order_by_sql() only accepts an allowed list of column names
