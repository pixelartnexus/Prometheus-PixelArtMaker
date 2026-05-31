
# Privacy Policy for Prometheus

Effective date: 5/31/2026

Prometheus is a browser extension designed to preserve and restore editable Pixel Art Maker canvas data for posts archived by Prometheus users.

## Summary

Prometheus stores Pixel Art Maker post IDs and compressed canvas data so that other Prometheus users can restore editable offshoot canvases.

Prometheus does not collect passwords, cookies, browsing history, names, emails, or Pixel Art Maker account credentials.

## Data Prometheus stores

Prometheus stores the following data in a Supabase database:

- Pixel Art Maker post ID
- Compressed Pixel Art Maker `pixel_array` canvas data
- Canvas width
- Canvas height
- Selection width
- Selection height
- Source label
- Creation timestamp

The compressed `pixel_array` data represents the editable canvas data needed to restore a Pixel Art Maker offshoot.

## Data Prometheus does not store

Prometheus does not store:

- Passwords
- Cookies
- Login credentials
- Names
- Email addresses
- Browsing history
- Pixel Art Maker account information
- Post title
- Post description
- Channel name
- Image preview data

## When data is stored

Data is stored only when a user has Prometheus installed and saves a Pixel Art Maker post.

When Pixel Art Maker successfully returns a new post ID, Prometheus stores that post ID together with the compressed canvas data sent during the save request.

## When data is retrieved

When a Prometheus user opens a Pixel Art Maker offshoot page, Prometheus checks whether the post ID exists in the Prometheus archive.

If the post exists, Prometheus retrieves the compressed canvas data and restores it into the Pixel Art Maker editor.

If the post does not exist, Prometheus shows a message explaining that the post may have been uploaded before Prometheus existed or by someone who was not using Prometheus.

## Public accessibility

Prometheus is designed as a shared archive. Stored canvas data may be retrievable by post ID.

Users should not save private or sensitive artwork with Prometheus unless they are comfortable with the canvas data being available to other Prometheus users.

## Third-party services

Prometheus uses Supabase to store and retrieve archived canvas data.

Supabase may process technical request data according to its own policies and infrastructure.

## Security

Prometheus uses Supabase security protocals and database constraints to limit database access.

The database is intended to allow:

- Reading archived posts
- Inserting new archived posts

The database is not intended to allow public updates or public deletes.

Prometheus also rejects canvas data larger than 500 by 500 pixels.

## Changes to this policy

This privacy policy may be updated as Prometheus changes.

## Contact

For questions or concerns about Prometheus, contact:

pixelartnexus@gmail.com
