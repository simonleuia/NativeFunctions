# CloudNote

This project was developed as part of Assignment 3.

CloudNote is a collaborative note-taking app built with React Native (Expo) and Supabase.
The app allows multiple users to create, view, edit, and delete shared notes, now with support for images and notifications.

---

## GitHub Repository

Project source code:
https://github.com/simonleuia/NativeFunctions

---

## Features

* User authentication (sign up, login, logout)
* Persistent login (session is remembered)
* Create notes
* View all notes from all users
* Edit notes
* Delete notes with confirmation
* Attach images to notes (camera or gallery)
* Image preview before saving
* Local notifications when a new note is created
* Input validation (no empty fields)
* Success and error messages

---

## Requirements checklist

### Camera Integration

* [x] Permissions for camera and media library
* [x] User can take a photo inside the app
* [x] User can pick an image from gallery
* [x] Selected image is previewed before saving

---

### Storage & Validation

* [x] Client-side validation:
  * Max size 15MB
  * Allowed formats: JPG, PNG, WebP
* [x] Images uploaded to Supabase Storage
* [x] Unique file names used to prevent overwriting
* [x] Image URL stored in database and linked to note

---

### UI/UX (Images & Feedback)

* [x] Loading state during upload (spinner + disabled save button)
* [x] Images displayed without stretching (correct aspect ratio)
* [x] Images shown:
  * As thumbnails in note list
  * In full view in note details
* [x] Clear error messages for:
  * Invalid file format
  * File too large
  * Upload failure

---

### Notifications

* [x] System permission requested for notifications
* [x] Local notification triggered after saving a note
* [x] Notification includes note title

Example:
