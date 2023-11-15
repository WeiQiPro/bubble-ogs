# Bubble-OGS Integration Guide

Integrate Online Go Server (OGS) games seamlessly into your Bubble application. This guide outlines the steps to display and interact with OGS games in Bubble.

## Setup Instructions

### Step 1: Inject JavaScript into Bubble

Paste the `jsDomloader` script into an HTML element within your Bubble application. This script is responsible for initializing and managing the Go board elements.

**Example:**

![jsDomLoader Script](https://github.com/WeiQiPro/bubble-ogs/assets/108106416/7d053a15-bddc-4e2f-bcea-df22aa0ee6b8)

### Step 2: Create Board Display Elements

You need to create another HTML element where the Go board will be displayed. You can use any HTML element capable of creating a `div`, such as a Repeating Group.

**Data Format:** The data source for this element should contain the `type` of the game (e.g., 'demo' or 'game') and the OGS game `id` (e.g., '1234565'). Ensure that the text within each `div` correctly reflects this data format.

**Example:**

![Board Display Element](https://github.com/WeiQiPro/bubble-ogs/assets/108106416/beceedc6-a72d-4959-8c79-c159df691e11)

### Step 3: Configure the Custom JavaScript Trigger

Set up a custom trigger to run JavaScript in Bubble. Use the `start(properties)` function in your script to activate the board setup.

**Parameters:**
- `param1`: URL of the board image.
- `param2`: URL of the black stone image.
- `param3`: URL of the white stone image.

Feel free to use any images that fit your design preferences.

**Example:**

![Custom JavaScript Trigger](https://github.com/WeiQiPro/bubble-ogs/assets/108106416/273757e5-d716-456f-9461-f0202f223ffd)

### Step 4: Initialization

Once set up, `jsDomLoader` will locate all unique Go boards (`gobans`) on the page. The boards will be initialized and ready for game play based on the provided game types and IDs.

---

## Additional Notes

- Ensure that all script and image URLs are correct and accessible.
- Verify that the game data format matches the expected structure in the scripts.
- Regularly check for updates to the integration scripts for new features or bug fixes.

For more information or support, visit [WeiQiPro's GitHub repository](https://github.com/WeiQiPro/bubble-ogs).

---
