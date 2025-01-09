# Bluesky Interaction Bot

The Bluesky Interaction Bot automates several tasks for interacting with Bluesky accounts, including fetching followers, fetching users who liked a post, and following users from a list.

---

## Features
1. Fetch followers of a specific profile and save them to a JSON file.
2. Fetch users who liked a specific post and save them to a JSON file.
3. Follow users from a JSON file (followers or likers).
4. Track successfully followed users to avoid duplicates.

---

## Prerequisites
- Bluesky account credentials.

---

## Setup
### 1. Download the Executable
Download the `Bluesky Interaction Bot` executable file 

---

## Usage Instructions

### 1. Login to Your Bluesky Account
- Log in to your Bluesky account through the platform.
- Retrieve your **Bearer Token** from the developer tools or API keys section.

### 2. Run the Bot
Run the downloaded executable file by double-clicking it.

### 3. Input Required Details
- Enter your **Bearer Token** when prompted.
- Enter your **Bluesky Handle** (e.g., `yourname.bsky.social`).

---

## Actions Available

### **1. Fetch Followers**
- Choose option `1` from the menu.
- Provide the profile URL of the user whose followers you want to fetch.
  Example: https://bsky.app/profile/username.bsky.social
- Followers will be saved to a file named `followers.json`.

### **2. Fetch Users Who Liked a Post**
- Choose option `2` from the menu.
- Provide the post URL.
Example:https://bsky.app/profile/username.bsky.social/post/post_id/liked-by
- Users who liked the post will be saved to a file named `post_likers.json`.

### **3. Follow Users from a JSON File**
- Choose option `3` from the menu.
- Provide the JSON file name containing the users you want to follow:
- `followers.json` for followers.
- `post_likers.json` for post likers.
- The bot will:
- Follow users listed in the provided file.
- Track successfully followed users in `followed.json` to prevent duplicates.
- Retain unfollowed users in the original file for retry.

### **4. Exit**
- Choose option `4` from the menu to safely exit the program.

---

## Output Files
1. **followers.json**: Contains the list of followers fetched from a profile.
2. **post_likers.json**: Contains the list of users who liked a specific post.
3. **followed.json**: Tracks users who were successfully followed.

---

## Demonstration Videos
### 1. How to Fetch Followers and Likers
https://youtu.be/8FPZpdM2Y-c
### 2. How to Follow Users from a JSON File
https://youtu.be/8FPZpdM2Y-c

---

## Error Handling
- If an error occurs while fetching data or following users, the bot logs the issue and continues with the next task.
- Ensure the provided Bearer Token and URLs are correct to avoid API errors.

---

## Future Enhancements
1. Automate Bearer Token retrieval.
2. Add support for fetching posts dynamically based on user preferences.
3. Retry failed requests with exponential backoff.

---

## Support
For questions or support, please open an issue on the repository or contact the project maintainer.
https://t.me/abid982
